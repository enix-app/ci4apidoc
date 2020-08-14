


 



<table>
<tr>
<td style="width:100%"><em>framework/system/CodeIgniter.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/WincacheHandler.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Commands/Cache/ClearCache.md">next</a></td>
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
<th>vendor</th>
<td>CodeIgniter
</td>
</tr>
<tr style="vertical-align:top;">
<th>package</th>
<td>codeigniter4/framework
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
<td><a href="https://opensource.org/licenses/MIT">https://opensource.org/licenses/MIT</a> MIT License
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com">https://codeigniter.com</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>since</th>
<td>
</td>
</tr>
<tr style="vertical-align:top;">
<th>filesource</th>
<td>framework/system/CodeIgniter.php
</td>
</tr>
</table>

 


 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>Closure</strong>
</td>
<td>Closure</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Debug/Timer.md"><strong>CodeIgniter\Debug\Timer</strong></a>
</td>
<td>Timer</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Events/Events.md"><strong>CodeIgniter\Events\Events</strong></a>
</td>
<td>Events</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Exceptions/PageNotFoundException.md"><strong>CodeIgniter\Exceptions\PageNotFoundException</strong></a>
</td>
<td>PageNotFoundException</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/CLIRequest.md"><strong>CodeIgniter\HTTP\CLIRequest</strong></a>
</td>
<td>CLIRequest</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/DownloadResponse.md"><strong>CodeIgniter\HTTP\DownloadResponse</strong></a>
</td>
<td>DownloadResponse</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/RedirectResponse.md"><strong>CodeIgniter\HTTP\RedirectResponse</strong></a>
</td>
<td>RedirectResponse</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/Request.md"><strong>CodeIgniter\HTTP\Request</strong></a>
</td>
<td>Request</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/Response.md"><strong>CodeIgniter\HTTP\Response</strong></a>
</td>
<td>Response</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/ResponseInterface.md"><strong>CodeIgniter\HTTP\ResponseInterface</strong></a>
</td>
<td>ResponseInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/URI.md"><strong>CodeIgniter\HTTP\URI</strong></a>
</td>
<td>URI</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RedirectException.md"><strong>CodeIgniter\Router\Exceptions\RedirectException</strong></a>
</td>
<td>RedirectException</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollectionInterface.md"><strong>CodeIgniter\Router\RouteCollectionInterface</strong></a>
</td>
<td>RouteCollectionInterface</td>
</tr>
<tr>
<td>
<strong>Config\Cache</strong>
</td>
<td>Cache</td>
</tr>
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
<tr>
<td>
<strong>Exception</strong>
</td>
<td>Exception</td>
</tr>
</table>



 
## CodeIgniter\CodeIgniter

<table style="text-align:left">
<tr><th>Class</th><td>CodeIgniter</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\CodeIgniter</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
This class is the core of the framework, and will analyse the
request, route it to a controller, and send back the response.
</td></tr>
</table>

<table>
<tr><td>
Of course, there are variations to that flow, but this is the brains.
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
<th><a href="#CI_VERSION"><strong>CI_VERSION</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>

