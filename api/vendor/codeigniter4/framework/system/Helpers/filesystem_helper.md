


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/filesystem_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/inflector_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/filesystem_helper.md">next</a></td>
</tr>
</table>




 



# Filesystem Helper


<hr>

## directory_map()

```php
function directory_map(string $source_dir, int $directory_depth = 0, bool $hidden = false) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create a Directory Map
</td></tr>
</table>

<table>
<tr><td>
Reads the specified directory and builds an array
representation of it. Sub-folders contained with the
directory will be mapped as well.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$source_dir</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Path to source</td>
</tr>

<tr>
<td>2.</td>
<td><code>$directory_depth</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Depth of directories to traverse
(0 = fully recursive, 1 = current dir, etc)</td>
</tr>

<tr>
<td>3.</td>
<td><code>$hidden</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to show hidden files</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 38 lines (64 - 101)</small></summary>

```php
function directory_map(string $source_dir, int $directory_depth = 0, bool $hidden = false): array
{
	try
	{
		$fp = opendir($source_dir);

		$fileData   = [];
		$new_depth  = $directory_depth - 1;
		$source_dir = rtrim($source_dir, DIRECTORY_SEPARATOR) . DIRECTORY_SEPARATOR;

		while (false !== ($file = readdir($fp)))
		{
			// Remove '.', '..', and hidden files [optional]
			if ($file === '.' || $file === '..' || ($hidden === false && $file[0] === '.'))
			{
				continue;
			}

			is_dir($source_dir . $file) && $file .= DIRECTORY_SEPARATOR;

			if (($directory_depth < 1 || $new_depth > 0) && is_dir($source_dir . $file))
			{
				$fileData[$file] = directory_map($source_dir . $file, $new_depth, $hidden);
			}
			else
			{
				$fileData[] = $file;
			}
		}

		closedir($fp);
		return $fileData;
	}
	catch (\Throwable $e)
	{
		return [];
	}
}
```

</details>


<hr>

## write_file()

```php
function write_file(string $path, string $data, string $mode = 'wb') : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Write File
</td></tr>
</table>

<table>
<tr><td>
Writes data to the file specified in the path.
Creates a new file if non-existent.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>File path</td>
</tr>

<tr>
<td>2.</td>
<td><code>$data</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Data to write</td>
</tr>

<tr>
<td>3.</td>
<td><code>$mode</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>fopen() mode (default: 'wb')</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 26 lines (120 - 145)</small></summary>

```php
function write_file(string $path, string $data, string $mode = 'wb'): bool
{
	try
	{
		$fp = fopen($path, $mode);

		flock($fp, LOCK_EX);

		for ($result = $written = 0, $length = strlen($data); $written < $length; $written += $result)
		{
			if (($result = fwrite($fp, substr($data, $written))) === false)
			{
				break;
			}
		}

		flock($fp, LOCK_UN);
		fclose($fp);

		return is_int($result);
	}
	catch (\Throwable $e)
	{
		return false;
	}
}
```

</details>


<hr>

## delete_files()

```php
function delete_files(string $path, bool $del_dir = false, bool $htdocs = false, bool $hidden = false) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Delete Files
</td></tr>
</table>

<table>
<tr><td>
Deletes all files contained in the supplied directory path.
Files must be writable or owned by the system in order to be deleted.
If the second parameter is set to true, any directories contained
within the supplied base directory will be nuked as well.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>File path</td>
</tr>

<tr>
<td>2.</td>
<td><code>$del_dir</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to delete any directories found in the path</td>
</tr>

<tr>
<td>3.</td>
<td><code>$htdocs</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to skip deleting .htaccess and index page files</td>
</tr>

<tr>
<td>4.</td>
<td><code>$hidden</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to include hidden files (files beginning with a period)</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 42 lines (167 - 208)</small></summary>

```php
function delete_files(string $path, bool $del_dir = false, bool $htdocs = false, bool $hidden = false): bool
{
	$path = realpath($path) ?: $path;
	$path = rtrim($path, DIRECTORY_SEPARATOR) . DIRECTORY_SEPARATOR;

	try
	{
		foreach (new RecursiveIteratorIterator(
			new RecursiveDirectoryIterator($path, RecursiveDirectoryIterator::SKIP_DOTS),
			RecursiveIteratorIterator::CHILD_FIRST
		) as $object)
		{
			$filename = $object->getFilename();

			if (! $hidden && $filename[0] === '.')
			{
				continue;
			}
			elseif (! $htdocs || ! preg_match('/^(\.htaccess|index\.(html|htm|php)|web\.config)$/i', $filename))
			{
				$isDir = $object->isDir();

				if ($isDir && $del_dir)
				{
					@rmdir($object->getPathname());
					continue;
				}

				if (! $isDir)
				{
					@unlink($object->getPathname());
				}
			}
		}

		return true;
	}
	catch (\Throwable $e)
	{
		return false;
	}
}
```

</details>


<hr>

## get_filenames()

```php
function get_filenames(string $source_dir, ?bool $include_path = false, bool $hidden = false) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get Filenames
</td></tr>
</table>

