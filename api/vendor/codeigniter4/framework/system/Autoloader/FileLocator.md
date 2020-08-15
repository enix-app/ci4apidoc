


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Autoloader/FileLocator.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/Autoloader.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">next</a></td>
</tr>
</table>







# CodeIgniter\Autoloader 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Autoloader</td></tr>
</table>

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CodeIgniter
</td></tr>
</table>

<table>
<tr><td>
An open source application development framework for PHP

This content is released under the MIT License (MIT)

Copyright (c) 2014-2019 British Columbia Institute of Technology
Copyright (c) 2019-2020 CodeIgniter Foundation

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter
</td>
</tr>
<tr style="vertical-align:top;">
<th>author</th>
<td>CodeIgniter Dev Team
</td>
</tr>
<tr style="vertical-align:top;">
<th>copyright</th>
<td>2019-2020 CodeIgniter Foundation
</td>
</tr>
<tr style="vertical-align:top;">
<th>license</th>
<td><a href="https://opensource.org/licenses/MIT">https://opensource.org/licenses/MIT</a>	MIT License
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com">https://codeigniter.com</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>filesource</th>
<td>framework/system/Autoloader/FileLocator.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/Autoloader.md">CodeIgniter\Autoloader\Autoloader</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/FileLocator.md">CodeIgniter\Autoloader\FileLocator</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Autoloader\FileLocator

<table style="text-align:left">
<tr><th>Class</th><td>FileLocator</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Autoloader\FileLocator</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class FileLocator
</td></tr>
</table>

<table>
<tr><td>
Allows loading non-class files in a namespaced manner.
Works with Helpers, Views, etc.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter
</td>
</tr>
</table>



### Summary


<table style="text-align:left;">
<tr>
<th>Name</th>
<th>Element</th>
<th>Modifier</th>
<th>Description</th>
</tr>

<tr>
<th><a href="#autoloader"><strong>autoloader</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Autoloader to use.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor</td>
</tr>
<tr>
<th><a href="#locateFile"><strong>locateFile</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attempts to locate a file by examining the name for a namespace
and looking through the PSR-4 namespaced files that we know about.</td>
</tr>
<tr>
<th><a href="#getClassname"><strong>getClassname</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Examines a file and returns the fully qualified domain name.</td>
</tr>
<tr>
<th><a href="#search"><strong>search</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Searches through all of the defined namespaces looking for a file.</td>
</tr>
<tr>
<th><a href="#ensureExt"><strong>ensureExt</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Ensures a extension is at the end of a filename</td>
</tr>
<tr>
<th><a href="#getNamespaces"><strong>getNamespaces</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Return the namespace mappings we know about.</td>
</tr>
<tr>
<th><a href="#findQualifiedNameFromPath"><strong>findQualifiedNameFromPath</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Find the qualified name of a file according to
the namespace of the first matched namespace path.</td>
</tr>
<tr>
<th><a href="#listFiles"><strong>listFiles</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Scans the defined namespaces, returning a list of all files
that are contained within the subpath specified by $path.</td>
</tr>
<tr>
<th><a href="#listNamespaceFiles"><strong>listNamespaceFiles</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Scans the provided namespace, returning a list of all files
that are contained within the subpath specified by $path.</td>
</tr>
<tr>
<th><a href="#legacyLocate"><strong>legacyLocate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Checks the application folder to see if the file can be found.</td>
</tr>

</table>





### Properties


<hr>

#### $autoloader

```php
protected $autoloader;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Autoloader to use.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Autoloader\Autoloader
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(Autoloader $autoloader)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor
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
<td><code>$autoloader</code></td>
<td><em>\Autoloader
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (66 - 69)</small></summary>

```php
public function __construct(Autoloader $autoloader)
{
	$this->autoloader = $autoloader;
}
```

</details>


<hr>

#### locateFile()

```php
public function locateFile(string $file, string $folder = null, string $ext = 'php')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to locate a file by examining the name for a namespace
and looking through the PSR-4 namespaced files that we know about.
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
<td>The namespaced file to locate</td>
</tr>

<tr>
<td>2.</td>
<td><code>$folder</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The folder within the namespace that we should look for the file.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$ext</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The file extension the file should have.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 77 lines (83 - 159)</small></summary>