<tr>
<th><a href="#startTime"><strong>startTime</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>App startup time.</td>
</tr>
<tr>
<th><a href="#totalTime"><strong>totalTime</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Total app execution time</td>
</tr>
<tr>
<th><a href="#config"><strong>config</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Main application configuration</td>
</tr>
<tr>
<th><a href="#benchmark"><strong>benchmark</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Timer instance.</td>
</tr>
<tr>
<th><a href="#request"><strong>request</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Current request.</td>
</tr>
<tr>
<th><a href="#response"><strong>response</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Current response.</td>
</tr>
<tr>
<th><a href="#router"><strong>router</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Router to use.</td>
</tr>
<tr>
<th><a href="#controller"><strong>controller</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Controller to use.</td>
</tr>
<tr>
<th><a href="#method"><strong>method</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Controller method to invoke.</td>
</tr>
<tr>
<th><a href="#output"><strong>output</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Output handler to use.</td>
</tr>
<tr>
<th><a href="#cacheTTL"><strong>cacheTTL</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Cache expiration time</td>
</tr>
<tr>
<th><a href="#path"><strong>path</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Request path to use.</td>
</tr>
<tr>
<th><a href="#useSafeOutput"><strong>useSafeOutput</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Should the Response instance &quot;pretend&quot;
to keep from setting headers/cookies/etc</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor.</td>
</tr>
<tr>
<th><a href="#initialize"><strong>initialize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Handles some basic app and environment setup.</td>
</tr>
<tr>
<th><a href="#initializeKint"><strong>initializeKint</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Initializes Kint</td>
</tr>
<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Launch the application!</td>
</tr>
<tr>
<th><a href="#useSafeOutput"><strong>useSafeOutput</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set our Response instance to &quot;pretend&quot; mode so that things like
cookies and headers are not actually sent, allowing PHP 7.2+ to
not complain when ini_set() function is used.</td>
</tr>
<tr>
<th><a href="#handleRequest"><strong>handleRequest</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Handles the main request logic and fires the controller.</td>
</tr>
<tr>
<th><a href="#detectEnvironment"><strong>detectEnvironment</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>You can load different configurations depending on your
current environment. Setting the environment also influences
things like logging and error reporting.</td>
</tr>
<tr>
<th><a href="#bootstrapEnvironment"><strong>bootstrapEnvironment</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Load any custom boot files based upon the current environment.</td>
</tr>
<tr>
<th><a href="#startBenchmark"><strong>startBenchmark</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Start the Benchmark</td>
</tr>
<tr>
<th><a href="#setRequest"><strong>setRequest</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets a Request object to be used for this request.</td>
</tr>
<tr>
<th><a href="#getRequestObject"><strong>getRequestObject</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get our Request object, (either IncomingRequest or CLIRequest)
and set the server protocol based on the information provided
by the server.</td>
</tr>
<tr>
<th><a href="#getResponseObject"><strong>getResponseObject</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get our Response object, and set some default values, including
the HTTP protocol version and a default successful response.</td>
</tr>
<tr>
<th><a href="#forceSecureAccess"><strong>forceSecureAccess</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Force Secure Site Access? If the config value &#039;forceGlobalSecureRequests&#039;
is true, will enforce that all requests to this site are made through
HTTPS. Will redirect the user to the current page with HTTPS, as well
as set the HTTP Strict Transport Security header for those browsers
that support it.</td>
</tr>
<tr>
<th><a href="#displayCache"><strong>displayCache</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines if a response has been cached for the given URI.</td>
</tr>
<tr>
<th><a href="#cache"><strong>cache</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Tells the app that the final output should be cached.</td>
</tr>
<tr>
<th><a href="#cachePage"><strong>cachePage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Caches the full response from the current request. Used for
full-page caching for very high performance.</td>
</tr>
<tr>
<th><a href="#getPerformanceStats"><strong>getPerformanceStats</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an array with our basic performance stats collected.</td>
</tr>
<tr>
<th><a href="#generateCacheName"><strong>generateCacheName</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Generates the cache name to use for our full-page caching.</td>
</tr>
<tr>
<th><a href="#displayPerformanceMetrics"><strong>displayPerformanceMetrics</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Replaces the memory_usage and elapsed_time tags.</td>
</tr>
<tr>
<th><a href="#tryToRouteIt"><strong>tryToRouteIt</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Try to Route It - As it sounds like, works with the router to
match a route against the current URI. If the route is a
&quot;redirect route&quot;, will also handle the redirect.</td>
</tr>
<tr>
<th><a href="#determinePath"><strong>determinePath</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Determines the path to use for us to try to route to, based
on user input (setPath), or the CLI/IncomingRequest path.</td>
</tr>
<tr>
<th><a href="#setPath"><strong>setPath</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows the request path to be set from outside the class,
instead of relying on CLIRequest or IncomingRequest for the path.</td>
</tr>
<tr>
<th><a href="#startController"><strong>startController</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Now that everything has been setup, this method attempts to run the
controller method and make the script go. If it&#039;s not able to, will
show the appropriate Page Not Found error.</td>
</tr>
<tr>
<th><a href="#createController"><strong>createController</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Instantiates the controller class.</td>
</tr>
<tr>
<th><a href="#runController"><strong>runController</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Runs the controller, allowing for _remap methods to function.</td>
</tr>
<tr>
<th><a href="#display404errors"><strong>display404errors</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Displays a 404 Page Not Found error. If set, will try to
call the 404Override controller/method that was set in routing config.</td>
</tr>
<tr>
<th><a href="#gatherOutput"><strong>gatherOutput</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Gathers the script output from the buffer, replaces some execution
time tag in the output and displays the debug toolbar, if required.</td>
</tr>
<tr>
<th><a href="#storePreviousURL"><strong>storePreviousURL</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>If we have a session object to use, store the current URI
as the previous URI. This is called just prior to sending the
response to the client, and will make it available next request.</td>
</tr>
<tr>
<th><a href="#spoofRequestMethod"><strong>spoofRequestMethod</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Modifies the Request Object to use a different method if a POST
variable called _method is found.</td>
</tr>
<tr>
<th><a href="#sendResponse"><strong>sendResponse</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Sends the output of this request back to the client.</td>
</tr>
<tr>
<th><a href="#callExit"><strong>callExit</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Exits the application, setting the exit code for CLI-based applications
that might be watching.</td>
</tr>

