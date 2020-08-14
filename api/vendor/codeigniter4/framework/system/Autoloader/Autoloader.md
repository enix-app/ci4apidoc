


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Autoloader/Autoloader.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/API/ResponseTrait.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/FileLocator.md">next</a></td>
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
<td>framework/system/Autoloader/Autoloader.php
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



 

 
## CodeIgniter\Autoloader\Autoloader

<table style="text-align:left">
<tr><th>Class</th><td>Autoloader</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Autoloader\Autoloader</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CodeIgniter Autoloader
</td></tr>
</table>

<table>
<tr><td>
An autoloader that uses both PSR4 autoloading, and traditional classmaps.

Given a foo-bar package of classes in the file system at the following paths:

     /path/to/packages/foo-bar/
         /src
             Baz.php         # Foo\Bar\Baz
             Qux/
                 Quux.php    # Foo\Bar\Qux\Quux

you can add the path to the configuration array that is passed in the constructor.
The Config array consists of 2 primary keys, both of which are associative arrays:
'psr4', and 'classmap'.

     $Config = [
         'psr4' => [
             'Foo\Bar'   => '/path/to/packages/foo-bar'
         ],
         'classmap' => [
             'MyClass'   => '/path/to/class/file.php'
         ]
     ];

Example:

     <?php
     // our configuration array
     $Config = [ ... ];
     $loader = new \CodeIgniter\Autoloader\Autoloader($Config);

     // register the autoloader
     $loader->register();
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Autoloader
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
<th><a href="#prefixes"><strong>prefixes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores namespaces as key, and path as values.</td>
</tr>
<tr>
<th><a href="#classmap"><strong>classmap</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores class name as key, and path as values.</td>
</tr>

<tr>
<th><a href="#initialize"><strong>initialize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Reads in the configuration array (described above) and stores
the valid parts that we&#039;ll need.</td>
</tr>
<tr>
<th><a href="#register"><strong>register</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Register the loader with the SPL autoloader stack.</td>
</tr>
<tr>
<th><a href="#addNamespace"><strong>addNamespace</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Registers namespaces with the autoloader.</td>
</tr>
<tr>
<th><a href="#getNamespace"><strong>getNamespace</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get namespaces with prefixes as keys and paths as values.</td>
</tr>
<tr>
<th><a href="#removeNamespace"><strong>removeNamespace</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Removes a single namespace from the psr4 settings.</td>
</tr>
<tr>
<th><a href="#loadClass"><strong>loadClass</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Loads the class file for a given class name.</td>
</tr>
<tr>
<th><a href="#loadInNamespace"><strong>loadInNamespace</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Loads the class file for a given class name.</td>
</tr>
<tr>
<th><a href="#loadLegacy"><strong>loadLegacy</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Attempts to load the class from common locations in previous
version of CodeIgniter, namely &#039;app/Libraries&#039;, and
&#039;app/Models&#039;.</td>
</tr>
<tr>
<th><a href="#requireFile"><strong>requireFile</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A central way to require a file is loaded. Split out primarily
for testing purposes.</td>
</tr>
<tr>
<th><a href="#sanitizeFilename"><strong>sanitizeFilename</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sanitizes a filename, replacing spaces with dashes.</td>
</tr>
<tr>
<th><a href="#discoverComposerNamespaces"><strong>discoverComposerNamespaces</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Locates all PSR4 compatible namespaces from Composer.</td>
</tr>

</table>





### Properties


<hr>

#### $prefixes

```php
protected $prefixes = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores namespaces as key, and path as values.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
</tr>
</table>


<hr>

#### $classmap

```php
protected $classmap = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores class name as key, and path as values.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
</tr>
</table>







### Methods


<hr>

#### initialize()

