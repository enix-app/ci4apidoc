


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Router/Router.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollectionInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouterInterface.md">next</a></td>
</tr>
</table>







# CodeIgniter\Router 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Router</td></tr>
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
<td>framework/system/Router/Router.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RedirectException.md">CodeIgniter\Router\Exceptions\RedirectException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RouterException.md">CodeIgniter\Router\Exceptions\RouterException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollection.md">CodeIgniter\Router\RouteCollection</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollectionInterface.md">CodeIgniter\Router\RouteCollectionInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Router.md">CodeIgniter\Router\Router</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouterInterface.md">CodeIgniter\Router\RouterInterface</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/PageNotFoundException.md"><strong>CodeIgniter\Exceptions\PageNotFoundException</strong></a>
</td>
<td>PageNotFoundException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Request.md"><strong>CodeIgniter\HTTP\Request</strong></a>
</td>
<td>Request</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RedirectException.md"><strong>CodeIgniter\Router\Exceptions\RedirectException</strong></a>
</td>
<td>RedirectException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RouterException.md"><strong>CodeIgniter\Router\Exceptions\RouterException</strong></a>
</td>
<td>RouterException</td>
</tr>
</table>



 
## CodeIgniter\Router\Router

<table style="text-align:left">
<tr><th>Class</th><td>Router</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Router\Router</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouterInterface.md">CodeIgniter\Router\RouterInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Request router.
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
<th><a href="#collection"><strong>collection</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>A RouteCollection instance.</td>
</tr>
<tr>
<th><a href="#directory"><strong>directory</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Sub-directory that contains the requested controller class.</td>
</tr>
<tr>
<th><a href="#controller"><strong>controller</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the controller class.</td>
</tr>
<tr>
<th><a href="#method"><strong>method</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the method to use.</td>
</tr>
<tr>
<th><a href="#params"><strong>params</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>An array of binds that were collected
so they can be sent to closure routes.</td>
</tr>
<tr>
<th><a href="#indexPage"><strong>indexPage</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the front controller.</td>
</tr>
<tr>
<th><a href="#translateURIDashes"><strong>translateURIDashes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether dashes in URI&#039;s should be converted
to underscores when determining method names.</td>
</tr>
<tr>
<th><a href="#matchedRoute"><strong>matchedRoute</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The route that was matched for this request.</td>
</tr>
<tr>
<th><a href="#matchedRouteOptions"><strong>matchedRouteOptions</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The options set for the matched route.</td>
</tr>
<tr>
<th><a href="#detectedLocale"><strong>detectedLocale</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The locale that was detected in a route.</td>
</tr>
<tr>
<th><a href="#filterInfo"><strong>filterInfo</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The filter info from Route Collection
if the matched route should be filtered.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Stores a reference to the RouteCollection object.</td>
</tr>
<tr>
<th><a href="#handle"><strong>handle</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#getFilter"><strong>getFilter</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the filter info for the matched route, if any.</td>
</tr>
<tr>
<th><a href="#controllerName"><strong>controllerName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the name of the matched controller.</td>
</tr>
<tr>
<th><a href="#methodName"><strong>methodName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the name of the method to run in the
chosen container.</td>
</tr>
<tr>
<th><a href="#get404Override"><strong>get404Override</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the 404 Override settings from the Collection.</td>
</tr>
<tr>
<th><a href="#params"><strong>params</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the binds that have been matched and collected
during the parsing process as an array, ready to send to
instance-&gt;method(...$params).</td>
</tr>
<tr>
<th><a href="#directory"><strong>directory</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the name of the sub-directory the controller is in,
if any. Relative to APPPATH.&#039;Controllers&#039;.</td>
</tr>
<tr>
<th><a href="#getMatchedRoute"><strong>getMatchedRoute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the routing information that was matched for this
request, if a route was defined.</td>
</tr>
<tr>
<th><a href="#getMatchedRouteOptions"><strong>getMatchedRouteOptions</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns all options set for the matched route</td>
</tr>
<tr>
<th><a href="#setIndexPage"><strong>setIndexPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the value that should be used to match the index.php file. Defaults
to index.php but this allows you to modify it in case your are using
something like mod_rewrite to remove the page. This allows you to set
it a blank.</td>
</tr>
<tr>
<th><a href="#setTranslateURIDashes"><strong>setTranslateURIDashes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Tells the system whether we should translate URI dashes or not
in the URI from a dash to an underscore.</td>
</tr>
<tr>
<th><a href="#hasLocale"><strong>hasLocale</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns true/false based on whether the current route contained
a {locale} placeholder.</td>
</tr>
<tr>
<th><a href="#getLocale"><strong>getLocale</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the detected locale, if any, or null.</td>
</tr>
<tr>
<th><a href="#checkRoutes"><strong>checkRoutes</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Compares the uri string against the routes that the
RouteCollection class defined for us, attempting to find a match.</td>
</tr>
<tr>
<th><a href="#autoRoute"><strong>autoRoute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attempts to match a URI path against Controllers and directories
found in APPPATH/Controllers, to find a matching route.</td>
</tr>
<tr>
<th><a href="#validateRequest"><strong>validateRequest</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Attempts to validate the URI request and determine the controller path.</td>
</tr>
<tr>
<th><a href="#setDirectory"><strong>setDirectory</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the sub-directory that the controller is in.</td>
</tr>
<tr>
<th><a href="#setRequest"><strong>setRequest</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Set request route</td>
</tr>
<tr>
<th><a href="#setDefaultController"><strong>setDefaultController</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Sets the default controller based on the info set in the RouteCollection.</td>
</tr>

