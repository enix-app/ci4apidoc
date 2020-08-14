


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Router/RouteCollection.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RouterException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollectionInterface.md">next</a></td>
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
<td>framework/system/Router/RouteCollection.php
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
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/FileLocator.md"><strong>CodeIgniter\Autoloader\FileLocator</strong></a>
</td>
<td>FileLocator</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Request.md"><strong>CodeIgniter\HTTP\Request</strong></a>
</td>
<td>Request</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RouterException.md"><strong>CodeIgniter\Router\Exceptions\RouterException</strong></a>
</td>
<td>RouterException</td>
</tr>
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
</table>



 
## CodeIgniter\Router\RouteCollection

<table style="text-align:left">
<tr><th>Class</th><td>RouteCollection</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Router\RouteCollection</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollectionInterface.md">CodeIgniter\Router\RouteCollectionInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class RouteCollection
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>todo</th>
<td>Implement nested resource routing (See CakePHP)
</td>
</tr>
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
<th><a href="#defaultNamespace"><strong>defaultNamespace</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The namespace to be added to any Controllers.</td>
</tr>
<tr>
<th><a href="#defaultController"><strong>defaultController</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the default controller to use
when no other controller is specified.</td>
</tr>
<tr>
<th><a href="#defaultMethod"><strong>defaultMethod</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the default method to use
when no other method has been specified.</td>
</tr>
<tr>
<th><a href="#defaultPlaceholder"><strong>defaultPlaceholder</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The placeholder used when routing &#039;resources&#039;
when no other placeholder has been specified.</td>
</tr>
<tr>
<th><a href="#translateURIDashes"><strong>translateURIDashes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether to convert dashes to underscores in URI.</td>
</tr>
<tr>
<th><a href="#autoRoute"><strong>autoRoute</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether to match URI against Controllers
when it doesn&#039;t match defined routes.</td>
</tr>
<tr>
<th><a href="#override404"><strong>override404</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>A callable that will be shown
when the route cannot be matched.</td>
</tr>
<tr>
<th><a href="#placeholders"><strong>placeholders</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Defined placeholders that can be used
within the</td>
</tr>
<tr>
<th><a href="#routes"><strong>routes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>An array of all routes and their mappings.</td>
</tr>
<tr>
<th><a href="#routesOptions"><strong>routesOptions</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Array of routes options</td>
</tr>
<tr>
<th><a href="#HTTPVerb"><strong>HTTPVerb</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The current method that the script is being called by.</td>
</tr>
<tr>
<th><a href="#defaultHTTPMethods"><strong>defaultHTTPMethods</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The default list of HTTP methods (and CLI for command line usage)
that is allowed if no other method is provided.</td>
</tr>
<tr>
<th><a href="#group"><strong>group</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the current group, if any.</td>
</tr>
<tr>
<th><a href="#currentSubdomain"><strong>currentSubdomain</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The current subdomain.</td>
</tr>
<tr>
<th><a href="#currentOptions"><strong>currentOptions</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores copy of current options being
applied during creation.</td>
</tr>
<tr>
<th><a href="#didDiscover"><strong>didDiscover</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>A little performance booster.</td>
</tr>
<tr>
<th><a href="#fileLocator"><strong>fileLocator</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Handle to the file locator to use.</td>
</tr>
<tr>
<th><a href="#moduleConfig"><strong>moduleConfig</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Handle to the modules config.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor</td>
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
<th><a href="#discoverRoutes"><strong>discoverRoutes</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Will attempt to discover any additional routes, either through
the local PSR4 namespaces, or through selected Composer packages.</td>
</tr>
<tr>
<th><a href="#setDefaultConstraint"><strong>setDefaultConstraint</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the default constraint to be used in the system. Typically
for use with the &#039;resource&#039; method.</td>
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
<th><a href="#getDefaultNamespace"><strong>getDefaultNamespace</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the default namespace as set in the Routes config file.</td>
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
<th><a href="#getRoutesOptions"><strong>getRoutesOptions</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns one or all routes options</td>
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
<th><a href="#setHTTPVerb"><strong>setHTTPVerb</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the current HTTP verb.</td>
</tr>
<tr>
<th><a href="#map"><strong>map</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>A shortcut method to add a number of routes at a single time.</td>
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
<th><a href="#addRedirect"><strong>addRedirect</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Adds a temporary redirect from one route to another. Used for
redirecting traffic from old, non-existing routes to the new
moved routes.</td>
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
<tr>
<th><a href="#group"><strong>group</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Group a series of routes under a single URL segment. This is handy
for grouping items into an admin area, like:</td>
</tr>
<tr>
<th><a href="#resource"><strong>resource</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Creates a collections of HTTP-verb based routes for a controller.</td>
</tr>
<tr>
<th><a href="#presenter"><strong>presenter</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Creates a collections of HTTP-verb based routes for a presenter controller.</td>
</tr>
<tr>
<th><a href="#match"><strong>match</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a single route to match for multiple HTTP Verbs.</td>
</tr>
<tr>
<th><a href="#get"><strong>get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a route that is only available to GET requests.</td>
</tr>
<tr>
<th><a href="#post"><strong>post</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a route that is only available to POST requests.</td>
</tr>
<tr>
<th><a href="#put"><strong>put</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a route that is only available to PUT requests.</td>
</tr>
<tr>
<th><a href="#delete"><strong>delete</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a route that is only available to DELETE requests.</td>
</tr>
<tr>
<th><a href="#head"><strong>head</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a route that is only available to HEAD requests.</td>
</tr>
<tr>
<th><a href="#patch"><strong>patch</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a route that is only available to PATCH requests.</td>
</tr>
<tr>
<th><a href="#options"><strong>options</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a route that is only available to OPTIONS requests.</td>
</tr>
<tr>
<th><a href="#cli"><strong>cli</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies a route that is only available to command-line requests.</td>
</tr>
<tr>
<th><a href="#environment"><strong>environment</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Limits the routes to a specified ENVIRONMENT or they won&#039;t run.</td>
</tr>
<tr>
<th><a href="#reverseRoute"><strong>reverseRoute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attempts to look up a route based on its destination.</td>
</tr>
<tr>
<th><a href="#localizeRoute"><strong>localizeRoute</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Replaces the {locale} tag with the current application locale</td>
</tr>
<tr>
<th><a href="#isFiltered"><strong>isFiltered</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks a route (using the &quot;from&quot;) to see if it&#039;s filtered or not.</td>
</tr>
<tr>
<th><a href="#getFilterForRoute"><strong>getFilterForRoute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the filter that should be applied for a single route, along
with any parameters it might have. Parameters are found by splitting
the parameter name on a colon to separate the filter name from the parameter list,
and the splitting the result on commas. So:</td>
</tr>
<tr>
<th><a href="#fillRouteParams"><strong>fillRouteParams</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Given a</td>
</tr>
<tr>
<th><a href="#create"><strong>create</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Does the heavy lifting of creating an actual route. You must specify
the request method(s) that this route will work for. They can be separated
by a pipe character &quot;|&quot; if there is more than one.</td>
</tr>
<tr>
<th><a href="#checkSubdomains"><strong>checkSubdomains</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Compares the subdomain(s) passed in against the current subdomain
on this page request.</td>
</tr>
<tr>
<th><a href="#determineCurrentSubdomain"><strong>determineCurrentSubdomain</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Examines the HTTP_HOST to get a best match for the subdomain. It
won&#039;t be perfect, but should work for our needs.</td>
</tr>
<tr>
<th><a href="#resetRoutes"><strong>resetRoutes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Reset the routes, so that a FeatureTestCase can provide the
explicit ones needed for it.</td>
</tr>