```php
public function initialize(\Config\Autoload $config, \Config\Modules $moduleConfig)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reads in the configuration array (described above) and stores
the valid parts that we'll need.
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
<td><code>$config</code></td>
<td><em>\Config\Autoload
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$moduleConfig</code></td>
<td><em>\Config\Modules
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 27 lines (107 - 133)</small></summary>

```php
public function initialize(\Config\Autoload $config, \Config\Modules $moduleConfig)
{
	// We have to have one or the other, though we don't enforce the need
	// to have both present in order to work.
	if (empty($config->psr4) && empty($config->classmap))
	{
		throw new \InvalidArgumentException('Config array must contain either the \'psr4\' key or the \'classmap\' key.');
	}

	if (isset($config->psr4))
	{
		$this->addNamespace($config->psr4);
	}

	if (isset($config->classmap))
	{
		$this->classmap = $config->classmap;
	}

	// Should we load through Composer's namespaces, also?
	if ($moduleConfig->discoverInComposer)
	{
		$this->discoverComposerNamespaces();
	}

	return $this;
}
```

</details>


<hr>

#### register()

```php
public function register()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Register the loader with the SPL autoloader stack.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 26 lines (140 - 165)</small></summary>

```php
public function register()
{
	// Since the default file extensions are searched
	// in order of .inc then .php, but we always use .php,
	// put the .php extension first to eek out a bit
	// better performance.
	// http://php.net/manual/en/function.spl-autoload.php#78053
	spl_autoload_extensions('.php,.inc');

	// Prepend the PSR4  autoloader for maximum performance.
	spl_autoload_register([$this, 'loadClass'], true, true);

	// Now prepend another loader for the files in our class map.
	$config = is_array($this->classmap) ? $this->classmap : [];

	spl_autoload_register(function ($class) use ($config) {
		if (empty($config[$class]))
		{
			return false;
		}

		include_once $config[$class];
	}, true, // Throw exception
		true // Prepend
	);
}
```

</details>


<hr>

#### addNamespace()

