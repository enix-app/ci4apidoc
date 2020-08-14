


 



<table>
<tr>
<td style="width:100%"><em>framework/system/ComposerScripts.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Commands/Utilities/Routes.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Config/AutoloadConfig.md">next</a></td>
</tr>
</table>







# CodeIgniter 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter</td></tr>
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
<td>framework/system/ComposerScripts.php
</td>
</tr>
</table>

 


 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>ReflectionClass</strong>
</td>
<td>ReflectionClass</td>
</tr>
</table>



 
## CodeIgniter\ComposerScripts

<table style="text-align:left">
<tr><th>Class</th><td>ComposerScripts</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\ComposerScripts</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
ComposerScripts
</td></tr>
</table>

<table>
<tr><td>
These scripts are used by Composer during installs and updates
to move files to locations within the system folder so that end-users
do not need to use Composer to install a package, but can simply
download
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
</td>
</tr>
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
<th><a href="#basePath"><strong>basePath</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Base path to use.</td>
</tr>

<tr>
<th><a href="#postUpdate"><strong>postUpdate</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>After composer install/update, this is called to move
the bare-minimum required files for our dependencies
to appropriate locations.</td>
</tr>
<tr>
<th><a href="#moveFile"><strong>moveFile</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Move a file.</td>
</tr>
<tr>
<th><a href="#getClassFilePath"><strong>getClassFilePath</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Determine file path of a class.</td>
</tr>
<tr>
<th><a href="#removeDir"><strong>removeDir</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>A recursive remove directory method.</td>
</tr>
<tr>
<th><a href="#copyDir"><strong>copyDir</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#moveEscaper"><strong>moveEscaper</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Moves the Laminas Escaper files into our base repo so that it&#039;s
available for packaged releases where the users don&#039;t user Composer.</td>
</tr>
<tr>
<th><a href="#moveKint"><strong>moveKint</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Moves the Kint file into our base repo so that it&#039;s
available for packaged releases where the users don&#039;t user Composer.</td>
</tr>

</table>





### Properties


<hr>

#### $basePath

```php
protected static $basePath = 'ThirdParty/';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Base path to use.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\type
</td>
</tr>
</table>







### Methods


<hr>

#### postUpdate()

```php
public static function postUpdate()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
After composer install/update, this is called to move
the bare-minimum required files for our dependencies
to appropriate locations.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>







<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 5 lines (71 - 75)</small></summary>

```php
public static function postUpdate()
{
	static::moveEscaper();
	static::moveKint();
}
```

</details>


<hr>

#### moveFile()

```php
protected static function moveFile(string $source, string $destination) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Move a file.
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
<td><code>$source</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$destination</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (87 - 104)</small></summary>

```php
protected static function moveFile(string $source, string $destination): bool
{
	$source = realpath($source);

	if (empty($source))
	{
		// @codeCoverageIgnoreStart
		die('Cannot move file. Source path invalid.');
		// @codeCoverageIgnoreEnd
	}

	if (! is_file($source))
	{
		return false;
	}

	return copy($source, $destination);
}
```

</details>


<hr>

#### getClassFilePath()

```php
protected static function getClassFilePath(string $class)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determine file path of a class.
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 6 lines (116 - 121)</small></summary>

```php
protected static function getClassFilePath(string $class)
{
	$reflector = new ReflectionClass($class);

	return $reflector->getFileName();
}
```

</details>


<hr>

#### removeDir()

```php
protected static function removeDir($dir)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A recursive remove directory method.
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
<td><code>$dir</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 23 lines (130 - 152)</small></summary>

```php
protected static function removeDir($dir)
{
	if (is_dir($dir))
	{
		$objects = scandir($dir);
		foreach ($objects as $object)
		{
			if ($object !== '.' && $object !== '..')
			{
				if (filetype($dir . '/' . $object) === 'dir')
				{
					static::removeDir($dir . '/' . $object);
				}
				else
				{
					unlink($dir . '/' . $object);
				}
			}
		}
		reset($objects);
		rmdir($dir);
	}
}
```

</details>


<hr>

#### copyDir()

```php
protected static function copyDir($source, $dest)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td><code>$source</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$dest</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 22 lines (154 - 175)</small></summary>

```php
protected static function copyDir($source, $dest)
{
	$dir = opendir($source);
	@mkdir($dest);

	while (false !== ( $file = readdir($dir)))
	{
		if (( $file !== '.' ) && ( $file !== '..' ))
		{
			if (is_dir($source . '/' . $file))
			{
				static::copyDir($source . '/' . $file, $dest . '/' . $file);
			}
			else
			{
				copy($source . '/' . $file, $dest . '/' . $file);
			}
		}
	}

	closedir($dir);
}
```

</details>


<hr>

#### moveEscaper()

```php
public static function moveEscaper()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Moves the Laminas Escaper files into our base repo so that it's
available for packaged releases where the users don't user Composer.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>







<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 32 lines (183 - 214)</small></summary>

```php
public static function moveEscaper()
{
	if (class_exists('\\Laminas\\Escaper\\Escaper') && is_file(static::getClassFilePath('\\Laminas\\Escaper\\Escaper')))
	{
		$base = basename(__DIR__) . '/' . static::$basePath . 'Escaper';

		foreach ([$base, $base . '/Exception'] as $path)
		{
			if (! is_dir($path))
			{
				mkdir($path, 0755);
			}
		}

		$files = [
			static::getClassFilePath('\\Laminas\\Escaper\\Exception\\ExceptionInterface')       => $base . '/Exception/ExceptionInterface.php',
			static::getClassFilePath('\\Laminas\\Escaper\\Exception\\InvalidArgumentException') => $base . '/Exception/InvalidArgumentException.php',
			static::getClassFilePath('\\Laminas\\Escaper\\Exception\\RuntimeException')         => $base . '/Exception/RuntimeException.php',
			static::getClassFilePath('\\Laminas\\Escaper\\Escaper')                             => $base . '/Escaper.php',
		];

		foreach ($files as $source => $dest)
		{
			if (! static::moveFile($source, $dest))
			{
				// @codeCoverageIgnoreStart
				die('Error moving: ' . $source);
				// @codeCoverageIgnoreEnd
			}
		}
	}
}
```

</details>


<hr>

#### moveKint()

```php
public static function moveKint()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Moves the Kint file into our base repo so that it's
available for packaged releases where the users don't user Composer.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 26 lines (222 - 247)</small></summary>

```php
public static function moveKint()
{
	$dir = 'vendor/kint-php/kint/src';

	if (is_dir($dir))
	{
		$base = basename(__DIR__) . '/' . static::$basePath . 'Kint';

		// Remove the contents of the previous Kint folder, if any.
		if (is_dir($base))
		{
			static::removeDir($base);
		}

		// Create Kint if it doesn't exist already
		if (! is_dir($base))
		{
			mkdir($base, 0755);
		}

		static::copyDir($dir, $base);
		static::copyDir($dir . '/../resources', $base . '/resources');
		copy($dir . '/../init.php', $base . '/init.php');
		copy($dir . '/../init_helpers.php', $base . '/init_helpers.php');
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/ComposerScripts.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Commands/Utilities/Routes.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Config/AutoloadConfig.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>