</table>





### Properties


<hr>

#### $collection

```php
protected $collection;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A RouteCollection instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\RouteCollection
</td>
</tr>
</table>


<hr>

#### $directory

```php
protected $directory;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sub-directory that contains the requested controller class.
</td></tr>
</table>

<table>
<tr><td>
Primarily used by 'autoRoute'.
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


<hr>

#### $controller

```php
protected $controller;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the controller class.
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


<hr>

#### $method

```php
protected $method;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the method to use.
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


<hr>

#### $params

```php
protected $params = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
An array of binds that were collected
so they can be sent to closure routes.
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

#### $indexPage

```php
protected $indexPage = 'index.php';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the front controller.
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


<hr>

#### $translateURIDashes

```php
protected $translateURIDashes = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether dashes in URI's should be converted
to underscores when determining method names.
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

#### $matchedRoute

```php
protected $matchedRoute;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The route that was matched for this request.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array<br>null
</td>
</tr>
</table>


<hr>

#### $matchedRouteOptions

```php
protected $matchedRouteOptions;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The options set for the matched route.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array<br>null
</td>
</tr>
</table>


<hr>

#### $detectedLocale

```php
protected $detectedLocale;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The locale that was detected in a route.
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


<hr>

#### $filterInfo

```php
protected $filterInfo;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The filter info from Route Collection
if the matched route should be filtered.
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

#### __construct()

```php
public function __construct(RouteCollectionInterface $routes, Request $request = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores a reference to the RouteCollection object.
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
<td><code>$routes</code></td>
<td><em>\RouteCollectionInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$request</code></td>
<td><em>\Request
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (142 - 150)</small></summary>

```php
public function __construct(RouteCollectionInterface $routes, Request $request = null)
{
	$this->collection = $routes;

	$this->controller = $this->collection->getDefaultController();
	$this->method     = $this->collection->getDefaultMethod();

	$this->collection->setHTTPVerb($request->getMethod() ?? strtolower($_SERVER['REQUEST_METHOD']));
}
```

</details>


<hr>

#### handle()

```php
public function handle(string $uri = null)
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
<td><code>$uri</code></td>
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
<td>mixed<br>string
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Router\Exceptions\RedirectException
</td>
</tr>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Exceptions\PageNotFoundException
</td>
</tr>
</table>



<details>
<summary><small>Source: 38 lines (161 - 198)</small></summary>

```php
public function handle(string $uri = null)
{
	$this->translateURIDashes = $this->collection->shouldTranslateURIDashes();

	// If we cannot find a URI to match against, then
	// everything runs off of it's default settings.
	if ($uri === null || $uri === '')
	{
		return strpos($this->controller, '\\') === false
			? $this->collection->getDefaultNamespace() . $this->controller
			: $this->controller;
	}

	// Decode URL-encoded string
	$uri = urldecode($uri);

	if ($this->checkRoutes($uri))
	{
		if ($this->collection->isFiltered($this->matchedRoute[0]))
		{
			$this->filterInfo = $this->collection->getFilterForRoute($this->matchedRoute[0]);
		}

		return $this->controller;
	}

	// Still here? Then we can try to match the URI against
	// Controllers/directories, but the application may not
	// want this, like in the case of API's.
	if (! $this->collection->shouldAutoRoute())
	{
		throw new PageNotFoundException("Can't find a route for '{$uri}'.");
	}

	$this->autoRoute($uri);

	return $this->controllerName();
}
```

</details>


<hr>

#### getFilter()

```php
public function getFilter()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the filter info for the matched route, if any.
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
<summary><small>Source: 4 lines (207 - 210)</small></summary>

```php
public function getFilter()
{
	return $this->filterInfo;
}
```

</details>


<hr>

#### controllerName()

```php
public function controllerName()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the name of the matched controller.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (219 - 224)</small></summary>

```php
public function controllerName()
{
	return $this->translateURIDashes
		? str_replace('-', '_', $this->controller)
		: $this->controller;
}
```

</details>


<hr>

#### methodName()

```php
public function methodName() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the name of the method to run in the
chosen container.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (234 - 239)</small></summary>

```php
public function methodName(): string
{
	return $this->translateURIDashes
		? str_replace('-', '_', $this->method)
		: $this->method;
}
```

</details>


<hr>

#### get404Override()

```php
public function get404Override()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the 404 Override settings from the Collection.
</td></tr>
</table>

<table>
<tr><td>
If the override is a string, will split to controller/index array.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 21 lines (247 - 267)</small></summary>

```php
public function get404Override()
{
	$route = $this->collection->get404Override();

	if (is_string($route))
	{
		$routeArray = explode('::', $route);

		return [
			$routeArray[0], // Controller
			$routeArray[1] ?? 'index',   // Method
		];
	}

	if (is_callable($route))
	{
		return $route;
	}

	return null;
}
```

</details>


<hr>

#### params()

```php
public function params() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the binds that have been matched and collected
during the parsing process as an array, ready to send to
instance->method(...$params).
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (278 - 281)</small></summary>

```php
public function params(): array
{
	return $this->params;
}
```

</details>


<hr>

#### directory()

```php
public function directory() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the name of the sub-directory the controller is in,
if any. Relative to APPPATH.'Controllers'.
</td></tr>
</table>

<table>
<tr><td>
Only used when auto-routing is turned on.
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
<summary><small>Source: 4 lines (293 - 296)</small></summary>

```php
public function directory(): string
{
	return ! empty($this->directory) ? $this->directory : '';
}
```

</details>


<hr>

#### getMatchedRoute()

```php
public function getMatchedRoute()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the routing information that was matched for this
request, if a route was defined.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (306 - 309)</small></summary>

```php
public function getMatchedRoute()
{
	return $this->matchedRoute;
}
```

</details>


<hr>

#### getMatchedRouteOptions()

```php
public function getMatchedRouteOptions()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns all options set for the matched route
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (318 - 321)</small></summary>

```php
public function getMatchedRouteOptions()
{
	return $this->matchedRouteOptions;
}
```

</details>


<hr>

#### setIndexPage()

```php
public function setIndexPage($page) : self
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the value that should be used to match the index.php file. Defaults
to index.php but this allows you to modify it in case your are using
something like mod_rewrite to remove the page. This allows you to set
it a blank.
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
<td><code>$page</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (335 - 340)</small></summary>

```php
public function setIndexPage($page): self
{
	$this->indexPage = $page;

	return $this;
}
```

</details>


<hr>

#### setTranslateURIDashes()

```php
public function setTranslateURIDashes(bool $val = false) : self
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Tells the system whether we should translate URI dashes or not
in the URI from a dash to an underscore.
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
<td><code>$val</code></td>
<td><em>bool<br>false
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
<summary><small>Source: 6 lines (352 - 357)</small></summary>

```php
public function setTranslateURIDashes(bool $val = false): self
{
	$this->translateURIDashes = $val;

	return $this;
}
```

</details>


<hr>

#### hasLocale()

```php
public function hasLocale()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns true/false based on whether the current route contained
a {locale} placeholder.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (367 - 370)</small></summary>

```php
public function hasLocale()
{
	return (bool) $this->detectedLocale;
}
```

</details>


<hr>

#### getLocale()

```php
public function getLocale()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the detected locale, if any, or null.
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
<summary><small>Source: 4 lines (379 - 382)</small></summary>

```php
public function getLocale()
{
	return $this->detectedLocale;
}
```

</details>


<hr>

#### checkRoutes()

```php
protected function checkRoutes(string $uri) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Compares the uri string against the routes that the
RouteCollection class defined for us, attempting to find a match.
</td></tr>
</table>

<table>
<tr><td>
This method will modify $this->controller, etal as needed.
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
<td><code>$uri</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The URI path to compare against the routes</td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Router\Exceptions\RedirectException
</td>
</tr>
</table>



<details>
<summary><small>Source: 117 lines (396 - 512)</small></summary>

```php
protected function checkRoutes(string $uri): bool
{
	$routes = $this->collection->getRoutes($this->collection->getHTTPVerb());

	// Don't waste any time
	if (empty($routes))
	{
		return false;
	}

	$uri = $uri === '/'
		? $uri
		: ltrim($uri, '/ ');

	// Loop through the route array looking for wildcards
	foreach ($routes as $key => $val)
	{
		// Reset localeSegment
		$localeSegment = null;

		$key = $key === '/'
			? $key
			: ltrim($key, '/ ');

		$matchedKey = $key;

		// Are we dealing with a locale?
		if (strpos($key, '{locale}') !== false)
		{
			$localeSegment = array_search('{locale}', preg_split('/[\/]*((^[a-zA-Z0-9])|\(([^()]*)\))*[\/]+/m', $key));

			// Replace it with a regex so it
			// will actually match.
			$key = str_replace('/', '\/', $key);
			$key = str_replace('{locale}', '[^\/]+', $key);
		}

		// Does the RegEx match?
		if (preg_match('#^' . $key . '$#u', $uri, $matches))
		{
			// Is this route supposed to redirect to another?
			if ($this->collection->isRedirect($key))
			{
				throw new RedirectException(is_array($val) ? key($val) : $val, $this->collection->getRedirectCode($key));
			}
			// Store our locale so CodeIgniter object can
			// assign it to the Request.
			if (isset($localeSegment))
			{
				// The following may be inefficient, but doesn't upset NetBeans :-/
				$temp                 = (explode('/', $uri));
				$this->detectedLocale = $temp[$localeSegment];
			}

			// Are we using Closures? If so, then we need
			// to collect the params into an array
			// so it can be passed to the controller method later.
			if (! is_string($val) && is_callable($val))
			{
				$this->controller = $val;

				// Remove the original string from the matches array
				array_shift($matches);

				$this->params = $matches;

				$this->matchedRoute = [
					$matchedKey,
					$val,
				];

				$this->matchedRouteOptions = $this->collection->getRoutesOptions($matchedKey);

				return true;
			}
			// Are we using the default method for back-references?

			// Support resource route when function with subdirectory
			// ex: $routes->resource('Admin/Admins');
			if (strpos($val, '$') !== false && strpos($key, '(') !== false && strpos($key, '/') !== false)
			{
				$replacekey = str_replace('/(.*)', '', $key);
				$val        = preg_replace('#^' . $key . '$#u', $val, $uri);
				$val        = str_replace($replacekey, str_replace('/', '\\', $replacekey), $val);
			}
			elseif (strpos($val, '$') !== false && strpos($key, '(') !== false)
			{
				$val = preg_replace('#^' . $key . '$#u', $val, $uri);
			}
			elseif (strpos($val, '/') !== false)
			{
				[
					$controller,
					$method,
				] = explode( '::', $val );

				// Only replace slashes in the controller, not in the method.
				$controller = str_replace('/', '\\', $controller);

				$val = $controller . '::' . $method;
			}

			$this->setRequest(explode('/', $val));

			$this->matchedRoute = [
				$matchedKey,
				$val,
			];

			$this->matchedRouteOptions = $this->collection->getRoutesOptions($matchedKey);

			return true;
		}
	}

	return false;
}
```

</details>


<hr>

#### autoRoute()

```php
public function autoRoute(string $uri)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to match a URI path against Controllers and directories
found in APPPATH/Controllers, to find a matching route.
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
<td><code>$uri</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 73 lines (522 - 594)</small></summary>

```php
public function autoRoute(string $uri)
{
	$segments = explode('/', $uri);

	$segments = $this->validateRequest($segments);

	// If we don't have any segments left - try the default controller;
	// WARNING: Directories get shifted out of the segments array.
	if (empty($segments))
	{
		$this->setDefaultController();
	}
	// If not empty, then the first segment should be the controller
	else
	{
		$this->controller = ucfirst(array_shift($segments));
	}

	// Use the method name if it exists.
	// If it doesn't, no biggie - the default method name
	// has already been set.
	if (! empty($segments))
	{
		$this->method = array_shift($segments) ?: $this->method;
	}

	if (! empty($segments))
	{
		$this->params = $segments;
	}

	$defaultNamespace = $this->collection->getDefaultNamespace();
	$controllerName   = $this->controllerName();
	if ($this->collection->getHTTPVerb() !== 'cli')
	{
		$controller  = '\\' . $defaultNamespace;
		$controller .= $this->directory ? str_replace('/', '\\', $this->directory) : '';
		$controller .= $controllerName;
		$controller  = strtolower($controller);
		$methodName  = strtolower($this->methodName());

		foreach ($this->collection->getRoutes('cli') as $route)
		{
			if (is_string($route))
			{
				$route = strtolower($route);
				if (strpos($route, $controller . '::' . $methodName) === 0)
				{
					throw new PageNotFoundException();
				}

				if ($route === $controller)
				{
					throw new PageNotFoundException();
				}
			}
		}
	}

	// Load the file so that it's available for CodeIgniter.
	$file = APPPATH . 'Controllers/' . $this->directory . $controllerName . '.php';
	if (is_file($file))
	{
		include_once $file;
	}

	// Ensure the controller stores the fully-qualified class name
	// We have to check for a length over 1, since by default it will be '\'
	if (strpos($this->controller, '\\') === false && strlen($defaultNamespace) > 1)
	{
		$this->controller = '\\' . ltrim(str_replace('/', '\\', $defaultNamespace . $this->directory . $controllerName), '\\');
	}
}
```

</details>


<hr>

#### validateRequest()

```php
protected function validateRequest(array $segments) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to validate the URI request and determine the controller path.
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
<td><code>$segments</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>URI segments</td>
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
<summary><small>Source: 28 lines (605 - 632)</small></summary>

```php
protected function validateRequest(array $segments): array
{
	$segments = array_filter($segments, function ($segment) {
		return ! empty($segment) || ($segment !== '0' || $segment !== 0);
	});
	$segments = array_values($segments);

	$c                  = count($segments);
	$directory_override = isset($this->directory);

	// Loop through our segments and return as soon as a controller
	// is found or when such a directory doesn't exist
	while ($c-- > 0)
	{
		$test = $this->directory . ucfirst($this->translateURIDashes === true ? str_replace('-', '_', $segments[0]) : $segments[0]);

		if (! is_file(APPPATH . 'Controllers/' . $test . '.php') && $directory_override === false && is_dir(APPPATH . 'Controllers/' . $this->directory . ucfirst($segments[0])))
		{
			$this->setDirectory(array_shift($segments), true);
			continue;
		}

		return $segments;
	}

	// This means that all segments were actually directories
	return $segments;
}
```

</details>


<hr>

#### setDirectory()

```php
public function setDirectory(string $dir = null, bool $append = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the sub-directory that the controller is in.
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
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$append</code></td>
<td><em>bool<br>false
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 19 lines (642 - 660)</small></summary>

```php
public function setDirectory(string $dir = null, bool $append = false)
{
	if (empty($dir))
	{
		$this->directory = null;
		return;
	}

	$dir = ucfirst($dir);

	if ($append !== true || empty($this->directory))
	{
		$this->directory = str_replace('.', '', trim($dir, '/')) . '/';
	}
	else
	{
		$this->directory .= str_replace('.', '', trim($dir, '/')) . '/';
	}
}
```

</details>


<hr>

#### setRequest()

```php
protected function setRequest(array $segments = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set request route
</td></tr>
</table>

<table>
<tr><td>
Takes an array of URI segments as input and sets the class/method
to be called.
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
<td><code>$segments</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>URI segments</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 25 lines (672 - 696)</small></summary>

```php
protected function setRequest(array $segments = [])
{
	// If we don't have any segments - try the default controller;
	if (empty($segments))
	{
		$this->setDefaultController();

		return;
	}

	list($controller, $method) = array_pad(explode('::', $segments[0]), 2, null);

	$this->controller = $controller;

	// $this->method already contains the default method name,
	// so don't overwrite it with emptiness.
	if (! empty($method))
	{
		$this->method = $method;
	}

	array_shift($segments);

	$this->params = $segments;
}
```

</details>


<hr>

#### setDefaultController()

```php
protected function setDefaultController()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the default controller based on the info set in the RouteCollection.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 22 lines (703 - 724)</small></summary>

```php
protected function setDefaultController()
{
	if (empty($this->controller))
	{
		throw RouterException::forMissingDefaultRoute();
	}

	// Is the method being specified?
	if (sscanf($this->controller, '%[^/]/%s', $class, $this->method) !== 2)
	{
		$this->method = 'index';
	}

	if (! is_file(APPPATH . 'Controllers/' . $this->directory . ucfirst($class) . '.php'))
	{
		return;
	}

	$this->controller = ucfirst($class);

	log_message('info', 'Used the default controller.');
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Router/Router.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollectionInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouterInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>