<table>
<tr><td>
Reads the specified directory and builds an array containing the filenames.
Any sub-folders contained within the specified path are read as well.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$source_dir</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Path to source</td>
</tr>

<tr>
<td>2.</td>
<td><code>$include_path</code></td>
<td><em>bool<br>null
</em></td>
<td>false</td>
<td>Whether to include the path as part of the filename; false for no path, null for a relative path, true for full path</td>
</tr>

<tr>
<td>3.</td>
<td><code>$hidden</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to include hidden files (files beginning with a period)</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 43 lines (227 - 269)</small></summary>

```php
function get_filenames(string $source_dir, ?bool $include_path = false, bool $hidden = false): array
{
	$files = [];

	$source_dir = realpath($source_dir) ?: $source_dir;
	$source_dir = rtrim($source_dir, DIRECTORY_SEPARATOR) . DIRECTORY_SEPARATOR;

	try
	{
		foreach (new RecursiveIteratorIterator(
				new RecursiveDirectoryIterator($source_dir, RecursiveDirectoryIterator::SKIP_DOTS),
				RecursiveIteratorIterator::SELF_FIRST
			) as $name => $object)
		{
			$basename = pathinfo($name, PATHINFO_BASENAME);

			if (! $hidden && $basename[0] === '.')
			{
				continue;
			}
			elseif ($include_path === false)
			{
				$files[] = $basename;
			}
			elseif (is_null($include_path))
			{
				$files[] = str_replace($source_dir, '', $name);
			}
			else
			{
				$files[] = $name;
			}
		}
	}
	catch (\Throwable $e)
	{
		return [];
	}

	sort($files);

	return $files;
}
```

</details>


<hr>

## get_dir_file_info()

```php
function get_dir_file_info(string $source_dir, bool $top_level_only = true, bool $recursion = false) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get Directory File Information
</td></tr>
</table>

<table>
<tr><td>
Reads the specified directory and builds an array containing the filenames,
filesize, dates, and permissions

Any sub-folders contained within the specified path are read as well.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$source_dir</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Path to source</td>
</tr>

<tr>
<td>2.</td>
<td><code>$top_level_only</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Look only at the top level directory specified?</td>
</tr>

<tr>
<td>3.</td>
<td><code>$recursion</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Internal variable to determine recursion status - do not use in calls</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 38 lines (290 - 327)</small></summary>

```php
function get_dir_file_info(string $source_dir, bool $top_level_only = true, bool $recursion = false): array
{
	static $fileData = [];
	$relative_path   = $source_dir;

	try
	{
		$fp = @opendir($source_dir); {
			// reset the array and make sure $source_dir has a trailing slash on the initial call
		if ($recursion === false)
			{
			$fileData   = [];
			$source_dir = rtrim(realpath($source_dir), DIRECTORY_SEPARATOR) . DIRECTORY_SEPARATOR;
		}

			// Used to be foreach (scandir($source_dir, 1) as $file), but scandir() is simply not as fast
		while (false !== ($file = readdir($fp)))
			{
			if (is_dir($source_dir . $file) && $file[0] !== '.' && $top_level_only === false)
			{
				get_dir_file_info($source_dir . $file . DIRECTORY_SEPARATOR, $top_level_only, true);
			}
			elseif ($file[0] !== '.')
			{
				$fileData[$file]                  = get_file_info($source_dir . $file);
				$fileData[$file]['relative_path'] = $relative_path;
			}
		}

			closedir($fp);
			return $fileData;
		}
	}
	catch (\Throwable $fe)
	{
		return [];
	}
}
```

</details>


<hr>

## get_file_info()

```php
function get_file_info(string $file, $returned_values = array('name', 'server_path', 'size', 'date'))
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get File Info
</td></tr>
</table>

<table>
<tr><td>
Given a file and path, returns the name, path, size, date modified
Second parameter allows you to explicitly declare what information you want returned
Options are: name, server_path, size, date, readable, writable, executable, fileperms
Returns false if the file cannot be found.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$file</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Path to file</td>
</tr>

<tr>
<td>2.</td>
<td><code>$returned_values</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Array or comma separated string of information returned</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 44 lines (347 - 390)</small></summary>

