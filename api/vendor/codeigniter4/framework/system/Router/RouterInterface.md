


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Router/RouterInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Router.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Security/Exceptions/SecurityException.md">next</a></td>
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
<td>framework/system/Router/RouterInterface.php
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
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Request.md"><strong>CodeIgniter\HTTP\Request</strong></a>
</td>
<td>Request</td>
</tr>
</table>



 
## CodeIgniter\Router\RouterInterface

<table style="text-align:left">
<tr><th>Interface</th><td>RouterInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Router\RouterInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Expected behavior of a Router.
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
<td>Scans the URI and attempts to match the current URI to the
one of the defined routes in the RouteCollection.</td>
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
<td><em>\CodeIgniter\HTTP\Request
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 56</small></summary>

```php
public function __construct(RouteCollectionInterface $routes, Request $request = null);
```

</details>


<hr>

#### handle()

```php
public function handle(string $uri = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Scans the URI and attempts to match the current URI to the
one of the defined routes in the RouteCollection.
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



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: line 68</small></summary>

```php
public function handle(string $uri = null);
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
<summary><small>Source: line 77</small></summary>

```php
public function controllerName();
```

</details>


<hr>

#### methodName()

```php
public function methodName()
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
<summary><small>Source: line 87</small></summary>

```php
public function methodName();
```

</details>


<hr>

#### params()

```php
public function params()
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
<summary><small>Source: line 98</small></summary>

```php
public function params();
```

</details>


<hr>

#### setIndexPage()

```php
public function setIndexPage($page)
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
<summary><small>Source: line 112</small></summary>

```php
public function setIndexPage($page);
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Router/RouterInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Router.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Security/Exceptions/SecurityException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:18**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>