</table>




### Class Constants


#### ::CI_VERSION

```php
const CI_VERSION = '4.0.4';
```






### Properties


<hr>

#### $startTime

```php
protected $startTime;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
App startup time.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>mixed
</td>
</tr>
</table>


<hr>

#### $totalTime

```php
protected $totalTime;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Total app execution time
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>float
</td>
</tr>
</table>


<hr>

#### $config

```php
protected $config;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Main application configuration
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Config\App
</td>
</tr>
</table>


<hr>

#### $benchmark

```php
protected $benchmark;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Timer instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Timer
</td>
</tr>
</table>


<hr>

#### $request

```php
protected $request;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Current request.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\HTTP\Request<br>\HTTP\IncomingRequest<br>\CLIRequest
</td>
</tr>
</table>


<hr>

#### $response

```php
protected $response;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Current response.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\HTTP\ResponseInterface
</td>
</tr>
</table>


<hr>

#### $router

```php
protected $router;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Router to use.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Router\Router
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
Controller to use.
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

#### $method

```php
protected $method;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Controller method to invoke.
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

#### $output

```php
protected $output;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Output handler to use.
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

#### $cacheTTL

```php
protected static $cacheTTL = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cache expiration time
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $path

```php
protected $path;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Request path to use.
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

#### $useSafeOutput

```php
protected $useSafeOutput = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Should the Response instance "pretend"
to keep from setting headers/cookies/etc
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







### Methods


<hr>

#### __construct()

```php
public function __construct($config)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor.
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
<td><code>$config</code></td>
<td><em>\type
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 5 lines (172 - 176)</small></summary>

```php
public function __construct($config)
{
	$this->startTime = microtime(true);
	$this->config    = $config;
}
```

</details>


<hr>

#### initialize()

```php
public function initialize()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles some basic app and environment setup.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 25 lines (183 - 207)</small></summary>

```php
public function initialize()
{
	// Set default locale on the server
	locale_set_default($this->config->defaultLocale ?? 'en');

	// Set default timezone on the server
	date_default_timezone_set($this->config->appTimezone ?? 'UTC');

	// Define environment variables
	$this->detectEnvironment();
	$this->bootstrapEnvironment();

	// Setup Exception Handling
	Services::exceptions()
			->initialize();

	$this->initializeKint();

	if (! CI_DEBUG)
	{
		// @codeCoverageIgnoreStart
		\Kint::$enabled_mode = false;
		// @codeCoverageIgnoreEnd
	}
}
```

</details>


<hr>

#### initializeKint()

