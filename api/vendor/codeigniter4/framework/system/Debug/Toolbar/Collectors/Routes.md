


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Toolbar/Collectors/Routes.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Logs.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Timers.md">next</a></td>
</tr>
</table>







# CodeIgniter\Debug\Toolbar\Collectors 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Debug\Toolbar\Collectors</td></tr>
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
<td>framework/system/Debug/Toolbar/Collectors/Routes.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/BaseCollector.md">CodeIgniter\Debug\Toolbar\Collectors\BaseCollector</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Config.md">CodeIgniter\Debug\Toolbar\Collectors\Config</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Database.md">CodeIgniter\Debug\Toolbar\Collectors\Database</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Events.md">CodeIgniter\Debug\Toolbar\Collectors\Events</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Files.md">CodeIgniter\Debug\Toolbar\Collectors\Files</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/History.md">CodeIgniter\Debug\Toolbar\Collectors\History</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Logs.md">CodeIgniter\Debug\Toolbar\Collectors\Logs</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Routes.md">CodeIgniter\Debug\Toolbar\Collectors\Routes</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Timers.md">CodeIgniter\Debug\Toolbar\Collectors\Timers</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Views.md">CodeIgniter\Debug\Toolbar\Collectors\Views</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
</table>



 
## CodeIgniter\Debug\Toolbar\Collectors\Routes

<table style="text-align:left">
<tr><th>Class</th><td>Routes</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Debug\Toolbar\Collectors\Routes</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/BaseCollector.md">CodeIgniter\Debug\Toolbar\Collectors\BaseCollector</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Routes collector
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
<th><a href="#hasTimeline"><strong>hasTimeline</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this collector has data that can
be displayed in the Timeline.</td>
</tr>
<tr>
<th><a href="#hasTabContent"><strong>hasTabContent</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this collector needs to display
content in a tab or not.</td>
</tr>
<tr>
<th><a href="#title"><strong>title</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The &#039;title&#039; of this Collector.</td>
</tr>

<tr>
<th><a href="#display"><strong>display</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the data of this collector to be formatted in the toolbar</td>
</tr>
<tr>
<th><a href="#getBadgeValue"><strong>getBadgeValue</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a count of all the routes in the system.</td>
</tr>
<tr>
<th><a href="#icon"><strong>icon</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Display the icon.</td>
</tr>

</table>





### Properties


<hr>

#### $hasTimeline

```php
protected $hasTimeline = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether this collector has data that can
be displayed in the Timeline.
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

#### $hasTabContent

```php
protected $hasTabContent = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether this collector needs to display
content in a tab or not.
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

#### $title

```php
protected $title = 'Routes';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The 'title' of this Collector.
</td></tr>
</table>

<table>
<tr><td>
Used to name things in the toolbar HTML.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>string
</td>
</tr>
</table>







### Methods


<hr>

#### display()

```php
public function display() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the data of this collector to be formatted in the toolbar
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
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
<summary><small>Source: 93 lines (81 - 173)</small></summary>

```php
public function display(): array
{
	$rawRoutes = Services::routes(true);
	$router    = Services::router(null, null, true);

	/*
	 * Matched Route
	 */
	$route = $router->getMatchedRoute();

	// Get our parameters
	// Closure routes
	if (is_callable($router->controllerName()))
	{
		$method = new \ReflectionFunction($router->controllerName());
	}
	else
	{
		try
		{
			$method = new \ReflectionMethod($router->controllerName(), $router->methodName());
		}
		catch (\ReflectionException $e)
		{
			// If we're here, the method doesn't exist
			// and is likely calculated in _remap.
			$method = new \ReflectionMethod($router->controllerName(), '_remap');
		}
	}

	$rawParams = $method->getParameters();

	$params = [];
	foreach ($rawParams as $key => $param)
	{
		$params[] = [
			'name'  => $param->getName(),
			'value' => $router->params()[$key] ??
				'&lt;empty&gt;&nbsp| default: ' . var_export($param->isDefaultValueAvailable() ? $param->getDefaultValue() : null, true),
		];
	}

	$matchedRoute = [
		[
			'directory'  => $router->directory(),
			'controller' => $router->controllerName(),
			'method'     => $router->methodName(),
			'paramCount' => count($router->params()),
			'truePCount' => count($params),
			'params'     => $params ?? [],
		],
	];

	/*
	* Defined Routes
	*/
	$routes  = [];
	$methods = [
		'get',
		'head',
		'post',
		'patch',
		'put',
		'delete',
		'options',
		'trace',
		'connect',
		'cli',
	];

	foreach ($methods as $method)
	{
		$raw = $rawRoutes->getRoutes($method);

		foreach ($raw as $route => $handler)
		{
			// filter for strings, as callbacks aren't displayable
			if (is_string($handler))
			{
				$routes[] = [
					'method'  => strtoupper($method),
					'route'   => $route,
					'handler' => $handler,
				];
			}
		}
	}

	return [
		'matchedRoute' => $matchedRoute,
		'routes'       => $routes,
	];
}
```

</details>


<hr>

#### getBadgeValue()

```php
public function getBadgeValue() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a count of all the routes in the system.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (182 - 187)</small></summary>

```php
public function getBadgeValue(): int
{
	$rawRoutes = Services::routes(true);

	return count($rawRoutes->getRoutes());
}
```

</details>


<hr>

#### icon()

```php
public function icon() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Display the icon.
</td></tr>
</table>

<table>
<tr><td>
Icon from <a href="https://icons8.com">https://icons8.com</a> - 1em package
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (198 - 201)</small></summary>

```php
public function icon(): string
{
	return 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFDSURBVEhL7ZRNSsNQFIUjVXSiOFEcuQIHDpzpxC0IGYeE/BEInbWlCHEDLsSiuANdhKDjgm6ggtSJ+l25ldrmmTwIgtgDh/t37r1J+16cX0dRFMtpmu5pWAkrvYjjOB7AETzStBFW+inxu3KUJMmhludQpoflS1zXban4LYqiO224h6VLTHr8Z+z8EpIHFF9gG78nDVmW7UgTHKjsCyY98QP+pcq+g8Ku2s8G8X3f3/I8b038WZTp+bO38zxfFd+I6YY6sNUvFlSDk9CRhiAI1jX1I9Cfw7GG1UB8LAuwbU0ZwQnbRDeEN5qqBxZMLtE1ti9LtbREnMIuOXnyIf5rGIb7Wq8HmlZgwYBH7ORTcKH5E4mpjeGt9fBZcHE2GCQ3Vt7oTNPNg+FXLHnSsHkw/FR+Gg2bB8Ptzrst/v6C/wrH+QB+duli6MYJdQAAAABJRU5ErkJggg==';
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Toolbar/Collectors/Routes.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Logs.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Timers.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>