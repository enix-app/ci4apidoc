


 



<table>
<tr>
<td style="width:100%"><em>framework/system/View/Cell.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md">next</a></td>
</tr>
</table>







# CodeIgniter\View 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\View</td></tr>
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
<td>framework/system/View/Cell.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Cell.md">CodeIgniter\View\Cell</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md">CodeIgniter\View\Exceptions\ViewException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Filters.md">CodeIgniter\View\Filters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Parser.md">CodeIgniter\View\Parser</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Plugins.md">CodeIgniter\View\Plugins</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">CodeIgniter\View\RendererInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Table.md">CodeIgniter\View\Table</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/View.md">CodeIgniter\View\View</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md"><strong>CodeIgniter\Cache\CacheInterface</strong></a>
</td>
<td>CacheInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md"><strong>CodeIgniter\View\Exceptions\ViewException</strong></a>
</td>
<td>ViewException</td>
</tr>
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
<tr>
<td>
<strong>ReflectionMethod</strong>
</td>
<td>ReflectionMethod</td>
</tr>
</table>



 
## CodeIgniter\View\Cell

<table style="text-align:left">
<tr><th>Class</th><td>Cell</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\View\Cell</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Cell
</td></tr>
</table>

<table>
<tr><td>
A simple class that can call any other class that can be loaded,
and echo out it's result. Intended for displaying small blocks of
content within views that can be managed by other libraries and
not require they are loaded within controller.

Used with the helper function, it's use will look like:

        viewCell('\Some\Class::method', 'limit=5 sort=asc', 60, 'cache-name');

Parameters are matched up with the callback method's arguments of the same name:

        class Class {
            function method($limit, $sort)
        }

Alternatively, the params will be passed into the callback method as a simple array
if matching params are not found.

        class Class {
            function method(array $params=null)
        }
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\View
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
<th><a href="#cache"><strong>cache</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Instance of the current Cache Instance</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Cell constructor.</td>
</tr>
<tr>
<th><a href="#render"><strong>render</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Render a cell, returning its body as a string.</td>
</tr>
<tr>
<th><a href="#prepareParams"><strong>prepareParams</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Parses the params attribute. If an array, returns untouched.</td>
</tr>
<tr>
<th><a href="#determineClass"><strong>determineClass</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Given the library string, attempts to determine the class and method
to call.</td>
</tr>

</table>





### Properties


<hr>

#### $cache

```php
protected $cache;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instance of the current Cache Instance
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CacheInterface
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(CacheInterface $cache)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cell constructor.
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
<td><code>$cache</code></td>
<td><em>\CodeIgniter\Cache\CacheInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (90 - 93)</small></summary>

```php
public function __construct(CacheInterface $cache)
{
	$this->cache = $cache;
}
```

</details>


<hr>

#### render()

```php
public function render(string $library, $params = null, int $ttl = 0, string $cacheName = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Render a cell, returning its body as a string.
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
<td><code>$library</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
<td><em>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$ttl</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$cacheName</code></td>
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
<summary><small>Source: 81 lines (108 - 188)</small></summary>

```php
public function render(string $library, $params = null, int $ttl = 0, string $cacheName = null): string
{
	list($class, $method) = $this->determineClass($library);

	// Is it cached?
	$cacheName = ! empty($cacheName)
		? $cacheName
		: str_replace(['\\', '/'], '', $class) . $method . md5(serialize($params));

	if (! empty($this->cache) && $output = $this->cache->get($cacheName))
	{
		return $output;
	}

	// Not cached - so grab it...
	$instance = new $class();

	if (method_exists($instance, 'initController'))
	{
		$instance->initController(Services::request(), Services::response(), Services::logger());
	}

	if (! method_exists($instance, $method))
	{
		throw ViewException::forInvalidCellMethod($class, $method);
	}

	// Try to match up the parameter list we were provided
	// with the parameter name in the callback method.
	$paramArray = $this->prepareParams($params);
	$refMethod  = new ReflectionMethod($instance, $method);
	$paramCount = $refMethod->getNumberOfParameters();
	$refParams  = $refMethod->getParameters();

	if ($paramCount === 0)
	{
		if (! empty($paramArray))
		{
			throw ViewException::forMissingCellParameters($class, $method);
		}

		$output = $instance->{$method}();
	}
	elseif (($paramCount === 1) && (
			( ! array_key_exists($refParams[0]->name, $paramArray)) ||
			(array_key_exists($refParams[0]->name, $paramArray) && count($paramArray) !== 1) )
	)
	{
		$output = $instance->{$method}($paramArray);
	}
	else
	{
		$fireArgs      = [];
		$method_params = [];

		foreach ($refParams as $arg)
		{
			$method_params[$arg->name] = true;
			if (array_key_exists($arg->name, $paramArray))
			{
				$fireArgs[$arg->name] = $paramArray[$arg->name];
			}
		}

		foreach ($paramArray as $key => $val)
		{
			if (! isset($method_params[$key]))
			{
				throw ViewException::forInvalidCellParameter($key);
			}
		}

		$output = $instance->$method(...array_values($fireArgs));
	}
	// Can we cache it?
	if (! empty($this->cache) && $ttl !== 0)
	{
		$this->cache->save($cacheName, $output, $ttl);
	}
	return $output;
}
```

</details>


<hr>

#### prepareParams()

```php
public function prepareParams($params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses the params attribute. If an array, returns untouched.
</td></tr>
</table>

<table>
<tr><td>
If a string, it should be in the format "key1=value key2=value".
It will be split and returned as an array.
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
<td><code>$params</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
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
<summary><small>Source: 41 lines (201 - 241)</small></summary>

```php
public function prepareParams($params)
{
	if (empty($params) || ( ! is_string($params) && ! is_array($params)))
	{
		return [];
	}

	if (is_string($params))
	{
		$new_params = [];
		$separator  = ' ';

		if (strpos($params, ',') !== false)
		{
			$separator = ',';
		}

		$params = explode($separator, $params);
		unset($separator);

		foreach ($params as $p)
		{
			if (! empty($p))
			{
				list($key, $val)        = explode('=', $p);
				$new_params[trim($key)] = trim($val, ', ');
			}
		}

		$params = $new_params;

		unset($new_params);
	}

	if (is_array($params) && empty($params))
	{
		return [];
	}

	return $params;
}
```

</details>


<hr>

#### determineClass()

```php
protected function determineClass(string $library) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Given the library string, attempts to determine the class and method
to call.
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
<td><code>$library</code></td>
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
<summary><small>Source: 28 lines (253 - 280)</small></summary>

```php
protected function determineClass(string $library): array
{
	// We don't want to actually call static methods
	// by default, so convert any double colons.
	$library = str_replace('::', ':', $library);

	list($class, $method) = explode(':', $library);

	if (empty($class))
	{
		throw ViewException::forNoCellClass();
	}

	if (! class_exists($class, true))
	{
		throw ViewException::forInvalidCellClass($class);
	}

	if (empty($method))
	{
		$method = 'index';
	}

	return [
		$class,
		$method,
	];
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/View/Cell.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>