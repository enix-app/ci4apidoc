


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Config/Config.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseService.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md">next</a></td>
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
<td>framework/system/Config/Config.php
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



 

 
## CodeIgniter\Config\Config

<table style="text-align:left">
<tr><th>Class</th><td>Config</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Config\Config</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Config
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Config
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
<th><a href="#instances"><strong>instances</strong></a></th>
<td>prop</td>
<td>
private<br>static

</td>
<td>Cache for instance of any configurations that
have been requested as &quot;shared&quot; instance.</td>
</tr>

<tr>
<th><a href="#get"><strong>get</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Create new configuration instances or return
a shared instance</td>
</tr>
<tr>
<th><a href="#injectMock"><strong>injectMock</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Helper method for injecting mock instances while testing.</td>
</tr>
<tr>
<th><a href="#reset"><strong>reset</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Resets the instances array</td>
</tr>
<tr>
<th><a href="#createClass"><strong>createClass</strong>()</a></th>
<td>method</td>
<td>
private<br>static

</td>
<td>Find configuration class and create instance</td>
</tr>

</table>





### Properties


<hr>

#### $instances

```php
static private $instances = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cache for instance of any configurations that
have been requested as "shared" instance.
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

#### get()

```php
public static function get(string $name, bool $getShared = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create new configuration instances or return
a shared instance
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
<td>Configuration name</td>
</tr>

<tr>
<td>2.</td>
<td><code>$getShared</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Use shared instance</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 19 lines (68 - 86)</small></summary>

```php
public static function get(string $name, bool $getShared = true)
{
	$class = $name;
	if (($pos = strrpos($name, '\\')) !== false)
	{
		$class = substr($name, $pos + 1);
	}

	if (! $getShared)
	{
		return self::createClass($name);
	}

	if (! isset( self::$instances[$class] ))
	{
		self::$instances[$class] = self::createClass($name);
	}
	return self::$instances[$class];
}
```

</details>


<hr>

#### injectMock()

```php
public static function injectMock(string $class, $instance)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Helper method for injecting mock instances while testing.
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

<tr>
<td>2.</td>
<td><code>$instance</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (96 - 99)</small></summary>

```php
public static function injectMock(string $class, $instance)
{
	self::$instances[$class] = $instance;
}
```

</details>


<hr>

#### reset()

```php
public static function reset()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Resets the instances array
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (106 - 109)</small></summary>

```php
public static function reset()
{
	static::$instances = [];
}
```

</details>


<hr>

#### createClass()

```php
private static function createClass(string $name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Find configuration class and create instance
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
<td>Classname</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 39 lines (120 - 158)</small></summary>

```php
private static function createClass(string $name)
{
	if (class_exists($name))
	{
		return new $name();
	}

	$locator = Services::locator();
	$file    = $locator->locateFile($name, 'Config');

	if (empty($file))
	{
		// No file found - check if the class was namespaced
		if (strpos($name, '\\') !== false)
		{
			// Class was namespaced and locateFile couldn't find it
			return null;
		}

		// Check all namespaces
		$files = $locator->search('Config/' . $name);
		if (empty($files))
		{
			return null;
		}

		// Get the first match (prioritizes user and framework)
		$file = reset($files);
	}

	$name = $locator->getClassname($file);

	if (empty($name))
	{
		return null;
	}

	return new $name();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Config/Config.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseService.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>