```php
public function locateFile(string $file, string $folder = null, string $ext = 'php')
{
	$file = $this->ensureExt($file, $ext);

	// Clears the folder name if it is at the beginning of the filename
	if (! empty($folder) && ($pos = strpos($file, $folder)) === 0)
	{
		$file = substr($file, strlen($folder . '/'));
	}

	// Is not namespaced? Try the application folder.
	if (strpos($file, '\\') === false)
	{
		return $this->legacyLocate($file, $folder);
	}

	// Standardize slashes to handle nested directories.
	$file = strtr($file, '/', '\\');

	$segments = explode('\\', $file);

	// The first segment will be empty if a slash started the filename.
	if (empty($segments[0]))
	{
		unset($segments[0]);
	}

	$paths    = [];
	$prefix   = '';
	$filename = '';

	// Namespaces always comes with arrays of paths
	$namespaces = $this->autoloader->getNamespace();

	while (! empty($segments))
	{
		$prefix .= empty($prefix) ? array_shift($segments) : '\\' . array_shift($segments);

		if (empty($namespaces[$prefix]))
		{
			continue;
		}
		$paths = $namespaces[$prefix];

		$filename = implode('/', $segments);
		break;
	}

	// if no namespaces matched then quit
	if (empty($paths))
	{
		return false;
	}

	// Check each path in the namespace
	foreach ($paths as $path)
	{
		// Ensure trailing slash
		$path = rtrim($path, '/') . '/';

		// If we have a folder name, then the calling function
		// expects this file to be within that folder, like 'Views',
		// or 'libraries'.
		if (! empty($folder) && strpos($path . $filename, '/' . $folder . '/') === false)
		{
			$path .= trim($folder, '/') . '/';
		}

		$path .= $filename;
		if (is_file($path))
		{
			return $path;
		}
	}

	return false;
}
```

</details>


<hr>

#### getClassname()

```php
public function getClassname(string $file) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Examines a file and returns the fully qualified domain name.
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
<td></td>
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
<summary><small>Source: 47 lines (170 - 216)</small></summary>

```php
public function getClassname(string $file) : string
{
	$php        = file_get_contents($file);
	$tokens     = token_get_all($php);
	$dlm        = false;
	$namespace  = '';
	$class_name = '';

	foreach ($tokens as $i => $token)
	{
		if ($i < 2)
		{
			continue;
		}

		if ((isset($tokens[$i - 2][1]) && ($tokens[$i - 2][1] === 'phpnamespace' || $tokens[$i - 2][1] === 'namespace')) || ($dlm && $tokens[$i - 1][0] === T_NS_SEPARATOR && $token[0] === T_STRING))
		{
			if (! $dlm)
			{
				$namespace = 0;
			}
			if (isset($token[1]))
			{
				$namespace = $namespace ? $namespace . '\\' . $token[1] : $token[1];
				$dlm       = true;
			}
		}
		elseif ($dlm && ($token[0] !== T_NS_SEPARATOR) && ($token[0] !== T_STRING))
		{
			$dlm = false;
		}
		if (($tokens[$i - 2][0] === T_CLASS || (isset($tokens[$i - 2][1]) && $tokens[$i - 2][1] === 'phpclass'))
			&& $tokens[$i - 1][0] === T_WHITESPACE
			&& $token[0] === T_STRING)
		{
			$class_name = $token[1];
			break;
		}
	}

	if (empty( $class_name ))
	{
		return '';
	}

	return $namespace . '\\' . $class_name;
}
```

</details>


<hr>

#### search()

```php
public function search(string $path, string $ext = 'php', bool $prioritizeApp = true) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Searches through all of the defined namespaces looking for a file.
</td></tr>
</table>

<table>
<tr><td>
Returns an array of all found locations for the defined file.

Example:

 $locator->search('Config/Routes.php');
 // Assuming PSR4 namespaces include foo and bar, might return:
 [
     'app/Modules/foo/Config/Routes.php',
     'app/Modules/bar/Config/Routes.php',
 ]
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
<td><code>$ext</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$prioritizeApp</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
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
<summary><small>Source: 40 lines (239 - 278)</small></summary>

```php
public function search(string $path, string $ext = 'php', bool $prioritizeApp = true): array
{
	$path = $this->ensureExt($path, $ext);

	$foundPaths = [];
	$appPaths   = [];

	foreach ($this->getNamespaces() as $namespace)
	{
		if (isset($namespace['path']) && is_file($namespace['path'] . $path))
		{
			$fullPath = $namespace['path'] . $path;
			if ($prioritizeApp)
			{
				$foundPaths[] = $fullPath;
			}
			else
			{
				if (strpos($fullPath, APPPATH) === 0)
				{
					$appPaths[] = $fullPath;
				}
				else
				{
					$foundPaths[] = $fullPath;
				}
			}
		}
	}

	if (! $prioritizeApp && ! empty($appPaths))
	{
		$foundPaths = array_merge($foundPaths, $appPaths);
	}

	// Remove any duplicates
	$foundPaths = array_unique($foundPaths);

	return $foundPaths;
}
```

</details>


<hr>

#### ensureExt()

