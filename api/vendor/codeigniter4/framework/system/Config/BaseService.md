


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Config/BaseService.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Config.md">next</a></td>
</tr>
</table>







# CodeIgniter\Config 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Config</td></tr>
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
<td>framework/system/Config/BaseService.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/AutoloadConfig.md">CodeIgniter\Config\AutoloadConfig</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">CodeIgniter\Config\BaseConfig</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseService.md">CodeIgniter\Config\BaseService</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Config.md">CodeIgniter\Config\Config</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md">CodeIgniter\Config\DotEnv</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/ForeignCharacters.md">CodeIgniter\Config\ForeignCharacters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Services.md">CodeIgniter\Config\Services</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/View.md">CodeIgniter\Config\View</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/Autoloader.md"><strong>CodeIgniter\Autoloader\Autoloader</strong></a>
</td>
<td>Autoloader</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/FileLocator.md"><strong>CodeIgniter\Autoloader\FileLocator</strong></a>
</td>
<td>FileLocator</td>
</tr>
<tr>
<td>
<strong>Config\Autoload</strong>
</td>
<td>Autoload</td>
</tr>
<tr>
<td>
<strong>Config\Modules</strong>
</td>
<td>Modules</td>
</tr>
</table>



 
## CodeIgniter\Config\BaseService

<table style="text-align:left">
<tr><th>Class</th><td>BaseService</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Config\BaseService</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Services Configuration file.
</td></tr>
</table>

<table>
<tr><td>
Services are simply other classes/libraries that the system uses
to do its job. This is used by CodeIgniter to allow the core of the
framework to be swapped out easily without affecting the usage within
the rest of your application.

This is used in place of a Dependency Injection container primarily
due to its simplicity, which allows a better long-term maintenance
of the applications built on top of CodeIgniter. A bonus side-effect
is that IDEs are able to determine what class you are calling
whereas with DI Containers there usually isn't a way for them to do this.
</td></tr>
</table>

</details>



<table style="text-align:left">
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
<th><a href="#instances"><strong>instances</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Cache for instance of any services that
have been requested as a &quot;shared&quot; instance.</td>
</tr>
<tr>
<th><a href="#mocks"><strong>mocks</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Mock objects for testing which are returned if exist.</td>
</tr>
<tr>
<th><a href="#discovered"><strong>discovered</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Have we already discovered other Services?</td>
</tr>
<tr>
<th><a href="#services"><strong>services</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>A cache of other service classes we&#039;ve found.</td>
</tr>

<tr>
<th><a href="#getSharedInstance"><strong>getSharedInstance</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Returns a shared instance of any of the class&#039; services.</td>
</tr>
<tr>
<th><a href="#autoloader"><strong>autoloader</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>The Autoloader class is the central class that handles our
spl_autoload_register method, and helper methods.</td>
</tr>
<tr>
<th><a href="#locator"><strong>locator</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>The file locator provides utility methods for looking for non-classes
within namespaced folders, as well as convenience methods for
loading &#039;helpers&#039;, and &#039;libraries&#039;.</td>
</tr>
<tr>
<th><a href="#__callStatic"><strong>__callStatic</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Provides the ability to perform case-insensitive calling of service
names.</td>
</tr>
<tr>
<th><a href="#reset"><strong>reset</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Reset shared instances and mocks for testing.</td>
</tr>
<tr>
<th><a href="#injectMock"><strong>injectMock</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Inject mock object for testing.</td>
</tr>
<tr>
<th><a href="#discoverServices"><strong>discoverServices</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Will scan all psr4 namespaces registered with system to look
for new Config\Services files. Caches a copy of each one, then
looks for the service method in each, returning an instance of
the service, if available.</td>
</tr>

</table>





### Properties


<hr>

#### $instances

```php
static protected $instances = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cache for instance of any services that
have been requested as a "shared" instance.
</td></tr>
</table>

<table>
<tr><td>
Keys should be lowercase service names.
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

#### $mocks

```php
static protected $mocks = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Mock objects for testing which are returned if exist.
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

#### $discovered

```php
static protected $discovered = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Have we already discovered other Services?
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>bool
</td>
</tr>
</table>


<hr>

#### $services

```php
static protected $services = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A cache of other service classes we've found.
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

#### getSharedInstance()

