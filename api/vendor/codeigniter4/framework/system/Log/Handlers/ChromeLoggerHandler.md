


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Log/Handlers/ChromeLoggerHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/BaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/FileHandler.md">next</a></td>
</tr>
</table>







# CodeIgniter\Log\Handlers 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Log\Handlers</td></tr>
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
<td>framework/system/Log/Handlers/ChromeLoggerHandler.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/BaseHandler.md">CodeIgniter\Log\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/ChromeLoggerHandler.md">CodeIgniter\Log\Handlers\ChromeLoggerHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/FileHandler.md">CodeIgniter\Log\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/HandlerInterface.md">CodeIgniter\Log\Handlers\HandlerInterface</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/ResponseInterface.md"><strong>CodeIgniter\HTTP\ResponseInterface</strong></a>
</td>
<td>ResponseInterface</td>
</tr>
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
</table>



 
## CodeIgniter\Log\Handlers\ChromeLoggerHandler

<table style="text-align:left">
<tr><th>Class</th><td>ChromeLoggerHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Log\Handlers\ChromeLoggerHandler</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/BaseHandler.md">CodeIgniter\Log\Handlers\BaseHandler</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/HandlerInterface.md">CodeIgniter\Log\Handlers\HandlerInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class ChromeLoggerHandler
</td></tr>
</table>

<table>
<tr><td>
Allows for logging items to the Chrome console for debugging.
Requires the ChromeLogger extension installed in your browser.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Log\Handlers
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
<th><a href="#VERSION"><strong>VERSION</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>

<tr>
<th><a href="#backtraceLevel"><strong>backtraceLevel</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The number of track frames returned from the backtrace.</td>
</tr>
<tr>
<th><a href="#json"><strong>json</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The final data that is sent to the browser.</td>
</tr>
<tr>
<th><a href="#header"><strong>header</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The header used to pass the data.</td>
</tr>
<tr>
<th><a href="#levels"><strong>levels</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Maps the log levels to the ChromeLogger types.</td>
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
<th><a href="#handle"><strong>handle</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Handles logging the message.</td>
</tr>
<tr>
<th><a href="#format"><strong>format</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Converts the object to display nicely in the Chrome Logger UI.</td>
</tr>
<tr>
<th><a href="#sendLogs"><strong>sendLogs</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attaches the header and the content to the passed in request object.</td>
</tr>

</table>




### Class Constants


#### ::VERSION

```php
const VERSION = 1.0;
```






### Properties


<hr>

#### $backtraceLevel

```php
protected $backtraceLevel = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The number of track frames returned from the backtrace.
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

#### $json

```php
protected $json = [
	'version' => self::VERSION,
	'columns' => [
		'log',
		'backtrace',
		'type',
	],
	'rows'    => [],
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The final data that is sent to the browser.
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

#### $header

```php
protected $header = 'X-ChromeLogger-Data';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The header used to pass the data.
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

#### $levels

```php
protected $levels = [
	'emergency' => 'error',
	'alert'     => 'error',
	'critical'  => 'error',
	'error'     => 'error',
	'warning'   => 'warn',
	'notice'    => 'warn',
	'info'      => 'info',
	'debug'     => 'info',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Maps the log levels to the ChromeLogger types.
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

#### __construct()

```php
public function __construct(array $config = array())
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
<td><code>$config</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 8 lines (117 - 124)</small></summary>

```php
public function __construct(array $config = [])
{
	parent::__construct($config);

	$request = Services::request(null, true);

	$this->json['request_uri'] = (string) $request->uri;
}
```

</details>


<hr>

#### handle()

```php
public function handle($level, $message) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles logging the message.
</td></tr>
</table>

<table>
<tr><td>
If the handler returns false, then execution of handlers
will stop. Any handlers that have not run, yet, will not
be run.
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
<td><code>$level</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$message</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 33 lines (139 - 171)</small></summary>

```php
public function handle($level, $message): bool
{
	// Format our message
	$message = $this->format($message);

	// Generate Backtrace info
	$backtrace = debug_backtrace(false, $this->backtraceLevel);
	$backtrace = end($backtrace);

	$backtraceMessage = 'unknown';
	if (isset($backtrace['file']) && isset($backtrace['line']))
	{
		$backtraceMessage = $backtrace['file'] . ':' . $backtrace['line'];
	}

	// Default to 'log' type.
	$type = '';

	if (array_key_exists($level, $this->levels))
	{
		$type = $this->levels[$level];
	}

	$this->json['rows'][] = [
		[$message],
		$backtraceMessage,
		$type,
	];

	$this->sendLogs();

	return true;
}
```

</details>


<hr>

#### format()

```php
protected function format($object)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts the object to display nicely in the Chrome Logger UI.
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
<td><code>$object</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (182 - 195)</small></summary>

```php
protected function format($object)
{
	if (! is_object($object))
	{
		return $object;
	}

	// @todo Modify formatting of objects once we can view them in browser.
	$objectArray = (array) $object;

	$objectArray['___class_name'] = get_class($object);

	return $objectArray;
}
```

</details>


<hr>

#### sendLogs()

```php
public function sendLogs(ResponseInterface &$response = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attaches the header and the content to the passed in request object.
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
<td><code>$response</code></td>
<td><em>\ResponseInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 11 lines (204 - 214)</small></summary>

```php
public function sendLogs(ResponseInterface &$response = null)
{
	if (is_null($response))
	{
		$response = Services::response(null, true);
	}

	$data = base64_encode(utf8_encode(json_encode($this->json)));

	$response->setHeader($this->header, $data);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Log/Handlers/ChromeLoggerHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/BaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/FileHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:17**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>