```php
function get_file_info(string $file, $returned_values = ['name', 'server_path', 'size', 'date'])
{
	if (! is_file($file))
	{
		return null;
	}

	if (is_string($returned_values))
	{
		$returned_values = explode(',', $returned_values);
	}

	foreach ($returned_values as $key)
	{
		switch ($key) {
			case 'name':
				$fileInfo['name'] = basename($file);
				break;
			case 'server_path':
				$fileInfo['server_path'] = $file;
				break;
			case 'size':
				$fileInfo['size'] = filesize($file);
				break;
			case 'date':
				$fileInfo['date'] = filemtime($file);
				break;
			case 'readable':
				$fileInfo['readable'] = is_readable($file);
				break;
			case 'writable':
				$fileInfo['writable'] = is_really_writable($file);
				break;
			case 'executable':
				$fileInfo['executable'] = is_executable($file);
				break;
			case 'fileperms':
				$fileInfo['fileperms'] = fileperms($file);
				break;
		}
	}

	return $fileInfo;
}
```

</details>


<hr>

## symbolic_permissions()

```php
function symbolic_permissions(int $perms) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Symbolic Permissions
</td></tr>
</table>

<table>
<tr><td>
Takes a numeric value representing a file's permissions and returns
standard symbolic notation representing that value
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$perms</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Permissions</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 52 lines (406 - 457)</small></summary>

```php
function symbolic_permissions(int $perms): string
{
	if (($perms & 0xC000) === 0xC000)
	{
		$symbolic = 's'; // Socket
	}
	elseif (($perms & 0xA000) === 0xA000)
	{
		$symbolic = 'l'; // Symbolic Link
	}
	elseif (($perms & 0x8000) === 0x8000)
	{
		$symbolic = '-'; // Regular
	}
	elseif (($perms & 0x6000) === 0x6000)
	{
		$symbolic = 'b'; // Block special
	}
	elseif (($perms & 0x4000) === 0x4000)
	{
		$symbolic = 'd'; // Directory
	}
	elseif (($perms & 0x2000) === 0x2000)
	{
		$symbolic = 'c'; // Character special
	}
	elseif (($perms & 0x1000) === 0x1000)
	{
		$symbolic = 'p'; // FIFO pipe
	}
	else
	{
		$symbolic = 'u'; // Unknown
	}

	// Owner
	$symbolic .= (($perms & 0x0100) ? 'r' : '-')
			. (($perms & 0x0080) ? 'w' : '-')
			. (($perms & 0x0040) ? (($perms & 0x0800) ? 's' : 'x' ) : (($perms & 0x0800) ? 'S' : '-'));

	// Group
	$symbolic .= (($perms & 0x0020) ? 'r' : '-')
			. (($perms & 0x0010) ? 'w' : '-')
			. (($perms & 0x0008) ? (($perms & 0x0400) ? 's' : 'x' ) : (($perms & 0x0400) ? 'S' : '-'));

	// World
	$symbolic .= (($perms & 0x0004) ? 'r' : '-')
			. (($perms & 0x0002) ? 'w' : '-')
			. (($perms & 0x0001) ? (($perms & 0x0200) ? 't' : 'x' ) : (($perms & 0x0200) ? 'T' : '-'));

	return $symbolic;
}
```

</details>


<hr>

## octal_permissions()

```php
function octal_permissions(int $perms) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Octal Permissions
</td></tr>
</table>

<table>
<tr><td>
Takes a numeric value representing a file's permissions and returns
a three character string representing the file's octal permissions
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$perms</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Permissions</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (473 - 476)</small></summary>

```php
function octal_permissions(int $perms): string
{
	return substr(sprintf('%o', $perms), -3);
}
```

</details>


<hr>

## set_realpath()

```php
function set_realpath(string $path, bool $check_existence = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Realpath
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>


**Params**

<table>
<thead>
<tr>
<th>#</th>
<th>Variable</th>
<th>Type</th>
<th>Variadic</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr>
<td>1.</td>
<td><code>$path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$check_existence</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Checks to see if the path exists</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 21 lines (491 - 511)</small></summary>

```php
function set_realpath(string $path, bool $check_existence = false): string
{
	// Security check to make sure the path is NOT a URL. No remote file inclusion!
	if (preg_match('#^(http:\/\/|https:\/\/|www\.|ftp)#i', $path) || filter_var($path, FILTER_VALIDATE_IP) === $path)
	{
		throw new InvalidArgumentException('The path you submitted must be a local server path, not a URL');
	}

	// Resolve the path
	if (realpath($path) !== false)
	{
		$path = realpath($path);
	}
	elseif ($check_existence && ! is_dir($path) && ! is_file($path))
	{
		throw new InvalidArgumentException('Not a valid path: ' . $path);
	}

	// Add a trailing slash, if this is a directory
	return is_dir($path) ? rtrim($path, DIRECTORY_SEPARATOR) . DIRECTORY_SEPARATOR : $path;
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/filesystem_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/inflector_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/filesystem_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:25**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>