```php
protected function initializeKint()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Initializes Kint
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 52 lines (214 - 265)</small></summary>

```php
protected function initializeKint()
{
	// If we have KINT_DIR it means it's already loaded via composer
	if (! defined('KINT_DIR'))
	{
		spl_autoload_register(function ($class) {
			$class = explode('\\', $class);

			if ('Kint' !== array_shift($class))
			{
				return;
			}

			$file = SYSTEMPATH . 'ThirdParty/Kint/' . implode('/', $class) . '.php';

			file_exists($file) && require_once $file;
		});

		require_once SYSTEMPATH . 'ThirdParty/Kint/init.php';
	}

	/**
	 * Config\Kint
	 */
	$config = config('Config\Kint');

	\Kint::$max_depth           = $config->maxDepth;
	\Kint::$display_called_from = $config->displayCalledFrom;
	\Kint::$expanded            = $config->expanded;

	if (! empty($config->plugins) && is_array($config->plugins))
	{
		\Kint::$plugins = $config->plugins;
	}

	\Kint\Renderer\RichRenderer::$theme  = $config->richTheme;
	\Kint\Renderer\RichRenderer::$folder = $config->richFolder;
	\Kint\Renderer\RichRenderer::$sort   = $config->richSort;
	if (! empty($config->richObjectPlugins) && is_array($config->richObjectPlugins))
	{
		\Kint\Renderer\RichRenderer::$object_plugins = $config->richObjectPlugins;
	}
	if (! empty($config->richTabPlugins) && is_array($config->richTabPlugins))
	{
		\Kint\Renderer\RichRenderer::$tab_plugins = $config->richTabPlugins;
	}

	\Kint\Renderer\CliRenderer::$cli_colors         = $config->cliColors;
	\Kint\Renderer\CliRenderer::$force_utf8         = $config->cliForceUTF8;
	\Kint\Renderer\CliRenderer::$detect_width       = $config->cliDetectWidth;
	\Kint\Renderer\CliRenderer::$min_terminal_width = $config->cliMinWidth;
}
```

</details>


<hr>

#### run()

```php
public function run(RouteCollectionInterface $routes = null, bool $returnResponse = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Launch the application!
</td></tr>
</table>

<table>
<tr><td>
This is "the loop" if you will. The main entry point into the script
that gets the required class instances, fires off the filters,
tries to route the response, loads the controller and generally
makes all of the pieces work together.
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
<td><em>\CodeIgniter\Router\RouteCollectionInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$returnResponse</code></td>
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
<td>bool<br>\CodeIgniter\HTTP\RequestInterface<br>\CodeIgniter\HTTP\Response<br>\CodeIgniter\HTTP\ResponseInterface<br>mixed
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
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 49 lines (284 - 332)</small></summary>

```php
public function run(RouteCollectionInterface $routes = null, bool $returnResponse = false)
{
	$this->startBenchmark();

	$this->getRequestObject();
	$this->getResponseObject();

	$this->forceSecureAccess();

	$this->spoofRequestMethod();

	Events::trigger('pre_system');

	// Check for a cached page. Execution will stop
	// if the page has been cached.
	$cacheConfig = new Cache();
	$response    = $this->displayCache($cacheConfig);
	if ($response instanceof ResponseInterface)
	{
		if ($returnResponse)
		{
			return $response;
		}

		$this->response->pretend($this->useSafeOutput)->send();
		$this->callExit(EXIT_SUCCESS);
	}

	try
	{
		return $this->handleRequest($routes, $cacheConfig, $returnResponse);
	}
	catch (RedirectException $e)
	{
		$logger = Services::logger();
		$logger->info('REDIRECTED ROUTE at ' . $e->getMessage());

		// If the route is a 'redirect' route, it throws
		// the exception with the $to as the message
		$this->response->redirect(base_url($e->getMessage()), 'auto', $e->getCode());
		$this->sendResponse();

		$this->callExit(EXIT_SUCCESS);
	}
	catch (PageNotFoundException $e)
	{
		$this->display404errors($e);
	}
}
```

</details>


<hr>

#### useSafeOutput()

```php
public function useSafeOutput(bool $safe = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set our Response instance to "pretend" mode so that things like
cookies and headers are not actually sent, allowing PHP 7.2+ to
not complain when ini_set() function is used.
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
<td><code>$safe</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (345 - 350)</small></summary>

```php
public function useSafeOutput(bool $safe = true)
{
	$this->useSafeOutput = $safe;

	return $this;
}
```

</details>


<hr>

#### handleRequest()

```php
protected function handleRequest(RouteCollectionInterface $routes = null, $cacheConfig, bool $returnResponse = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles the main request logic and fires the controller.
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
<td><em>\CodeIgniter\Router\RouteCollectionInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$cacheConfig</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$returnResponse</code></td>
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
<td>\CodeIgniter\HTTP\RequestInterface<br>\CodeIgniter\HTTP\Response<br>\CodeIgniter\HTTP\ResponseInterface<br>mixed
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
<summary><small>Source: 96 lines (364 - 459)</small></summary>

```php
protected function handleRequest(RouteCollectionInterface $routes = null, $cacheConfig, bool $returnResponse = false)
{
	$routeFilter = $this->tryToRouteIt($routes);

	// Run "before" filters
	$filters = Services::filters();

	// If any filters were specified within the routes file,
	// we need to ensure it's active for the current request
	if (! is_null($routeFilter))
	{
		$filters->enableFilter($routeFilter, 'before');
		$filters->enableFilter($routeFilter, 'after');
	}

	$uri = $this->request instanceof CLIRequest ? $this->request->getPath() : $this->request->uri->getPath();

	// Never run filters when running through Spark cli
	if (! defined('SPARKED'))
	{
		$possibleRedirect = $filters->run($uri, 'before');
		if ($possibleRedirect instanceof RedirectResponse)
		{
			return $possibleRedirect->send();
		}
		// If a Response instance is returned, the Response will be sent back to the client and script execution will stop
		if ($possibleRedirect instanceof ResponseInterface)
		{
			return $possibleRedirect->send();
		}
	}

	$returned = $this->startController();

	// Closure controller has run in startController().
	if (! is_callable($this->controller))
	{
		$controller = $this->createController();

		// Is there a "post_controller_constructor" event?
		Events::trigger('post_controller_constructor');

		$returned = $this->runController($controller);
	}
	else
	{
		$this->benchmark->stop('controller_constructor');
		$this->benchmark->stop('controller');
	}

	// If $returned is a string, then the controller output something,
	// probably a view, instead of echoing it directly. Send it along
	// so it can be used with the output.
	$this->gatherOutput($cacheConfig, $returned);

	// Never run filters when running through Spark cli
	if (! defined('SPARKED'))
	{
		$filters->setResponse($this->response);
		// Run "after" filters
		$response = $filters->run($uri, 'after');
	}
	else
	{
		$response = $this->response;

		// Set response code for CLI command failures
		if (is_numeric($returned) || $returned === false)
		{
			$response->setStatusCode(400);
		}
	}

	if ($response instanceof Response)
	{
		$this->response = $response;
	}

	// Save our current URI as the previous URI in the session
	// for safer, more accurate use with `previous_url()` helper function.
	$this->storePreviousURL((string)current_url(true));

	unset($uri);

	if (! $returnResponse)
	{
		$this->sendResponse();
	}

	//--------------------------------------------------------------------
	// Is there a post-system event?
	//--------------------------------------------------------------------
	Events::trigger('post_system');

	return $this->response;
}
```

</details>


<hr>

#### detectEnvironment()

```php
protected function detectEnvironment()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
You can load different configurations depending on your
current environment. Setting the environment also influences
things like logging and error reporting.
</td></tr>
</table>

<table>
<tr><td>
This can be set to anything, but default usage is:

development
testing
production
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 16 lines (474 - 489)</small></summary>

```php
protected function detectEnvironment()
{
	// Make sure ENVIRONMENT isn't already set by other means.
	if (! defined('ENVIRONMENT'))
	{
		// running under Continuous Integration server?
		if (getenv('CI') !== false)
		{
			define('ENVIRONMENT', 'testing');
		}
		else
		{
			define('ENVIRONMENT', $_SERVER['CI_ENVIRONMENT'] ?? 'production');
		}
	}
}
```

</details>


<hr>

#### bootstrapEnvironment()

```php
protected function bootstrapEnvironment()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Load any custom boot files based upon the current environment.
</td></tr>
</table>

<table>
<tr><td>
If no boot file exists, we shouldn't continue because something
is wrong. At the very least, they should have error reporting setup.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 15 lines (499 - 513)</small></summary>

```php
protected function bootstrapEnvironment()
{
	if (is_file(APPPATH . 'Config/Boot/' . ENVIRONMENT . '.php'))
	{
		require_once APPPATH . 'Config/Boot/' . ENVIRONMENT . '.php';
	}
	else
	{
		// @codeCoverageIgnoreStart
		header('HTTP/1.1 503 Service Unavailable.', true, 503);
		echo 'The application environment is not set correctly.';
		exit(1); // EXIT_ERROR
		// @codeCoverageIgnoreEnd
	}
}
```

</details>


<hr>

#### startBenchmark()

```php
protected function startBenchmark()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Start the Benchmark
</td></tr>
</table>

<table>
<tr><td>
The timer is used to display total script execution both in the
debug toolbar, and potentially on the displayed page.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 8 lines (523 - 530)</small></summary>

```php
protected function startBenchmark()
{
	$this->startTime = microtime(true);

	$this->benchmark = Services::timer();
	$this->benchmark->start('total_execution', $this->startTime);
	$this->benchmark->start('bootstrap');
}
```

</details>


<hr>

#### setRequest()

```php
public function setRequest(Request $request)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets a Request object to be used for this request.
</td></tr>
</table>

<table>
<tr><td>
Used when running certain tests.
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
<td><code>$request</code></td>
<td><em>\CodeIgniter\HTTP\Request
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\CodeIgniter
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (542 - 547)</small></summary>

```php
public function setRequest(Request $request)
{
	$this->request = $request;

	return $this;
}
```

</details>


<hr>

#### getRequestObject()

```php
protected function getRequestObject()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get our Request object, (either IncomingRequest or CLIRequest)
and set the server protocol based on the information provided
by the server.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 20 lines (556 - 575)</small></summary>

```php
protected function getRequestObject()
{
	if ($this->request instanceof Request)
	{
		return;
	}

	if (is_cli() && ENVIRONMENT !== 'testing')
	{
		// @codeCoverageIgnoreStart
		$this->request = Services::clirequest($this->config);
		// @codeCoverageIgnoreEnd
	}
	else
	{
		$this->request = Services::request($this->config);
		// guess at protocol if needed
		$this->request->setProtocolVersion($_SERVER['SERVER_PROTOCOL'] ?? 'HTTP/1.1');
	}
}
```

</details>


<hr>

#### getResponseObject()

```php
protected function getResponseObject()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get our Response object, and set some default values, including
the HTTP protocol version and a default successful response.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 12 lines (583 - 594)</small></summary>

```php
protected function getResponseObject()
{
	$this->response = Services::response($this->config);

	if (! is_cli() || ENVIRONMENT === 'testing')
	{
		$this->response->setProtocolVersion($this->request->getProtocolVersion());
	}

	// Assume success until proven otherwise.
	$this->response->setStatusCode(200);
}
```

</details>


<hr>

#### forceSecureAccess()

```php
protected function forceSecureAccess($duration = 31536000)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Force Secure Site Access? If the config value 'forceGlobalSecureRequests'
is true, will enforce that all requests to this site are made through
HTTPS. Will redirect the user to the current page with HTTPS, as well
as set the HTTP Strict Transport Security header for those browsers
that support it.
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
<td><code>$duration</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>How long the Strict Transport Security
should be enforced for this URL.</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (608 - 616)</small></summary>

```php
protected function forceSecureAccess($duration = 31536000)
{
	if ($this->config->forceGlobalSecureRequests !== true)
	{
		return;
	}

	force_https($duration, $this->request, $this->response);
}
```

</details>


<hr>

#### displayCache()

```php
public function displayCache($config)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines if a response has been cached for the given URI.
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
<td><code>$config</code></td>
<td><em>\Config\Cache
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool<br>\CodeIgniter\HTTP\ResponseInterface
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 33 lines (629 - 661)</small></summary>

```php
public function displayCache($config)
{
	if ($cachedResponse = cache()->get($this->generateCacheName($config)))
	{
		$cachedResponse = unserialize($cachedResponse);
		if (! is_array($cachedResponse) || ! isset($cachedResponse['output']) || ! isset($cachedResponse['headers']))
		{
			throw new Exception('Error unserializing page cache');
		}

		$headers = $cachedResponse['headers'];
		$output  = $cachedResponse['output'];

		// Clear all default headers
		foreach ($this->response->getHeaders() as $key => $val)
		{
			$this->response->removeHeader($key);
		}

		// Set cached headers
		foreach ($headers as $name => $value)
		{
			$this->response->setHeader($name, $value);
		}

		$output = $this->displayPerformanceMetrics($output);
		$this->response->setBody($output);

		return $this->response;
	}

	return false;
}
```

</details>


<hr>

#### cache()

```php
public static function cache(int $time)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Tells the app that the final output should be cached.
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
<td><code>$time</code></td>
<td><em>int
</em></td>
<td>false</td>
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
<summary><small>Source: 4 lines (672 - 675)</small></summary>

```php
public static function cache(int $time)
{
	static::$cacheTTL = $time;
}
```

</details>


<hr>

#### cachePage()

```php
public function cachePage(Cache $config)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Caches the full response from the current request. Used for
full-page caching for very high performance.
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
<td><code>$config</code></td>
<td><em>\Config\Cache
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
<summary><small>Source: 12 lines (687 - 698)</small></summary>

```php
public function cachePage(Cache $config)
{
	$headers = [];
	foreach ($this->response->getHeaders() as $header)
	{
		$headers[$header->getName()] = $header->getValueLine();
	}

	return cache()->save(
					$this->generateCacheName($config), serialize(['headers' => $headers, 'output' => $this->output]), static::$cacheTTL
	);
}
```

</details>


<hr>

#### getPerformanceStats()

```php
public function getPerformanceStats() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array with our basic performance stats collected.
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





<details>
<summary><small>Source: 7 lines (707 - 713)</small></summary>

```php
public function getPerformanceStats(): array
{
	return [
		'startTime' => $this->startTime,
		'totalTime' => $this->totalTime,
	];
}
```

</details>


<hr>

#### generateCacheName()

```php
protected function generateCacheName($config) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates the cache name to use for our full-page caching.
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
<td><code>$config</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 24 lines (724 - 747)</small></summary>

```php
protected function generateCacheName($config): string
{
	if (get_class($this->request) === CLIRequest::class)
	{
		return md5($this->request->getPath());
	}

	$uri = $this->request->uri;

	if ($config->cacheQueryString)
	{
		$name = URI::createURIString(
						$uri->getScheme(), $uri->getAuthority(), $uri->getPath(), $uri->getQuery()
		);
	}
	else
	{
		$name = URI::createURIString(
						$uri->getScheme(), $uri->getAuthority(), $uri->getPath()
		);
	}

	return md5($name);
}
```

</details>


<hr>

#### displayPerformanceMetrics()

```php
public function displayPerformanceMetrics(string $output) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replaces the memory_usage and elapsed_time tags.
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
<td><code>$output</code></td>
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
<summary><small>Source: 6 lines (758 - 763)</small></summary>

```php
public function displayPerformanceMetrics(string $output): string
{
	$this->totalTime = $this->benchmark->getElapsedTime('total_execution');

	return str_replace('{elapsed_time}', $this->totalTime, $output);
}
```

</details>


<hr>

#### tryToRouteIt()

```php
protected function tryToRouteIt(RouteCollectionInterface $routes = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Try to Route It - As it sounds like, works with the router to
match a route against the current URI. If the route is a
"redirect route", will also handle the redirect.
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
<td>An collection interface to use in place
of the config file.</td>
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
<td>\CodeIgniter\Router\Exceptions\RedirectException
</td>
</tr>
</table>



<details>
<summary><small>Source: 31 lines (778 - 808)</small></summary>

```php
protected function tryToRouteIt(RouteCollectionInterface $routes = null)
{
	if (empty($routes) || ! $routes instanceof RouteCollectionInterface)
	{
		require APPPATH . 'Config/Routes.php';
	}

	// $routes is defined in Config/Routes.php
	$this->router = Services::router($routes, $this->request);

	$path = $this->determinePath();

	$this->benchmark->stop('bootstrap');
	$this->benchmark->start('routing');

	ob_start();

	$this->controller = $this->router->handle($path);
	$this->method     = $this->router->methodName();

	// If a {locale} segment was matched in the final route,
	// then we need to set the correct locale on our Request.
	if ($this->router->hasLocale())
	{
		$this->request->setLocale($this->router->getLocale());
	}

	$this->benchmark->stop('routing');

	return $this->router->getFilter();
}
```

</details>


<hr>

#### determinePath()

```php
protected function determinePath()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines the path to use for us to try to route to, based
on user input (setPath), or the CLI/IncomingRequest path.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 9 lines (816 - 824)</small></summary>

```php
protected function determinePath()
{
	if (! empty($this->path))
	{
		return $this->path;
	}

	return (is_cli() && ! (ENVIRONMENT === 'testing')) ? $this->request->getPath() : $this->request->uri->getPath();
}
```

</details>


<hr>

#### setPath()

```php
public function setPath(string $path)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows the request path to be set from outside the class,
instead of relying on CLIRequest or IncomingRequest for the path.
</td></tr>
</table>

<table>
<tr><td>
This is primarily used by the Console.
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
<td><code>$path</code></td>
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
<summary><small>Source: 6 lines (838 - 843)</small></summary>

```php
public function setPath(string $path)
{
	$this->path = $path;

	return $this;
}
```

</details>


<hr>

#### startController()

```php
protected function startController()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Now that everything has been setup, this method attempts to run the
controller method and make the script go. If it's not able to, will
show the appropriate Page Not Found error.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 30 lines (852 - 881)</small></summary>

```php
protected function startController()
{
	$this->benchmark->start('controller');
	$this->benchmark->start('controller_constructor');

	// Is it routed to a Closure?
	if (is_object($this->controller) && (get_class($this->controller) === 'Closure'))
	{
		$controller = $this->controller;
		return $controller(...$this->router->params());
	}

	// No controller specified - we don't know what to do now.
	if (empty($this->controller))
	{
		throw PageNotFoundException::forEmptyController();
	}

	// Try to autoload the class
	if (! class_exists($this->controller, true) || $this->method[0] === '_')
	{
		throw PageNotFoundException::forControllerNotFound($this->controller, $this->method);
	}
	else if (! method_exists($this->controller, '_remap') &&
			! is_callable([$this->controller, $this->method], false)
	)
	{
		throw PageNotFoundException::forMethodNotFound($this->method);
	}
}
```

</details>


<hr>

#### createController()

```php
protected function createController()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instantiates the controller class.
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
<summary><small>Source: 9 lines (890 - 898)</small></summary>

```php
protected function createController()
{
	$class = new $this->controller();
	$class->initController($this->request, $this->response, Services::logger());

	$this->benchmark->stop('controller_constructor');

	return $class;
}
```

</details>


<hr>

#### runController()

```php
protected function runController($class)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs the controller, allowing for _remap methods to function.
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (909 - 926)</small></summary>

```php
protected function runController($class)
{
	// If this is a console request then use the input segments as parameters
	$params = defined('SPARKED') ? $this->request->getSegments() : $this->router->params();

	if (method_exists($class, '_remap'))
	{
		$output = $class->_remap($this->method, ...$params);
	}
	else
	{
		$output = $class->{$this->method}(...$params);
	}

	$this->benchmark->stop('controller');

	return $output;
}
```

</details>


<hr>

#### display404errors()

```php
protected function display404errors(PageNotFoundException $e)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Displays a 404 Page Not Found error. If set, will try to
call the 404Override controller/method that was set in routing config.
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
<td><code>$e</code></td>
<td><em>\PageNotFoundException
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 53 lines (936 - 988)</small></summary>

```php
protected function display404errors(PageNotFoundException $e)
{
	// Is there a 404 Override available?
	if ($override = $this->router->get404Override())
	{
		if ($override instanceof Closure)
		{
			echo $override($e->getMessage());
		}
		else if (is_array($override))
		{
			$this->benchmark->start('controller');
			$this->benchmark->start('controller_constructor');

			$this->controller = $override[0];
			$this->method     = $override[1];

			unset($override);

			$controller = $this->createController();
			$this->runController($controller);
		}

		$cacheConfig = new Cache();
		$this->gatherOutput($cacheConfig);
		$this->sendResponse();

		return;
	}

	// Display 404 Errors
	$this->response->setStatusCode($e->getCode());

	if (ENVIRONMENT !== 'testing')
	{
		// @codeCoverageIgnoreStart
		if (ob_get_level() > 0)
		{
			ob_end_flush();
		}
		// @codeCoverageIgnoreEnd
	}
	else
	{
		// When testing, one is for phpunit, another is for test case.
		if (ob_get_level() > 2)
		{
			ob_end_flush();
		}
	}

	throw PageNotFoundException::forPageNotFound(ENVIRONMENT !== 'production' || is_cli() ? $e->getMessage() : '');
}
```

</details>


<hr>

#### gatherOutput()

```php
protected function gatherOutput($cacheConfig = null, $returned = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gathers the script output from the buffer, replaces some execution
time tag in the output and displays the debug toolbar, if required.
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
<td><code>$cacheConfig</code></td>
<td><em>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$returned</code></td>
<td><em>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 43 lines (999 - 1041)</small></summary>

```php
protected function gatherOutput($cacheConfig = null, $returned = null)
{
	$this->output = ob_get_contents();
	// If buffering is not null.
	// Clean (erase) the output buffer and turn off output buffering
	if (ob_get_length())
	{
		ob_end_clean();
	}

	if ($returned instanceof DownloadResponse)
	{
		$this->response = $returned;
		return;
	}
	// If the controller returned a response object,
	// we need to grab the body from it so it can
	// be added to anything else that might have been
	// echoed already.
	// We also need to save the instance locally
	// so that any status code changes, etc, take place.
	if ($returned instanceof Response)
	{
		$this->response = $returned;
		$returned       = $returned->getBody();
	}

	if (is_string($returned))
	{
		$this->output .= $returned;
	}

	// Cache it without the performance metrics replaced
	// so that we can have live speed updates along the way.
	if (static::$cacheTTL > 0)
	{
		$this->cachePage($cacheConfig);
	}

	$this->output = $this->displayPerformanceMetrics($this->output);

	$this->response->setBody($this->output);
}
```

</details>


<hr>

#### storePreviousURL()

```php
public function storePreviousURL($uri)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
If we have a session object to use, store the current URI
as the previous URI. This is called just prior to sending the
response to the client, and will make it available next request.
</td></tr>
</table>

<table>
<tr><td>
This helps provider safer, more reliable previous_url() detection.
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
<td><em>\CodeIgniter\HTTP\URI
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 24 lines (1054 - 1077)</small></summary>

```php
public function storePreviousURL($uri)
{
	// Ignore CLI requests
	if (is_cli())
	{
		return;
	}
	// Ignore AJAX requests
	if (method_exists($this->request, 'isAJAX') && $this->request->isAJAX())
	{
		return;
	}

	// This is mainly needed during testing...
	if (is_string($uri))
	{
		$uri = new URI($uri);
	}

	if (isset($_SESSION))
	{
		$_SESSION['_ci_previous_url'] = (string) $uri;
	}
}
```

</details>


<hr>

#### spoofRequestMethod()

```php
public function spoofRequestMethod()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Modifies the Request Object to use a different method if a POST
variable called _method is found.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 17 lines (1085 - 1101)</small></summary>

```php
public function spoofRequestMethod()
{
	// Only works with POSTED forms
	if ($this->request->getMethod() !== 'post')
	{
		return;
	}

	$method = $this->request->getPost('_method');

	if (empty($method))
	{
		return;
	}

	$this->request = $this->request->setMethod($method);
}
```

</details>


<hr>

#### sendResponse()

```php
protected function sendResponse()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sends the output of this request back to the client.
</td></tr>
</table>

<table>
<tr><td>
This is what they've been waiting for!
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (1107 - 1110)</small></summary>

```php
protected function sendResponse()
{
	$this->response->pretend($this->useSafeOutput)->send();
}
```

</details>


<hr>

#### callExit()

```php
protected function callExit($code)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Exits the application, setting the exit code for CLI-based applications
that might be watching.
</td></tr>
</table>

<table>
<tr><td>
Made into a separate method so that it can be mocked during testing
without actually stopping script execution.
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
<td><code>$code</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 6 lines (1123 - 1128)</small></summary>

```php
protected function callExit($code)
{
	// @codeCoverageIgnoreStart
	exit($code);
	// @codeCoverageIgnoreEnd
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/CodeIgniter.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/WincacheHandler.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Commands/Cache/ClearCache.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>