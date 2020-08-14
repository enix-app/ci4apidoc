


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Router/RouteCollectionInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollection.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Router.md">next</a></td>
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
<td>framework/system/Router/RouteCollectionInterface.php
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



 

 
## CodeIgniter\Router\RouteCollectionInterface

<table style="text-align:left">
<tr><th>Interface</th><td>RouteCollectionInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Router\RouteCollectionInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Interface RouteCollectionInterface
</td></tr>
</table>

<table>
<tr><td>
A Route Collection's sole job is to hold a series of routes. The required
number of methods is kept very small on purpose, but implementors may
add a number of additional methods to customize how the routes are defined.

The RouteCollection provides the Router with the routes so that it can determine
which controller should be ran.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Router
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
<th><a href="#add"><strong>add</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Adds a single route to the collection.</td>
</tr>
<tr>
<th><a href="#addPlaceholder"><strong>addPlaceholder</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Registers a new constraint with the system. Constraints are used
by the routes as placeholders for regular expressions to make defining
the routes more human-friendly.</td>
</tr>
<tr>
<th><a href="#setDefaultNamespace"><strong>setDefaultNamespace</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the default namespace to use for Controllers when no other
namespace has been specified.</td>
</tr>
<tr>
<th><a href="#setDefaultController"><strong>setDefaultController</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the default controller to use when no other controller has been
specified.</td>
</tr>
<tr>
<th><a href="#setDefaultMethod"><strong>setDefaultMethod</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the default method to call on the controller when no other
method has been set in the route.</td>
</tr>
<tr>
<th><a href="#setTranslateURIDashes"><strong>setTranslateURIDashes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Tells the system whether to convert dashes in URI strings into
underscores. In some search engines, including Google, dashes
create more meaning and make it easier for the search engine to
find words and meaning in the URI for better SEO. But it
doesn&#039;t work well with PHP method names.</td>
</tr>
<tr>
<th><a href="#setAutoRoute"><strong>setAutoRoute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>If TRUE, the system will attempt to match the URI against
Controllers by matching each segment against folders/files
in APPPATH/Controllers, when a match wasn&#039;t found against
defined routes.</td>
</tr>
<tr>
<th><a href="#set404Override"><strong>set404Override</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the class/method that should be called if routing doesn&#039;t
find a match. It can be either a closure or the controller/method
name exactly like a route is defined: Users::index</td>
</tr>
<tr>
<th><a href="#get404Override"><strong>get404Override</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the 404 Override setting, which can be null, a closure
or the controller/string.</td>
</tr>
<tr>
<th><a href="#getDefaultController"><strong>getDefaultController</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the name of the default controller. With Namespace.</td>
</tr>
<tr>
<th><a href="#getDefaultMethod"><strong>getDefaultMethod</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the name of the default method to use within the controller.</td>
</tr>
<tr>
<th><a href="#shouldTranslateURIDashes"><strong>shouldTranslateURIDashes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the current value of the translateURIDashes setting.</td>
</tr>
<tr>
<th><a href="#shouldAutoRoute"><strong>shouldAutoRoute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the flag that tells whether to autoRoute URI against Controllers.</td>
</tr>
<tr>
<th><a href="#getRoutes"><strong>getRoutes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the raw array of available routes.</td>
</tr>
<tr>
<th><a href="#getHTTPVerb"><strong>getHTTPVerb</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the current HTTP Verb being used.</td>
</tr>
<tr>
<th><a href="#reverseRoute"><strong>reverseRoute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attempts to look up a route based on it&#039;s destination.</td>
</tr>
<tr>
<th><a href="#isRedirect"><strong>isRedirect</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines if the route is a redirecting route.</td>
</tr>
<tr>
<th><a href="#getRedirectCode"><strong>getRedirectCode</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Grabs the HTTP status code from a redirecting Route.</td>
</tr>

</table>






### Methods


<hr>

#### add()