</table>





### Properties


<hr>

#### $defaultNamespace

```php
protected $defaultNamespace = '\\';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The namespace to be added to any Controllers.
</td></tr>
</table>

<table>
<tr><td>
Defaults to the global namespaces (\)
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

#### $defaultController

```php
protected $defaultController = 'Home';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the default controller to use
when no other controller is specified.
</td></tr>
</table>

<table>
<tr><td>
Not used here. Pass-thru value for Router class.
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

#### $defaultMethod

```php
protected $defaultMethod = 'index';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the default method to use
when no other method has been specified.
</td></tr>
</table>

<table>
<tr><td>
Not used here. Pass-thru value for Router class.
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

#### $defaultPlaceholder

```php
protected $defaultPlaceholder = 'any';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The placeholder used when routing 'resources'
when no other placeholder has been specified.
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
Whether to convert dashes to underscores in URI.
</td></tr>
</table>

<table>
<tr><td>
Not used here. Pass-thru value for Router class.
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

#### $autoRoute

```php
protected $autoRoute = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to match URI against Controllers
when it doesn't match defined routes.
</td></tr>
</table>

<table>
<tr><td>
Not used here. Pass-thru value for Router class.
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

#### $override404

```php
protected $override404;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A callable that will be shown
when the route cannot be matched.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>string<br>\Closure
</td>
</tr>
</table>


<hr>

#### $placeholders