```php
protected static function getSharedInstance(string $key, ...$params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a shared instance of any of the class' services.
</td></tr>
</table>

<table>
<tr><td>
$key must be a name matching a service.
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
<td><code>$key</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
<td><em>array
</em></td>
<td>true</td>
<td></td>
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
<summary><small>Source: 20 lines (108 - 127)</small></summary>

```php
protected static function getSharedInstance(string $key, ...$params)
{
	$key = strtolower($key);

	// Returns mock if exists
	if (isset(static::$mocks[$key]))
	{
		return static::$mocks[$key];
	}

	if (! isset(static::$instances[$key]))
	{
		// Make sure $getShared is false
		array_push($params, false);

		static::$instances[$key] = static::$key(...$params);
	}

	return static::$instances[$key];
}
```

</details>


<hr>

#### autoloader()

```php
public static function autoloader(bool $getShared = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Autoloader class is the central class that handles our
spl_autoload_register method, and helper methods.
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
<td><code>$getShared</code></td>
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
<td>\CodeIgniter\Autoloader\Autoloader
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (139 - 152)</small></summary>

```php
public static function autoloader(bool $getShared = true)
{
	if ($getShared)
	{
		if (empty(static::$instances['autoloader']))
		{
			static::$instances['autoloader'] = new Autoloader();
		}

		return static::$instances['autoloader'];
	}

	return new Autoloader();
}
```

</details>


<hr>

#### locator()

```php
public static function locator(bool $getShared = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The file locator provides utility methods for looking for non-classes
within namespaced folders, as well as convenience methods for
loading 'helpers', and 'libraries'.
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
<td><code>$getShared</code></td>
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
<td>\CodeIgniter\Autoloader\FileLocator
</td>
</tr>
</table>





<details>
<summary><small>Source: 16 lines (165 - 180)</small></summary>

```php
public static function locator(bool $getShared = true)
{
	if ($getShared)
	{
		if (empty(static::$instances['locator']))
		{
			static::$instances['locator'] = new FileLocator(
				static::autoloader()
			);
		}

		return static::$instances['locator'];
	}

	return new FileLocator(static::autoloader());
}
```

</details>


<hr>

#### __callStatic()

```php
public static function __callStatic(string $name, array $arguments)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides the ability to perform case-insensitive calling of service
names.
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
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$arguments</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
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
<summary><small>Source: 11 lines (193 - 203)</small></summary>

```php
public static function __callStatic(string $name, array $arguments)
{
	$name = strtolower($name);

	if (method_exists(Services::class, $name))
	{
		return Services::$name(...$arguments);
	}

	return static::discoverServices($name, $arguments);
}
```

</details>


<hr>

#### reset()

```php
public static function reset(bool $init_autoloader = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reset shared instances and mocks for testing.
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
<td><code>$init_autoloader</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Initializes autoloader instance</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 11 lines (212 - 222)</small></summary>

```php
public static function reset(bool $init_autoloader = false)
{
	static::$mocks = [];

	static::$instances = [];

	if ($init_autoloader)
	{
		static::autoloader()->initialize(new Autoload(), new Modules());
	}
}
```

</details>


<hr>

#### injectMock()

```php
public static function injectMock(string $name, $mock)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Inject mock object for testing.
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
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$mock</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 5 lines (232 - 236)</small></summary>

```php
public static function injectMock(string $name, $mock)
{
	$name                 = strtolower($name);
	static::$mocks[$name] = $mock;
}
```

</details>


<hr>

#### discoverServices()

```php
protected static function discoverServices(string $name, array $arguments)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Will scan all psr4 namespaces registered with system to look
for new Config\Services files. Caches a copy of each one, then
looks for the service method in each, returning an instance of
the service, if available.
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
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$arguments</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
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
<summary><small>Source: 49 lines (251 - 299)</small></summary>

```php
protected static function discoverServices(string $name, array $arguments)
{
	if (! static::$discovered)
	{
		$config = config('Modules');

		if ($config->shouldDiscover('services'))
		{
			$locator = static::locator();
			$files   = $locator->search('Config/Services');

			if (empty($files))
			{
				// no files at all found - this would be really, really bad
				return null;
			}

			// Get instances of all service classes and cache them locally.
			foreach ($files as $file)
			{
				$classname = $locator->getClassname($file);

				if (! in_array($classname, ['CodeIgniter\\Config\\Services']))
				{
					static::$services[] = new $classname();
				}
			}
		}

		static::$discovered = true;
	}

	if (! static::$services)
	{
		// we found stuff, but no services - this would be really bad
		return null;
	}

	// Try to find the desired service method
	foreach (static::$services as $class)
	{
		if (method_exists(get_class($class), $name))
		{
			return $class::$name(...$arguments);
		}
	}

	return null;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Config/BaseService.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Config.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>