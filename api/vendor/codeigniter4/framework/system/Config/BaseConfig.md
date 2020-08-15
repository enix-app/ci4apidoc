


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Config/BaseConfig.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/AutoloadConfig.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseService.md">next</a></td>
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
<td>framework/system/Config/BaseConfig.php
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



 

 
## CodeIgniter\Config\BaseConfig

<table style="text-align:left">
<tr><th>Class</th><td>BaseConfig</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Config\BaseConfig</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class BaseConfig
</td></tr>
</table>

<table>
<tr><td>
Not intended to be used on its own, this class will attempt to
automatically populate the child class' properties with values
from the environment.

These can be set within the .env file.
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
<th><a href="#registrars"><strong>registrars</strong></a></th>
<td>prop</td>
<td>
public<br>static

</td>
<td>An optional array of classes that will act as Registrars
for rapidly setting config class properties.</td>
</tr>
<tr>
<th><a href="#didDiscovery"><strong>didDiscovery</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Has module discovery happened yet?</td>
</tr>
<tr>
<th><a href="#moduleConfig"><strong>moduleConfig</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>The modules configuration.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Will attempt to get environment variables with names
that match the properties of the child class.</td>
</tr>
<tr>
<th><a href="#initEnvValue"><strong>initEnvValue</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Initialization an environment-specific configuration setting</td>
</tr>
<tr>
<th><a href="#getEnvValue"><strong>getEnvValue</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Retrieve an environment-specific configuration setting</td>
</tr>
<tr>
<th><a href="#registerProperties"><strong>registerProperties</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Provides external libraries a simple way to register one or more
options into a config file.</td>
</tr>

</table>





### Properties


<hr>

#### $registrars

```php
public static $registrars = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
An optional array of classes that will act as Registrars
for rapidly setting config class properties.
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

#### $didDiscovery

```php
protected static $didDiscovery = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Has module discovery happened yet?
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

#### $moduleConfig

```php
protected static $moduleConfig;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The modules configuration.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Config\Modules
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Will attempt to get environment variables with names
that match the properties of the child class.
</td></tr>
</table>

<table>
<tr><td>
The "shortPrefix" is the lowercase-only config class name.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 36 lines (82 - 117)</small></summary>

```php
public function __construct()
{
	static::$moduleConfig = config('Modules');

	$properties  = array_keys(get_object_vars($this));
	$prefix      = get_class($this);
	$slashAt     = strrpos($prefix, '\\');
	$shortPrefix = strtolower(substr($prefix, $slashAt === false ? 0 : $slashAt + 1));

	foreach ($properties as $property)
	{
		$this->initEnvValue($this->$property, $property, $prefix, $shortPrefix);

		if ($shortPrefix === 'encryption' && $property === 'key')
		{
			// Handle hex2bin prefix
			if (strpos($this->$property, 'hex2bin:') === 0)
			{
				$this->$property = hex2bin(substr($this->$property, 8));
			}
			// Handle base64 prefix
			elseif (strpos($this->$property, 'base64:') === 0)
			{
				$this->$property = base64_decode(substr($this->$property, 7), true);
			}
		}
	}

	if (defined('ENVIRONMENT') && ENVIRONMENT !== 'testing')
	{
		// well, this won't happen during unit testing
		// @codeCoverageIgnoreStart
		$this->registerProperties();
		// @codeCoverageIgnoreEnd
	}
}
```

</details>


<hr>

#### initEnvValue()

```php
protected function initEnvValue(&$property, string $name, string $prefix, string $shortPrefix)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Initialization an environment-specific configuration setting
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
<td><code>$</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>&$property</td>
</tr>

<tr>
<td>2.</td>
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$prefix</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$shortPrefix</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 30 lines (131 - 160)</small></summary>

```php
protected function initEnvValue(&$property, string $name, string $prefix, string $shortPrefix)
{
	if (is_array($property))
	{
		foreach ($property as $key => $val)
		{
			$this->initEnvValue($property[$key], "{$name}.{$key}", $prefix, $shortPrefix);
		}
	}
	else
	{
		if (($value = $this->getEnvValue($name, $prefix, $shortPrefix)) !== false)
		{
			if (! is_null($value))
			{
				if ($value === 'false')
				{
					$value = false;
				}
				elseif ($value === 'true')
				{
					$value = true;
				}

				$property = is_bool($value) ? $value : trim($value, '\'"');
			}
		}
	}
	return $property;
}
```

</details>


<hr>

#### getEnvValue()

```php
protected function getEnvValue(string $property, string $prefix, string $shortPrefix)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve an environment-specific configuration setting
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
<td><code>$property</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$prefix</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$shortPrefix</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (173 - 190)</small></summary>

```php
protected function getEnvValue(string $property, string $prefix, string $shortPrefix)
{
	$shortPrefix = ltrim($shortPrefix, '\\');
	switch (true)
	{
		case array_key_exists("{$shortPrefix}.{$property}", $_ENV):
			return $_ENV["{$shortPrefix}.{$property}"];
		case array_key_exists("{$shortPrefix}.{$property}", $_SERVER):
			return $_SERVER["{$shortPrefix}.{$property}"];
		case array_key_exists("{$prefix}.{$property}", $_ENV):
			return $_ENV["{$prefix}.{$property}"];
		case array_key_exists("{$prefix}.{$property}", $_SERVER):
			return $_SERVER["{$prefix}.{$property}"];
		default:
			$value = getenv($property);
			return $value === false ? null : $value;
	}
}
```

</details>


<hr>

#### registerProperties()

```php
protected function registerProperties()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides external libraries a simple way to register one or more
options into a config file.
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
<summary><small>Source: 54 lines (200 - 253)</small></summary>

```php
protected function registerProperties()
{
	if (! static::$moduleConfig->shouldDiscover('registrars'))
	{
		return;
	}

	if (! static::$didDiscovery)
	{
		$locator         = \Config\Services::locator();
		$registrarsFiles = $locator->search('Config/Registrar.php');

		foreach ($registrarsFiles as $file)
		{
			$className            = $locator->getClassname($file);
			static::$registrars[] = new $className();
		}

		static::$didDiscovery = true;
	}

	$shortName = (new \ReflectionClass($this))->getShortName();

	// Check the registrar class for a method named after this class' shortName
	foreach (static::$registrars as $callable)
	{
		// ignore non-applicable registrars
		if (! method_exists($callable, $shortName))
		{
			// @codeCoverageIgnoreStart
			continue;
			// @codeCoverageIgnoreEnd
		}

		$properties = $callable::$shortName();

		if (! is_array($properties))
		{
			throw new \RuntimeException('Registrars must return an array of properties and their values.');
		}

		foreach ($properties as $property => $value)
		{
			if (isset($this->$property) && is_array($this->$property) && is_array($value))
			{
				$this->$property = array_merge($this->$property, $value);
			}
			else
			{
				$this->$property = $value;
			}
		}
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Config/BaseConfig.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/AutoloadConfig.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseService.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>