```php
protected $placeholders = [
	'any'      => '.*',
	'segment'  => '[^/]+',
	'alphanum' => '[a-zA-Z0-9]+',
	'num'      => '[0-9]+',
	'alpha'    => '[a-zA-Z]+',
	'hash'     => '[^/]+',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Defined placeholders that can be used
within the
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

#### $routes

```php
protected $routes = [
	'*'       => [],
	'options' => [],
	'get'     => [],
	'head'    => [],
	'post'    => [],
	'put'     => [],
	'delete'  => [],
	'trace'   => [],
	'connect' => [],
	'cli'     => [],
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
An array of all routes and their mappings.
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

#### $routesOptions

```php
protected $routesOptions = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Array of routes options
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

#### $HTTPVerb

```php
protected $HTTPVerb;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The current method that the script is being called by.
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

#### $defaultHTTPMethods

```php
protected $defaultHTTPMethods = [
	'options',
	'get',
	'head',
	'post',
	'put',
	'delete',
	'trace',
	'connect',
	'cli',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The default list of HTTP methods (and CLI for command line usage)
that is allowed if no other method is provided.
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

#### $group

```php
protected $group;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the current group, if any.
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

#### $currentSubdomain

```php
protected $currentSubdomain;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The current subdomain.
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

#### $currentOptions

```php
protected $currentOptions;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores copy of current options being
applied during creation.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>null
</td>
</tr>
</table>


<hr>

#### $didDiscover

```php
protected $didDiscover = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A little performance booster.
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

#### $fileLocator

```php
protected $fileLocator;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handle to the file locator to use.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Autoloader\FileLocator
</td>
</tr>
</table>


<hr>

#### $moduleConfig

```php
protected $moduleConfig;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handle to the modules config.
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
public function __construct(FileLocator $locator, $moduleConfig)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor
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
<td><code>$locator</code></td>
<td><em>\CodeIgniter\Autoloader\FileLocator
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








<details>
<summary><small>Source: 5 lines (236 - 240)</small></summary>

```php
public function __construct(FileLocator $locator, $moduleConfig)
{
	$this->fileLocator  = $locator;
	$this->moduleConfig = $moduleConfig;
}
```

</details>


<hr>

#### addPlaceholder()

```php
public function addPlaceholder($placeholder, string $pattern = null) : RouteCollectionInterface
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
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (257 - 267)</small></summary>

```php
public function addPlaceholder($placeholder, string $pattern = null): RouteCollectionInterface
{
	if (! is_array($placeholder))
	{
		$placeholder = [$placeholder => $pattern];
	}

	$this->placeholders = array_merge($this->placeholders, $placeholder);

	return $this;
}
```

</details>


<hr>

#### setDefaultNamespace()

```php
public function setDefaultNamespace(string $value) : RouteCollectionInterface
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
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 7 lines (279 - 285)</small></summary>

```php
public function setDefaultNamespace(string $value): RouteCollectionInterface
{
	$this->defaultNamespace = filter_var($value, FILTER_SANITIZE_STRING);
	$this->defaultNamespace = rtrim($this->defaultNamespace, '\\') . '\\';

	return $this;
}
```

</details>


<hr>

#### setDefaultController()

```php
public function setDefaultController(string $value) : RouteCollectionInterface
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
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (297 - 302)</small></summary>

```php
public function setDefaultController(string $value): RouteCollectionInterface
{
	$this->defaultController = filter_var($value, FILTER_SANITIZE_STRING);

	return $this;
}
```

</details>


<hr>

#### setDefaultMethod()

```php
public function setDefaultMethod(string $value) : RouteCollectionInterface
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
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (314 - 319)</small></summary>

```php
public function setDefaultMethod(string $value): RouteCollectionInterface
{
	$this->defaultMethod = filter_var($value, FILTER_SANITIZE_STRING);

	return $this;
}
```

</details>


<hr>

#### setTranslateURIDashes()

```php
public function setTranslateURIDashes(bool $value) : RouteCollectionInterface
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
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (334 - 339)</small></summary>

```php
public function setTranslateURIDashes(bool $value): RouteCollectionInterface
{
	$this->translateURIDashes = $value;

	return $this;
}
```

</details>


<hr>

#### setAutoRoute()

```php
public function setAutoRoute(bool $value) : RouteCollectionInterface
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
<summary><small>Source: 6 lines (355 - 360)</small></summary>

```php
public function setAutoRoute(bool $value): RouteCollectionInterface
{
	$this->autoRoute = $value;

	return $this;
}
```

</details>


<hr>

#### set404Override()

```php
public function set404Override($callable = null) : RouteCollectionInterface
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
<summary><small>Source: 6 lines (375 - 380)</small></summary>

```php
public function set404Override($callable = null): RouteCollectionInterface
{
	$this->override404 = $callable;

	return $this;
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
<summary><small>Source: 4 lines (390 - 393)</small></summary>

```php
public function get404Override()
{
	return $this->override404;
}
```

</details>


<hr>

#### discoverRoutes()

```php
protected function discoverRoutes()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Will attempt to discover any additional routes, either through
the local PSR4 namespaces, or through selected Composer packages.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 29 lines (401 - 429)</small></summary>

```php
protected function discoverRoutes()
{
	if ($this->didDiscover)
	{
		return;
	}

	// We need this var in local scope
	// so route files can access it.
	$routes = $this;

	if ($this->moduleConfig->shouldDiscover('routes'))
	{
		$files = $this->fileLocator->search('Config/Routes.php');

		foreach ($files as $file)
		{
			// Don't include our main file again...
			if ($file === APPPATH . 'Config/Routes.php')
			{
				continue;
			}

			include $file;
		}
	}

	$this->didDiscover = true;
}
```

</details>


<hr>

#### setDefaultConstraint()

```php
public function setDefaultConstraint(string $placeholder) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the default constraint to be used in the system. Typically
for use with the 'resource' method.
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
<td>\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (441 - 449)</small></summary>

```php
public function setDefaultConstraint(string $placeholder): RouteCollectionInterface
{
	if (array_key_exists($placeholder, $this->placeholders))
	{
		$this->defaultPlaceholder = $placeholder;
	}

	return $this;
}
```

</details>


<hr>

#### getDefaultController()

```php
public function getDefaultController() : string
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
<summary><small>Source: 4 lines (458 - 461)</small></summary>

```php
public function getDefaultController(): string
{
	return $this->defaultController;
}
```

</details>


<hr>

#### getDefaultMethod()

```php
public function getDefaultMethod() : string
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
<summary><small>Source: 4 lines (470 - 473)</small></summary>

```php
public function getDefaultMethod(): string
{
	return $this->defaultMethod;
}
```

</details>


<hr>

#### getDefaultNamespace()

```php
public function getDefaultNamespace() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the default namespace as set in the Routes config file.
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
<summary><small>Source: 4 lines (482 - 485)</small></summary>

```php
public function getDefaultNamespace(): string
{
	return $this->defaultNamespace;
}
```

</details>


<hr>

#### shouldTranslateURIDashes()

```php
public function shouldTranslateURIDashes() : bool
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (494 - 497)</small></summary>

```php
public function shouldTranslateURIDashes(): bool
{
	return $this->translateURIDashes;
}
```

</details>


<hr>

#### shouldAutoRoute()

```php
public function shouldAutoRoute() : bool
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
<summary><small>Source: 4 lines (506 - 509)</small></summary>

```php
public function shouldAutoRoute(): bool
{
	return $this->autoRoute;
}
```

</details>


<hr>

#### getRoutes()

```php
public function getRoutes($verb = null) : array
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
<td><code>$verb</code></td>
<td><em>mixed
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
<summary><small>Source: 32 lines (520 - 551)</small></summary>

```php
public function getRoutes($verb = null): array
{
	if (empty($verb))
	{
		$verb = $this->getHTTPVerb();
	}

	// Since this is the entry point for the Router,
	// take a moment to do any route discovery
	// we might need to do.
	$this->discoverRoutes();

	$routes = [];

	if (isset($this->routes[$verb]))
	{
		// Keep current verb's routes at the beginning so they're matched
		// before any of the generic, "add" routes.
		if (isset($this->routes['*']))
		{
			$extraRules = array_diff_key($this->routes['*'], $this->routes[$verb]);
			$collection = array_merge($this->routes[$verb], $extraRules);
		}
		foreach ($collection as $r)
		{
			$key          = key($r['route']);
			$routes[$key] = $r['route'][$key];
		}
	}

	return $routes;
}
```

</details>


<hr>

#### getRoutesOptions()

```php
public function getRoutesOptions(string $from = null) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns one or all routes options
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (562 - 565)</small></summary>

```php
public function getRoutesOptions(string $from = null): array
{
	return $from ? $this->routesOptions[$from] ?? [] : $this->routesOptions;
}
```

</details>


<hr>

#### getHTTPVerb()

```php
public function getHTTPVerb() : string
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
<summary><small>Source: 4 lines (574 - 577)</small></summary>

```php
public function getHTTPVerb(): string
{
	return $this->HTTPVerb;
}
```

</details>


<hr>

#### setHTTPVerb()

```php
public function setHTTPVerb(string $verb)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the current HTTP verb.
</td></tr>
</table>

<table>
<tr><td>
Used primarily for testing.
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
<td><code>$verb</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (589 - 594)</small></summary>

```php
public function setHTTPVerb(string $verb)
{
	$this->HTTPVerb = $verb;

	return $this;
}
```

</details>


<hr>

#### map()

```php
public function map(array $routes = array(), array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A shortcut method to add a number of routes at a single time.
</td></tr>
</table>

<table>
<tr><td>
It does not allow any options to be set on the route, or to
define the method used.
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
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (606 - 614)</small></summary>

```php
public function map(array $routes = [], array $options = null): RouteCollectionInterface
{
	foreach ($routes as $from => $to)
	{
		$this->add($from, $to, $options);
	}

	return $this;
}
```

</details>


<hr>

#### add()

```php
public function add(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Adds a single route to the collection.
</td></tr>
</table>

<table>
<tr><td>
Example:
$routes->add('news', 'Posts::index');
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
<td><em>array<br>null
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
<summary><small>Source: 6 lines (630 - 635)</small></summary>

```php
public function add(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('*', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### addRedirect()

```php
public function addRedirect(string $from, string $to, int $status = 302)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Adds a temporary redirect from one route to another. Used for
redirecting traffic from old, non-existing routes to the new
moved routes.
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
<td>The pattern to match against</td>
</tr>

<tr>
<td>2.</td>
<td><code>$to</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Either a route name or a URI to redirect to</td>
</tr>

<tr>
<td>3.</td>
<td><code>$status</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The HTTP status code that should be returned with this redirect</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\RouteCollection
</td>
</tr>
</table>





<details>
<summary><small>Source: 16 lines (650 - 665)</small></summary>

```php
public function addRedirect(string $from, string $to, int $status = 302)
{
	// Use the named route's pattern if this is a named route.
	if (array_key_exists($to, $this->routes['*']))
	{
		$to = $this->routes['*'][$to]['route'];
	}
	elseif (array_key_exists($to, $this->routes['get']))
	{
		$to = $this->routes['get'][$to]['route'];
	}

	$this->create('*', $from, $to, ['redirect' => $status]);

	return $this;
}
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
<summary><small>Source: 13 lines (676 - 688)</small></summary>

```php
public function isRedirect(string $from): bool
{
	foreach ($this->routes['*'] as $name => $route)
	{
		// Named route?
		if ($name === $from || key($route['route']) === $from)
		{
			return isset($route['redirect']) && is_numeric($route['redirect']);
		}
	}

	return false;
}
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
<summary><small>Source: 13 lines (699 - 711)</small></summary>

```php
public function getRedirectCode(string $from): int
{
	foreach ($this->routes['*'] as $name => $route)
	{
		// Named route?
		if ($name === $from || key($route['route']) === $from)
		{
			return $route['redirect'] ?? 0;
		}
	}

	return 0;
}
```

</details>


<hr>

#### group()

```php
public function group(string $name, ...$params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Group a series of routes under a single URL segment. This is handy
for grouping items into an admin area, like:
</td></tr>
</table>

<table>
<tr><td>
Example:
// Creates route: admin/users
$route->group('admin', function() {
       $route->resource('users');
});
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
<td>The name to group/prefix the routes with.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
<td><em>mixed
</em></td>
<td>true</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 24 lines (733 - 756)</small></summary>

```php
public function group(string $name, ...$params)
{
	$oldGroup   = $this->group;
	$oldOptions = $this->currentOptions;

	// To register a route, we'll set a flag so that our router
	// so it will see the group name.
	$this->group = ltrim($oldGroup . '/' . $name, '/');

	$callback = array_pop($params);

	if ($params && is_array($params[0]))
	{
		$this->currentOptions = array_shift($params);
	}

	if (is_callable($callback))
	{
		$callback($this);
	}

	$this->group          = $oldGroup;
	$this->currentOptions = $oldOptions;
}
```

</details>


<hr>

#### resource()

```php
public function resource(string $name, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Creates a collections of HTTP-verb based routes for a controller.
</td></tr>
</table>

<table>
<tr><td>
Possible Options:
     'controller'    - Customize the name of the controller used in the 'to' route
     'placeholder'   - The regex used by the Router. Defaults to '(:any)'
     'websafe'   -	- '1' if only GET and POST HTTP verbs are supported

Example:

     $route->resource('photos');

     // Generates the following routes:
     HTTP Verb | Path        | Action        | Used for...
     ----------+-------------+---------------+-----------------
     GET         /photos             index           an array of photo objects
     GET         /photos/new         new             an empty photo object, with default properties
     GET         /photos/{id}/edit   edit            a specific photo object, editable properties
     GET         /photos/{id}        show            a specific photo object, all properties
     POST        /photos             create          a new photo object, to add to the resource
     DELETE      /photos/{id}        delete          deletes the specified photo object
     PUT/PATCH   /photos/{id}        update          replacement properties for existing photo

 If 'websafe' option is present, the following paths are also available:

     POST		/photos/{id}/delete delete
     POST        /photos/{id}        update
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
<td>The name of the resource/controller to route to.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td>An list of possible ways to customize the routing.</td>
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
<summary><small>Source: 85 lines (804 - 888)</small></summary>

```php
public function resource(string $name, array $options = null): RouteCollectionInterface
{
	// In order to allow customization of the route the
	// resources are sent to, we need to have a new name
	// to store the values in.
	$new_name = ucfirst($name);

	// If a new controller is specified, then we replace the
	// $name value with the name of the new controller.
	if (isset($options['controller']))
	{
		$new_name = ucfirst(filter_var($options['controller'], FILTER_SANITIZE_STRING));
	}

	// In order to allow customization of allowed id values
	// we need someplace to store them.
	$id = $this->placeholders[$this->defaultPlaceholder] ?? '(:segment)';

	if (isset($options['placeholder']))
	{
		$id = $options['placeholder'];
	}

	// Make sure we capture back-references
	$id = '(' . trim($id, '()') . ')';

	$methods = isset($options['only']) ? (is_string($options['only']) ? explode(',', $options['only']) : $options['only']) : ['index', 'show', 'create', 'update', 'delete', 'new', 'edit'];

	if (isset($options['except']))
	{
		$options['except'] = is_array($options['except']) ? $options['except'] : explode(',', $options['except']);
		foreach ($methods as $i => $method)
		{
			if (in_array($method, $options['except']))
			{
				unset($methods[$i]);
			}
		}
	}

	if (in_array('index', $methods))
	{
		$this->get($name, $new_name . '::index', $options);
	}
	if (in_array('new', $methods))
	{
		$this->get($name . '/new', $new_name . '::new', $options);
	}
	if (in_array('edit', $methods))
	{
		$this->get($name . '/' . $id . '/edit', $new_name . '::edit/$1', $options);
	}
	if (in_array('show', $methods))
	{
		$this->get($name . '/' . $id, $new_name . '::show/$1', $options);
	}
	if (in_array('create', $methods))
	{
		$this->post($name, $new_name . '::create', $options);
	}
	if (in_array('update', $methods))
	{
		$this->put($name . '/' . $id, $new_name . '::update/$1', $options);
		$this->patch($name . '/' . $id, $new_name . '::update/$1', $options);
	}
	if (in_array('delete', $methods))
	{
		$this->delete($name . '/' . $id, $new_name . '::delete/$1', $options);
	}

	// Web Safe? delete needs checking before update because of method name
	if (isset($options['websafe']))
	{
		if (in_array('delete', $methods))
		{
			$this->post($name . '/' . $id . '/delete', $new_name . '::delete/$1', $options);
		}
		if (in_array('update', $methods))
		{
			$this->post($name . '/' . $id, $new_name . '::update/$1', $options);
		}
	}

	return $this;
}
```

</details>


<hr>

#### presenter()

```php
public function presenter(string $name, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Creates a collections of HTTP-verb based routes for a presenter controller.
</td></tr>
</table>

<table>
<tr><td>
Possible Options:
     'controller'    - Customize the name of the controller used in the 'to' route
     'placeholder'   - The regex used by the Router. Defaults to '(:any)'

Example:

     $route->presenter('photos');

     // Generates the following routes:
     HTTP Verb | Path        | Action        | Used for...
     ----------+-------------+---------------+-----------------
     GET         /photos             index           showing all array of photo objects
     GET         /photos/show/{id}   show            showing a specific photo object, all properties
     GET         /photos/new         new             showing a form for an empty photo object, with default properties
     POST        /photos/create      create          processing the form for a new photo
     GET         /photos/edit/{id}   edit            show an editing form for a specific photo object, editable properties
     POST        /photos/update/{id} update          process the editing form data
     GET         /photos/remove/{id} remove          show a form to confirm deletion of a specific photo object
     POST        /photos/delete/{id} delete          deleting the specified photo object
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
<td>The name of the controller to route to.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td>An list of possible ways to customize the routing.</td>
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
<summary><small>Source: 83 lines (918 - 1000)</small></summary>

```php
public function presenter(string $name, array $options = null): RouteCollectionInterface
{
	// In order to allow customization of the route the
	// resources are sent to, we need to have a new name
	// to store the values in.
	$newName = ucfirst($name);

	// If a new controller is specified, then we replace the
	// $name value with the name of the new controller.
	if (isset($options['controller']))
	{
		$newName = ucfirst(filter_var($options['controller'], FILTER_SANITIZE_STRING));
	}

	// In order to allow customization of allowed id values
	// we need someplace to store them.
	$id = $this->placeholders[$this->defaultPlaceholder] ?? '(:segment)';

	if (isset($options['placeholder']))
	{
		$id = $options['placeholder'];
	}

	// Make sure we capture back-references
	$id = '(' . trim($id, '()') . ')';

	$methods = isset($options['only']) ? (is_string($options['only']) ? explode(',', $options['only']) : $options['only']) : ['index', 'show', 'new', 'create', 'edit', 'update', 'remove', 'delete'];

	if (isset($options['except']))
	{
		$options['except'] = is_array($options['except']) ? $options['except'] : explode(',', $options['except']);
		foreach ($methods as $i => $method)
		{
			if (in_array($method, $options['except']))
			{
				unset($methods[$i]);
			}
		}
	}

	if (in_array('index', $methods))
	{
		$this->get($name, $newName . '::index', $options);
	}
	if (in_array('show', $methods))
	{
		$this->get($name . '/show/' . $id, $newName . '::show/$1', $options);
	}
	if (in_array('new', $methods))
	{
		$this->get($name . '/new', $newName . '::new', $options);
	}
	if (in_array('create', $methods))
	{
		$this->post($name . '/create', $newName . '::create', $options);
	}
	if (in_array('edit', $methods))
	{
		$this->get($name . '/edit/' . $id, $newName . '::edit/$1', $options);
	}
	if (in_array('update', $methods))
	{
		$this->post($name . '/update/' . $id, $newName . '::update/$1', $options);
	}
	if (in_array('remove', $methods))
	{
		$this->get($name . '/remove/' . $id, $newName . '::remove/$1', $options);
	}
	if (in_array('delete', $methods))
	{
		$this->post($name . '/delete/' . $id, $newName . '::delete/$1', $options);
	}
	if (in_array('show', $methods))
	{
		$this->get($name . '/' . $id, $newName . '::show/$1', $options);
	}
	if (in_array('create', $methods))
	{
		$this->post($name, $newName . '::create', $options);
	}

	return $this;
}
```

</details>


<hr>

#### match()

```php
public function match(array $verbs = array(), string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a single route to match for multiple HTTP Verbs.
</td></tr>
</table>

<table>
<tr><td>
Example:
$route->match( ['get', 'post'], 'users/(:num)', 'users/$1);
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
<td><code>$verbs</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$from</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$to</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (1017 - 1027)</small></summary>

```php
public function match(array $verbs = [], string $from, $to, array $options = null): RouteCollectionInterface
{
	foreach ($verbs as $verb)
	{
		$verb = strtolower($verb);

		$this->{$verb}($from, $to, $options);
	}

	return $this;
}
```

</details>


<hr>

#### get()

```php
public function get(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a route that is only available to GET requests.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1040 - 1045)</small></summary>

```php
public function get(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('get', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### post()

```php
public function post(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a route that is only available to POST requests.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1058 - 1063)</small></summary>

```php
public function post(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('post', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### put()

```php
public function put(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a route that is only available to PUT requests.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1076 - 1081)</small></summary>

```php
public function put(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('put', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### delete()

```php
public function delete(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a route that is only available to DELETE requests.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1094 - 1099)</small></summary>

```php
public function delete(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('delete', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### head()

```php
public function head(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a route that is only available to HEAD requests.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1112 - 1117)</small></summary>

```php
public function head(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('head', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### patch()

```php
public function patch(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a route that is only available to PATCH requests.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1130 - 1135)</small></summary>

```php
public function patch(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('patch', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### options()

```php
public function options(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a route that is only available to OPTIONS requests.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1148 - 1153)</small></summary>

```php
public function options(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('options', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### cli()

```php
public function cli(string $from, $to, array $options = null) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies a route that is only available to command-line requests.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1166 - 1171)</small></summary>

```php
public function cli(string $from, $to, array $options = null): RouteCollectionInterface
{
	$this->create('cli', $from, $to, $options);

	return $this;
}
```

</details>


<hr>

#### environment()

```php
public function environment(string $env, \Closure $callback) : RouteCollectionInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Limits the routes to a specified ENVIRONMENT or they won't run.
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
<td><code>$env</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$callback</code></td>
<td><em>\Closure
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\RouteCollectionInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (1183 - 1191)</small></summary>

```php
public function environment(string $env, \Closure $callback): RouteCollectionInterface
{
	if (ENVIRONMENT === $env)
	{
		$callback($this);
	}

	return $this;
}
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
Attempts to look up a route based on its destination.
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
<summary><small>Source: 54 lines (1213 - 1266)</small></summary>

```php
public function reverseRoute(string $search, ...$params)
{
	// Named routes get higher priority.
	foreach ($this->routes as $collection)
	{
		if (array_key_exists($search, $collection))
		{
			$route = $this->fillRouteParams(key($collection[$search]['route']), $params);
			return $this->localizeRoute($route);
		}
	}

	// If it's not a named route, then loop over
	// all routes to find a match.
	foreach ($this->routes as $collection)
	{
		foreach ($collection as $route)
		{
			$from = key($route['route']);
			$to   = $route['route'][$from];

			// ignore closures
			if (! is_string($to))
			{
				continue;
			}

			// Lose any namespace slash at beginning of strings
			// to ensure more consistent match.
			$to     = ltrim($to, '\\');
			$search = ltrim($search, '\\');

			// If there's any chance of a match, then it will
			// be with $search at the beginning of the $to string.
			if (strpos($to, $search) !== 0)
			{
				continue;
			}

			// Ensure that the number of $params given here
			// matches the number of back-references in the route
			if (substr_count($to, '$') !== count($params))
			{
				continue;
			}

			$route = $this->fillRouteParams($from, $params);
			return $this->localizeRoute($route);
		}
	}

	// If we're still here, then we did not find a match.
	return false;
}
```

</details>


<hr>

#### localizeRoute()

```php
protected function localizeRoute(string $route) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replaces the {locale} tag with the current application locale
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
<td><code>$route</code></td>
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
<summary><small>Source: 4 lines (1277 - 1280)</small></summary>

```php
protected function localizeRoute(string $route) :string
{
	return strtr($route, ['{locale}' => Services::request()->getLocale()]);
}
```

</details>


<hr>

#### isFiltered()

```php
public function isFiltered(string $search) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks a route (using the "from") to see if it's filtered or not.
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
<summary><small>Source: 4 lines (1291 - 1294)</small></summary>

```php
public function isFiltered(string $search): bool
{
	return isset($this->routesOptions[$search]['filter']);
}
```

</details>


<hr>

#### getFilterForRoute()

```php
public function getFilterForRoute(string $search) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the filter that should be applied for a single route, along
with any parameters it might have. Parameters are found by splitting
the parameter name on a colon to separate the filter name from the parameter list,
and the splitting the result on commas. So:
</td></tr>
</table>

<table>
<tr><td>
'role:admin,manager'

has a filter of "role", with parameters of ['admin', 'manager'].
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
<summary><small>Source: 9 lines (1312 - 1320)</small></summary>

```php
public function getFilterForRoute(string $search): string
{
	if (! $this->isFiltered($search))
	{
		return '';
	}

	return $this->routesOptions[$search]['filter'];
}
```

</details>


<hr>

#### fillRouteParams()

```php
protected function fillRouteParams(string $from, array $params = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Given a
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
<td><code>$params</code></td>
<td><em>array<br>null
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
<td>\CodeIgniter\Router\Exceptions\RouterException
</td>
</tr>
</table>



<details>
<summary><small>Source: 27 lines (1333 - 1359)</small></summary>

```php
protected function fillRouteParams(string $from, array $params = null): string
{
	// Find all of our back-references in the original route
	preg_match_all('/\(([^)]+)\)/', $from, $matches);

	if (empty($matches[0]))
	{
		return '/' . ltrim($from, '/');
	}

	// Build our resulting string, inserting the $params in
	// the appropriate places.
	foreach ($matches[0] as $index => $pattern)
	{
		if (! preg_match('#^' . $pattern . '$#u', $params[$index]))
		{
			throw RouterException::forInvalidParameterType();
		}

		// Ensure that the param we're inserting matches
		// the expected param type.
		$pos  = strpos($from, $pattern);
		$from = substr_replace($from, $params[$index], $pos, strlen($pattern));
	}

	return '/' . ltrim($from, '/');
}
```

</details>


<hr>

#### create()

```php
protected function create(string $verb, string $from, $to, array $options = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does the heavy lifting of creating an actual route. You must specify
the request method(s) that this route will work for. They can be separated
by a pipe character "|" if there is more than one.
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
<td><code>$verb</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$from</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$to</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$options</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 108 lines (1373 - 1480)</small></summary>

```php
protected function create(string $verb, string $from, $to, array $options = null)
{
	$overwrite = false;
	$prefix    = is_null($this->group) ? '' : $this->group . '/';

	$from = filter_var($prefix . $from, FILTER_SANITIZE_STRING);

	// While we want to add a route within a group of '/',
	// it doesn't work with matching, so remove them...
	if ($from !== '/')
	{
		$from = trim($from, '/');
	}

	$options = array_merge((array) $this->currentOptions, (array) $options);

	// Hostname limiting?
	if (! empty($options['hostname']))
	{
		// @todo determine if there's a way to whitelist hosts?
		if (isset($_SERVER['HTTP_HOST']) && strtolower($_SERVER['HTTP_HOST']) !== strtolower($options['hostname']))
		{
			return;
		}

		$overwrite = true;
	}

	// Limiting to subdomains?
	else if (! empty($options['subdomain']))
	{
		// If we don't match the current subdomain, then
		// we don't need to add the route.
		if (! $this->checkSubdomains($options['subdomain']))
		{
			return;
		}

		$overwrite = true;
	}

	// Are we offsetting the binds?
	// If so, take care of them here in one
	// fell swoop.
	if (isset($options['offset']) && is_string($to))
	{
		// Get a constant string to work with.
		$to = preg_replace('/(\$\d+)/', '$X', $to);

		for ($i = (int) $options['offset'] + 1; $i < (int) $options['offset'] + 7; $i ++)
		{
			$to = preg_replace_callback(
					'/\$X/', function ($m) use ($i) {
						return '$' . $i;
					}, $to, 1
			);
		}
	}

	// Replace our regex pattern placeholders with the actual thing
	// so that the Router doesn't need to know about any of this.
	foreach ($this->placeholders as $tag => $pattern)
	{
		$from = str_ireplace(':' . $tag, $pattern, $from);
	}

	//If is redirect, No processing
	if (! isset($options['redirect']))
	{
		if (is_string($to))
		{
			// If no namespace found, add the default namespace
			if (strpos($to, '\\') === false || strpos($to, '\\') > 0)
			{
				$namespace = $options['namespace'] ?? $this->defaultNamespace;
				$to        = trim($namespace, '\\') . '\\' . $to;
			}

			// Always ensure that we escape our namespace so we're not pointing to
			// \CodeIgniter\Routes\Controller::method.
			$to = '\\' . ltrim($to, '\\');
		}
	}

	$name = $options['as'] ?? $from;

	// Don't overwrite any existing 'froms' so that auto-discovered routes
	// do not overwrite any app/Config/Routes settings. The app
	// routes should always be the "source of truth".
	// this works only because discovered routes are added just prior
	// to attempting to route the request.
	if (isset($this->routes[$verb][$name]) && ! $overwrite)
	{
		return;
	}

	$this->routes[$verb][$name] = [
		'route' => [$from => $to],
	];

	$this->routesOptions[$from] = $options;

	// Is this a redirect?
	if (isset($options['redirect']) && is_numeric($options['redirect']))
	{
		$this->routes['*'][$name]['redirect'] = $options['redirect'];
	}
}
```

</details>


<hr>

#### checkSubdomains()

```php
private function checkSubdomains($subdomains) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Compares the subdomain(s) passed in against the current subdomain
on this page request.
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
<td><code>$subdomains</code></td>
<td><em>mixed
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
<summary><small>Source: 27 lines (1492 - 1518)</small></summary>

```php
private function checkSubdomains($subdomains): bool
{
	// CLI calls can't be on subdomain.
	if (! isset($_SERVER['HTTP_HOST']))
	{
		return false;
	}

	if (is_null($this->currentSubdomain))
	{
		$this->currentSubdomain = $this->determineCurrentSubdomain();
	}

	if (! is_array($subdomains))
	{
		$subdomains = [$subdomains];
	}

	// Routes can be limited to any sub-domain. In that case, though,
	// it does require a sub-domain to be present.
	if (! empty($this->currentSubdomain) && in_array('*', $subdomains))
	{
		return true;
	}

	return in_array($this->currentSubdomain, $subdomains, true);
}
```

</details>


<hr>

#### determineCurrentSubdomain()

```php
private function determineCurrentSubdomain()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Examines the HTTP_HOST to get a best match for the subdomain. It
won't be perfect, but should work for our needs.
</td></tr>
</table>

<table>
<tr><td>
It's especially not perfect since it's possible to register a domain
with a period (.) as part of the domain name.
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
<summary><small>Source: 38 lines (1531 - 1568)</small></summary>

```php
private function determineCurrentSubdomain()
{
	// We have to ensure that a scheme exists
	// on the URL else parse_url will mis-interpret
	// 'host' as the 'path'.
	$url = $_SERVER['HTTP_HOST'];
	if (strpos($url, 'http') !== 0)
	{
		$url = 'http://' . $url;
	}

	$parsedUrl = parse_url($url);

	$host = explode('.', $parsedUrl['host']);

	if ($host[0] === 'www')
	{
		unset($host[0]);
	}

	// Get rid of any domains, which will be the last
	unset($host[count($host)]);

	// Account for .co.uk, .co.nz, etc. domains
	if (end($host) === 'co')
	{
		$host = array_slice($host, 0, -1);
	}

	// If we only have 1 part left, then we don't have a sub-domain.
	if (count($host) === 1)
	{
		// Set it to false so we don't make it back here again.
		return false;
	}

	return array_shift($host);
}
```

</details>


<hr>

#### resetRoutes()

```php
public function resetRoutes()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reset the routes, so that a FeatureTestCase can provide the
explicit ones needed for it.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 8 lines (1576 - 1583)</small></summary>

```php
public function resetRoutes()
{
	$this->routes = ['*' => []];
	foreach ($this->defaultHTTPMethods as $verb)
	{
		$this->routes[$verb] = [];
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Router/RouteCollection.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RouterException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollectionInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>