```php
protected function ensureExt(string $path, string $ext) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ensures a extension is at the end of a filename
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
<td><code>$ext</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
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
<summary><small>Source: 14 lines (290 - 303)</small></summary>

```php
protected function ensureExt(string $path, string $ext): string
{
	if ($ext)
	{
		$ext = '.' . $ext;

		if (substr($path, -strlen($ext)) !== $ext)
		{
			$path .= $ext;
		}
	}

	return $path;
}
```

</details>


<hr>

#### getNamespaces()

```php
protected function getNamespaces()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the namespace mappings we know about.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 32 lines (312 - 343)</small></summary>

```php
protected function getNamespaces()
{
	$namespaces = [];

	// Save system for last
	$system = [];

	foreach ($this->autoloader->getNamespace() as $prefix => $paths)
	{
		foreach ($paths as $path)
		{
			if ($prefix === 'CodeIgniter')
			{
				$system = [
					'prefix' => $prefix,
					'path'   => rtrim($path, '\\/') . DIRECTORY_SEPARATOR,
				];

				continue;
			}

			$namespaces[] = [
				'prefix' => $prefix,
				'path'   => rtrim($path, '\\/') . DIRECTORY_SEPARATOR,
			];
		}
	}

	$namespaces[] = $system;

	return $namespaces;
}
```

</details>


<hr>

#### findQualifiedNameFromPath()

```php
public function findQualifiedNameFromPath(string $path)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Find the qualified name of a file according to
the namespace of the first matched namespace path.
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


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 37 lines (355 - 391)</small></summary>

```php
public function findQualifiedNameFromPath(string $path)
{
	$path = realpath($path);

	if (! $path)
	{
		return false;
	}

	foreach ($this->getNamespaces() as $namespace)
	{
		$namespace['path'] = realpath($namespace['path']);

		if (empty($namespace['path']))
		{
			continue;
		}

		if (mb_strpos($path, $namespace['path']) === 0)
		{
			$className = '\\' . $namespace['prefix'] . '\\' .
					ltrim(str_replace('/', '\\', mb_substr(
						$path, mb_strlen($namespace['path']))
					), '\\');
			// Remove the file extension (.php)
			$className = mb_substr($className, 0, -4);

			// Check if this exists
			if (class_exists($className))
			{
				return $className;
			}
		}
	}

	return false;
}
```

</details>


<hr>

#### listFiles()

```php
public function listFiles(string $path) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Scans the defined namespaces, returning a list of all files
that are contained within the subpath specified by $path.
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
<summary><small>Source: 29 lines (403 - 431)</small></summary>

```php
public function listFiles(string $path): array
{
	if (empty($path))
	{
		return [];
	}

	$files = [];
	helper('filesystem');

	foreach ($this->getNamespaces() as $namespace)
	{
		$fullPath = realpath($namespace['path'] . $path);

		if (! is_dir($fullPath))
		{
			continue;
		}

		$tempFiles = get_filenames($fullPath, true);

		if (! empty($tempFiles))
		{
			$files = array_merge($files, $tempFiles);
		}
	}

	return $files;
}
```

</details>


<hr>

#### listNamespaceFiles()

```php
public function listNamespaceFiles(string $prefix, string $path) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Scans the provided namespace, returning a list of all files
that are contained within the subpath specified by $path.
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
<td><code>$prefix</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
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
<summary><small>Source: 30 lines (444 - 473)</small></summary>

```php
public function listNamespaceFiles(string $prefix, string $path): array
{
	if (empty($path) || empty($prefix))
	{
		return [];
	}

	$files = [];
	helper('filesystem');

	// autoloader->getNamespace($prefix) returns an array of paths for that namespace
	foreach ($this->autoloader->getNamespace($prefix) as $namespacePath)
	{
		$fullPath = realpath(rtrim($namespacePath, '/') . '/' . $path);

		if (! is_dir($fullPath))
		{
			continue;
		}

		$tempFiles = get_filenames($fullPath, true);

		if (! empty($tempFiles))
		{
			$files = array_merge($files, $tempFiles);
		}
	}

	return $files;
}
```

</details>


<hr>

#### legacyLocate()

```php
protected function legacyLocate(string $file, string $folder = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks the application folder to see if the file can be found.
</td></tr>
</table>

<table>
<tr><td>
Only for use with filenames that DO NOT include namespacing.
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
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$folder</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 19 lines (486 - 504)</small></summary>

```php
protected function legacyLocate(string $file, string $folder = null)
{
	$paths = [
		APPPATH,
		SYSTEMPATH,
	];

	foreach ($paths as $path)
	{
		$path .= empty($folder) ? $file : $folder . '/' . $file;

		if (is_file($path))
		{
			return $path;
		}
	}

	return false;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Autoloader/FileLocator.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/Autoloader.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>