```php
public function addNamespace($namespace, string $path = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Registers namespaces with the autoloader.
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
<td><code>$namespace</code></td>
<td><em>array<br>string
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
<td>\Autoloader
</td>
</tr>
</table>





<details>
<summary><small>Source: 28 lines (177 - 204)</small></summary>

```php
public function addNamespace($namespace, string $path = null)
{
	if (is_array($namespace))
	{
		foreach ($namespace as $prefix => $path)
		{
			$prefix = trim($prefix, '\\');

			if (is_array($path))
			{
				foreach ($path as $dir)
				{
					$this->prefixes[$prefix][] = rtrim($dir, '/') . '/';
				}

				continue;
			}

			$this->prefixes[$prefix][] = rtrim($path, '/') . '/';
		}
	}
	else
	{
		$this->prefixes[trim($namespace, '\\')][] = rtrim($path, '/') . '/';
	}

	return $this;
}
```

</details>


<hr>

#### getNamespace()

```php
public function getNamespace(string $prefix = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get namespaces with prefixes as keys and paths as values.
</td></tr>
</table>

<table>
<tr><td>
If a prefix param is set, returns only paths to the given prefix.
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (217 - 225)</small></summary>

```php
public function getNamespace(string $prefix = null)
{
	if ($prefix === null)
	{
		return $this->prefixes;
	}

	return $this->prefixes[trim($prefix, '\\')] ?? [];
}
```

</details>


<hr>

#### removeNamespace()

```php
public function removeNamespace(string $namespace)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes a single namespace from the psr4 settings.
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
<td><code>$namespace</code></td>
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
<td>\Autoloader
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (236 - 241)</small></summary>

```php
public function removeNamespace(string $namespace)
{
	unset($this->prefixes[trim($namespace, '\\')]);

	return $this;
}
```

</details>


<hr>

#### loadClass()

```php
public function loadClass(string $class)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Loads the class file for a given class name.
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
<td><code>$class</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The fully qualified class name.</td>
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
<summary><small>Source: 16 lines (253 - 268)</small></summary>

```php
public function loadClass(string $class)
{
	$class = trim($class, '\\');
	$class = str_ireplace('.php', '', $class);

	$mapped_file = $this->loadInNamespace($class);

	// Nothing? One last chance by looking
	// in common CodeIgniter folders.
	if (! $mapped_file)
	{
		$mapped_file = $this->loadLegacy($class);
	}

	return $mapped_file;
}
```

</details>


<hr>

#### loadInNamespace()

```php
protected function loadInNamespace(string $class)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Loads the class file for a given class name.
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
<td><code>$class</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The fully-qualified class name</td>
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
<summary><small>Source: 38 lines (279 - 316)</small></summary>

```php
protected function loadInNamespace(string $class)
{
	if (strpos($class, '\\') === false)
	{
		$class    = 'Config\\' . $class;
		$filePath = APPPATH . str_replace('\\', DIRECTORY_SEPARATOR, $class) . '.php';
		$filename = $this->requireFile($filePath);

		if ($filename)
		{
			return $filename;
		}

		return false;
	}

	foreach ($this->prefixes as $namespace => $directories)
	{
		foreach ($directories as $directory)
		{
			$directory = rtrim($directory, '\\/');

			if (strpos($class, $namespace) === 0)
			{
				$filePath = $directory . str_replace('\\', DIRECTORY_SEPARATOR, substr($class, strlen($namespace))) . '.php';
				$filename = $this->requireFile($filePath);

				if ($filename)
				{
					return $filename;
				}
			}
		}
	}

	// never found a mapped file
	return false;
}
```

</details>


<hr>

#### loadLegacy()

```php
protected function loadLegacy(string $class)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to load the class from common locations in previous
version of CodeIgniter, namely 'app/Libraries', and
'app/Models'.
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
<td><code>$class</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The class name. This typically should NOT have a namespace.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 27 lines (329 - 355)</small></summary>

```php
protected function loadLegacy(string $class)
{
	// If there is a namespace on this class, then
	// we cannot load it from traditional locations.
	if (strpos($class, '\\') !== false)
	{
		return false;
	}

	$paths = [
		APPPATH . 'Controllers/',
		APPPATH . 'Libraries/',
		APPPATH . 'Models/',
	];

	$class = str_replace('\\', DIRECTORY_SEPARATOR, $class) . '.php';

	foreach ($paths as $path)
	{
		if ($file = $this->requireFile($path . $class))
		{
			return $file;
		}
	}

	return false;
}
```

</details>


<hr>

#### requireFile()

```php
protected function requireFile(string $file)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A central way to require a file is loaded. Split out primarily
for testing purposes.
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
<td>string<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 13 lines (367 - 379)</small></summary>

```php
protected function requireFile(string $file)
{
	$file = $this->sanitizeFilename($file);

	if (is_file($file))
	{
		require_once $file;

		return $file;
	}

	return false;
}
```

</details>


<hr>

#### sanitizeFilename()

```php
public function sanitizeFilename(string $filename) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sanitizes a filename, replacing spaces with dashes.
</td></tr>
</table>

<table>
<tr><td>
Removes special characters that are illegal in filenames on certain
operating systems and special characters requiring special escaping
to manipulate at the command line. Replaces spaces and consecutive
dashes with a single dash. Trim period, dash and underscore from beginning
and end of filename.
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
<td><code>$filename</code></td>
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
<summary><small>Source: 14 lines (396 - 409)</small></summary>

```php
public function sanitizeFilename(string $filename): string
{
	// Only allow characters deemed safe for POSIX portable filenames.
	// Plus the forward slash for directory separators since this might
	// be a path.
	// http://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_278
	// Modified to allow backslash and colons for on Windows machines.
	$filename = preg_replace('/[^0-9\p{L}\s\/\-\_\.\:\\\\]/u', '', $filename);

	// Clean up our filename edges.
	$filename = trim($filename, '.-_');

	return $filename;
}
```

</details>


<hr>

#### discoverComposerNamespaces()

```php
protected function discoverComposerNamespaces()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Locates all PSR4 compatible namespaces from Composer.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 27 lines (416 - 442)</small></summary>

```php
protected function discoverComposerNamespaces()
{
	if (! is_file(COMPOSER_PATH))
	{
		return false;
	}

	$composer = include COMPOSER_PATH;

	$paths = $composer->getPrefixesPsr4();
	unset($composer);

	// Get rid of CodeIgniter so we don't have duplicates
	if (isset($paths['CodeIgniter\\']))
	{
		unset($paths['CodeIgniter\\']);
	}

	// Composer stores namespaces with trailing slash. We don't.
	$newPaths = [];
	foreach ($paths as $key => $value)
	{
		$newPaths[rtrim($key, '\\ ')] = $value;
	}

	$this->prefixes = array_merge($this->prefixes, $newPaths);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Autoloader/Autoloader.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/API/ResponseTrait.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/FileLocator.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:07**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>