```php
public function add(string $from, $to, array $options = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Adds a single route to the collection.
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
<td><code>$from</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$to</code></td>
<td><em>array<br>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
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
<summary><small>Source: line 66</small></summary>

```php
public function add(string $from, $to, array $options = null);
```

</details>


<hr>

#### addPlaceholder()

```php
public function addPlaceholder($placeholder, string $pattern = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Registers a new constraint with the system. Constraints are used
by the routes as placeholders for regular expressions to make defining
the routes more human-friendly.
</td></tr>
</table>

<table>
<tr><td>
You can pass an associative array as $placeholder, and have
multiple placeholders added at once.
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
<td><code>$placeholder</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$pattern</code></td>
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
<summary><small>Source: line 83</small></summary>

```php
public function addPlaceholder($placeholder, string $pattern = null);
```

</details>


<hr>

#### setDefaultNamespace()

```php
public function setDefaultNamespace(string $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the default namespace to use for Controllers when no other
namespace has been specified.
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
<td><code>$value</code></td>
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
<summary><small>Source: line 95</small></summary>

```php
public function setDefaultNamespace(string $value);
```

</details>


<hr>

#### setDefaultController()

```php
public function setDefaultController(string $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the default controller to use when no other controller has been
specified.
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
<td><code>$value</code></td>
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
<summary><small>Source: line 107</small></summary>

```php
public function setDefaultController(string $value);
```

</details>


<hr>

#### setDefaultMethod()

```php
public function setDefaultMethod(string $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the default method to call on the controller when no other
method has been set in the route.
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
<td><code>$value</code></td>
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
<summary><small>Source: line 119</small></summary>

```php
public function setDefaultMethod(string $value);
```

</details>


<hr>

#### setTranslateURIDashes()

```php
public function setTranslateURIDashes(bool $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Tells the system whether to convert dashes in URI strings into
underscores. In some search engines, including Google, dashes
create more meaning and make it easier for the search engine to
find words and meaning in the URI for better SEO. But it
doesn't work well with PHP method names.
</td></tr>
</table>

<table>
<tr><td>
...
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
<td><code>$value</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: line 134</small></summary>

```php
public function setTranslateURIDashes(bool $value);
```

</details>


<hr>

#### setAutoRoute()

```php
public function setAutoRoute(bool $value) : self
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
If TRUE, the system will attempt to match the URI against
Controllers by matching each segment against folders/files
in APPPATH/Controllers, when a match wasn't found against
defined routes.
</td></tr>
</table>

<table>
<tr><td>
If FALSE, will stop searching and do NO automatic routing.
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
<td><code>$value</code></td>
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
<td>\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 150</small></summary>

```php
public function setAutoRoute(bool $value): self;
```

</details>


<hr>

#### set404Override()

```php
public function set404Override($callable = null) : self
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the class/method that should be called if routing doesn't
find a match. It can be either a closure or the controller/method
name exactly like a route is defined: Users::index
</td></tr>
</table>

<table>
<tr><td>
This setting is passed to the Router class and handled there.
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
<td><code>$callable</code></td>
<td><em>callable<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 165</small></summary>

```php
public function set404Override($callable = null): self;
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
Returns the 404 Override setting, which can be null, a closure
or the controller/string.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>\Closure<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: line 175</small></summary>

```php
public function get404Override();
```

</details>


<hr>

#### getDefaultController()

```php
public function getDefaultController()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the name of the default controller. With Namespace.
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
<summary><small>Source: line 184</small></summary>

```php
public function getDefaultController();
```

</details>


<hr>

#### getDefaultMethod()

```php
public function getDefaultMethod()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the name of the default method to use within the controller.
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
<summary><small>Source: line 193</small></summary>

```php
public function getDefaultMethod();
```

</details>


<hr>

#### shouldTranslateURIDashes()

```php
public function shouldTranslateURIDashes()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the current value of the translateURIDashes setting.
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
<summary><small>Source: line 202</small></summary>

```php
public function shouldTranslateURIDashes();
```

</details>


<hr>

#### shouldAutoRoute()

```php
public function shouldAutoRoute()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the flag that tells whether to autoRoute URI against Controllers.
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
<summary><small>Source: line 211</small></summary>

```php
public function shouldAutoRoute();
```

</details>


<hr>

#### getRoutes()

```php
public function getRoutes()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the raw array of available routes.
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
<summary><small>Source: line 220</small></summary>

```php
public function getRoutes();
```

</details>


<hr>

#### getHTTPVerb()

```php
public function getHTTPVerb()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the current HTTP Verb being used.
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
<summary><small>Source: line 229</small></summary>

```php
public function getHTTPVerb();
```

</details>


<hr>

#### reverseRoute()

```php
public function reverseRoute(string $search, ...$params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to look up a route based on it's destination.
</td></tr>
</table>

<table>
<tr><td>
If a route exists:

     'path/(:any)/(:any)' => 'Controller::method/$1/$2'

This method allows you to know the Controller and method
and get the route that leads to it.

     // Equals 'path/$param1/$param2'
     reverseRoute('Controller::method', $param1, $param2);
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
<td><code>$search</code></td>
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
<td>string<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: line 251</small></summary>

```php
public function reverseRoute(string $search, ...$params);
```

</details>


<hr>

#### isRedirect()

```php
public function isRedirect(string $from) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines if the route is a redirecting route.
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
<td><code>$from</code></td>
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
<summary><small>Source: line 262</small></summary>

```php
public function isRedirect(string $from): bool;
```

</details>


<hr>

#### getRedirectCode()

```php
public function getRedirectCode(string $from) : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Grabs the HTTP status code from a redirecting Route.
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
<td><code>$from</code></td>
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
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: line 273</small></summary>

```php
public function getRedirectCode(string $from): int;
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Router/RouteCollectionInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollection.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Router.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>