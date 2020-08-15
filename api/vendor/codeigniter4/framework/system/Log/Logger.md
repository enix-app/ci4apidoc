


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Log/Logger.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/HandlerInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Model.md">next</a></td>
</tr>
</table>







# CodeIgniter\Log 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Log</td></tr>
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
<td>framework/system/Log/Logger.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Exceptions/LogException.md">CodeIgniter\Log\Exceptions\LogException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/BaseHandler.md">CodeIgniter\Log\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/ChromeLoggerHandler.md">CodeIgniter\Log\Handlers\ChromeLoggerHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/FileHandler.md">CodeIgniter\Log\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/HandlerInterface.md">CodeIgniter\Log\Handlers\HandlerInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Logger.md">CodeIgniter\Log\Logger</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Exceptions/LogException.md"><strong>CodeIgniter\Log\Exceptions\LogException</strong></a>
</td>
<td>LogException</td>
</tr>
<tr>
<td>
<strong>Psr\Log\LoggerInterface</strong>
</td>
<td>LoggerInterface</td>
</tr>
</table>



 
## CodeIgniter\Log\Logger

<table style="text-align:left">
<tr><th>Class</th><td>Logger</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Log\Logger</td></tr>
<tr><th>Implements</th>
<td>
<a href="">Psr\Log\LoggerInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The CodeIgntier Logger
</td></tr>
</table>

<table>
<tr><td>
The message MUST be a string or object implementing __toString().

The message MAY contain placeholders in the form: {foo} where foo
will be replaced by the context data in key "foo".

The context array can contain arbitrary data, the only assumption that
can be made by implementors is that if an Exception instance is given
to produce a stack trace, it MUST be in a key named "exception".
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Log
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
<th><a href="#logLevels"><strong>logLevels</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Used by the logThreshold Config setting to define
which errors to show.</td>
</tr>
<tr>
<th><a href="#loggableLevels"><strong>loggableLevels</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Array of levels to be logged.</td>
</tr>
<tr>
<th><a href="#filePermissions"><strong>filePermissions</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>File permissions</td>
</tr>
<tr>
<th><a href="#dateFormat"><strong>dateFormat</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Format of the timestamp for log files.</td>
</tr>
<tr>
<th><a href="#fileExt"><strong>fileExt</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Filename Extension</td>
</tr>
<tr>
<th><a href="#handlers"><strong>handlers</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Caches instances of the handlers.</td>
</tr>
<tr>
<th><a href="#handlerConfig"><strong>handlerConfig</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Holds the configuration for each handler.</td>
</tr>
<tr>
<th><a href="#logCache"><strong>logCache</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Caches logging calls for debugbar.</td>
</tr>
<tr>
<th><a href="#cacheLogs"><strong>cacheLogs</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Should we cache our logged items?</td>
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
<th><a href="#emergency"><strong>emergency</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>System is unusable.</td>
</tr>
<tr>
<th><a href="#alert"><strong>alert</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Action must be taken immediately.</td>
</tr>
<tr>
<th><a href="#critical"><strong>critical</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Critical conditions.</td>
</tr>
<tr>
<th><a href="#error"><strong>error</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runtime errors that do not require immediate action but should typically
be logged and monitored.</td>
</tr>
<tr>
<th><a href="#warning"><strong>warning</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Exceptional occurrences that are not errors.</td>
</tr>
<tr>
<th><a href="#notice"><strong>notice</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Normal but significant events.</td>
</tr>
<tr>
<th><a href="#info"><strong>info</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Interesting events.</td>
</tr>
<tr>
<th><a href="#debug"><strong>debug</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Detailed debug information.</td>
</tr>
<tr>
<th><a href="#log"><strong>log</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Logs with an arbitrary level.</td>
</tr>
<tr>
<th><a href="#interpolate"><strong>interpolate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Replaces any placeholders in the message with variables
from the context, as well as a few special items like:</td>
</tr>
<tr>
<th><a href="#determineFile"><strong>determineFile</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines the file and line that the logging call
was made from by analyzing the backtrace.</td>
</tr>
<tr>
<th><a href="#cleanFileNames"><strong>cleanFileNames</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Cleans the paths of filenames by replacing APPPATH, SYSTEMPATH, FCPATH
with the actual var. i.e.</td>
</tr>

</table>





### Properties


<hr>

#### $logLevels

```php
protected $logLevels = [
	'emergency' => 1,
	'alert'     => 2,
	'critical'  => 3,
	'error'     => 4,
	'warning'   => 5,
	'notice'    => 6,
	'info'      => 7,
	'debug'     => 8,
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used by the logThreshold Config setting to define
which errors to show.
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

#### $loggableLevels

```php
protected $loggableLevels = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Array of levels to be logged.
</td></tr>
</table>

<table>
<tr><td>
The rest will be ignored.
Set in Config/logger.php
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

#### $filePermissions

```php
protected $filePermissions = 0644;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
File permissions
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

#### $dateFormat

```php
protected $dateFormat = 'Y-m-d H:i:s';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Format of the timestamp for log files.
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

#### $fileExt

```php
protected $fileExt;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Filename Extension
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

#### $handlers

```php
protected $handlers = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Caches instances of the handlers.
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

#### $handlerConfig

```php
protected $handlerConfig = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Holds the configuration for each handler.
</td></tr>
</table>

<table>
<tr><td>
The key is the handler's class name. The
value is an associative array of configuration
items.
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

#### $logCache

```php
public $logCache;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Caches logging calls for debugbar.
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

#### $cacheLogs

```php
protected $cacheLogs = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Should we cache our logged items?
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
public function __construct($config, bool $debug = CI_DEBUG)
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
<td><em>\Config\Logger
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$debug</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\RuntimeException
</td>
</tr>
</table>



<details>
<summary><small>Source: 35 lines (149 - 183)</small></summary>

```php
public function __construct($config, bool $debug = CI_DEBUG)
{
	$this->loggableLevels = is_array($config->threshold) ? $config->threshold : range(1, (int) $config->threshold);

	// Now convert loggable levels to strings.
	// We only use numbers to make the threshold setting convenient for users.
	if ($this->loggableLevels)
	{
		$temp = [];
		foreach ($this->loggableLevels as $level)
		{
			$temp[] = array_search((int) $level, $this->logLevels);
		}

		$this->loggableLevels = $temp;
		unset($temp);
	}

	$this->dateFormat = $config->dateFormat ?? $this->dateFormat;

	if (! is_array($config->handlers) || empty($config->handlers))
	{
		throw LogException::forNoHandlers('LoggerConfig');
	}

	// Save the handler configuration for later.
	// Instances will be created on demand.
	$this->handlerConfig = $config->handlers;

	$this->cacheLogs = $debug;
	if ($this->cacheLogs)
	{
		$this->logCache = [];
	}
}
```

</details>


<hr>

#### emergency()

```php
public function emergency($message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
System is unusable.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (195 - 198)</small></summary>

```php
public function emergency($message, array $context = []): bool
{
	return $this->log('emergency', $message, $context);
}
```

</details>


<hr>

#### alert()

```php
public function alert($message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Action must be taken immediately.
</td></tr>
</table>

<table>
<tr><td>
Example: Entire website down, database unavailable, etc. This should
trigger the SMS alerts and wake you up.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (213 - 216)</small></summary>

```php
public function alert($message, array $context = []): bool
{
	return $this->log('alert', $message, $context);
}
```

</details>


<hr>

#### critical()

```php
public function critical($message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Critical conditions.
</td></tr>
</table>

<table>
<tr><td>
Example: Application component unavailable, unexpected exception.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (230 - 233)</small></summary>

```php
public function critical($message, array $context = []): bool
{
	return $this->log('critical', $message, $context);
}
```

</details>


<hr>

#### error()

```php
public function error($message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runtime errors that do not require immediate action but should typically
be logged and monitored.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (246 - 249)</small></summary>

```php
public function error($message, array $context = []): bool
{
	return $this->log('error', $message, $context);
}
```

</details>


<hr>

#### warning()

```php
public function warning($message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Exceptional occurrences that are not errors.
</td></tr>
</table>

<table>
<tr><td>
Example: Use of deprecated APIs, poor use of an API, undesirable things
that are not necessarily wrong.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (264 - 267)</small></summary>

```php
public function warning($message, array $context = []): bool
{
	return $this->log('warning', $message, $context);
}
```

</details>


<hr>

#### notice()

```php
public function notice($message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Normal but significant events.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (279 - 282)</small></summary>

```php
public function notice($message, array $context = []): bool
{
	return $this->log('notice', $message, $context);
}
```

</details>


<hr>

#### info()

```php
public function info($message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Interesting events.
</td></tr>
</table>

<table>
<tr><td>
Example: User logs in, SQL logs.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (296 - 299)</small></summary>

```php
public function info($message, array $context = []): bool
{
	return $this->log('info', $message, $context);
}
```

</details>


<hr>

#### debug()

```php
public function debug($message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Detailed debug information.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (311 - 314)</small></summary>

```php
public function debug($message, array $context = []): bool
{
	return $this->log('debug', $message, $context);
}
```

</details>


<hr>

#### log()

```php
public function log($level, $message, array $context = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Logs with an arbitrary level.
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$context</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 62 lines (327 - 388)</small></summary>

```php
public function log($level, $message, array $context = []): bool
{
	if (is_numeric($level))
	{
		$level = array_search((int) $level, $this->logLevels);
	}

	// Is the level a valid level?
	if (! array_key_exists($level, $this->logLevels))
	{
		throw LogException::forInvalidLogLevel($level);
	}

	// Does the app want to log this right now?
	if (! in_array($level, $this->loggableLevels))
	{
		return false;
	}

	// Parse our placeholders
	$message = $this->interpolate($message, $context);

	if (! is_string($message))
	{
		$message = print_r($message, true);
	}

	if ($this->cacheLogs)
	{
		$this->logCache[] = [
			'level' => $level,
			'msg'   => $message,
		];
	}

	foreach ($this->handlerConfig as $className => $config)
	{
		if (! array_key_exists($className, $this->handlers))
		{
			$this->handlers[$className] = new $className($config);
		}

		/**
		 * @var \CodeIgniter\Log\Handlers\HandlerInterface
		 */
		$handler = $this->handlers[$className];

		if (! $handler->canHandle($level))
		{
			continue;
		}

		// If the handler returns false, then we
		// don't execute any other handlers.
		if (! $handler->setDateFormat($this->dateFormat)->handle($level, $message))
		{
			break;
		}
	}

	return true;
}
```

</details>


<hr>

#### interpolate()

```php
protected function interpolate($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replaces any placeholders in the message with variables
from the context, as well as a few special items like:
</td></tr>
</table>

<table>
<tr><td>
{session_vars}
{post_vars}
{get_vars}
{env}
{env:foo}
{file}
{line}
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
<td><code>$message</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<summary><small>Source: 60 lines (409 - 468)</small></summary>

```php
protected function interpolate($message, array $context = [])
{
	if (! is_string($message))
	{
		return $message;
	}

	// build a replacement array with braces around the context keys
	$replace = [];

	foreach ($context as $key => $val)
	{
		// Verify that the 'exception' key is actually an exception
		// or error, both of which implement the 'Throwable' interface.
		if ($key === 'exception' && $val instanceof \Throwable)
		{
			$val = $val->getMessage() . ' ' . $this->cleanFileNames($val->getFile()) . ':' . $val->getLine();
		}

		// todo - sanitize input before writing to file?
		$replace['{' . $key . '}'] = $val;
	}

	// Add special placeholders
	$replace['{post_vars}'] = '$_POST: ' . print_r($_POST, true);
	$replace['{get_vars}']  = '$_GET: ' . print_r($_GET, true);
	$replace['{env}']       = ENVIRONMENT;

	// Allow us to log the file/line that we are logging from
	if (strpos($message, '{file}') !== false)
	{
		list($file, $line) = $this->determineFile();

		$replace['{file}'] = $file;
		$replace['{line}'] = $line;
	}

	// Match up environment variables in {env:foo} tags.
	if (strpos($message, 'env:') !== false)
	{
		preg_match('/env:[^}]+/', $message, $matches);

		if ($matches)
		{
			foreach ($matches as $str)
			{
				$key                 = str_replace('env:', '', $str);
				$replace["{{$str}}"] = $_ENV[$key] ?? 'n/a';
			}
		}
	}

	if (isset($_SESSION))
	{
		$replace['{session_vars}'] = '$_SESSION: ' . print_r($_SESSION, true);
	}

	// interpolate replacement values into the message and return
	return strtr($message, $replace);
}
```

</details>


<hr>

#### determineFile()

```php
public function determineFile() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines the file and line that the logging call
was made from by analyzing the backtrace.
</td></tr>
</table>

<table>
<tr><td>
Find the earliest stack frame that is part of our logging system.
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
<summary><small>Source: 40 lines (477 - 516)</small></summary>

```php
public function determineFile(): array
{
	$logFunctions = [
		'log_message',
		'log',
		'error',
		'debug',
		'info',
		'warning',
		'critical',
		'emergency',
		'alert',
		'notice',
	];

	// Generate Backtrace info
	$trace = \debug_backtrace(false);

	// So we search from the bottom (earliest) of the stack frames
	$stackFrames = \array_reverse($trace);

	// Find the first reference to a Logger class method
	foreach ($stackFrames as $frame)
	{
		if (\in_array($frame['function'], $logFunctions))
		{
			$file = isset($frame['file']) ? $this->cleanFileNames($frame['file']) : 'unknown';
			$line = $frame['line'] ?? 'unknown';
			return [
				$file,
				$line,
			];
		}
	}

	return [
		'unknown',
		'unknown',
	];
}
```

</details>


<hr>

#### cleanFileNames()

```php
protected function cleanFileNames(string $file) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cleans the paths of filenames by replacing APPPATH, SYSTEMPATH, FCPATH
with the actual var. i.e.
</td></tr>
</table>

<table>
<tr><td>
/var/www/site/app/Controllers/Home.php
    becomes:
APPPATH/Controllers/Home.php
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
<td><code>$file</code></td>
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
<summary><small>Source: 7 lines (532 - 538)</small></summary>

```php
protected function cleanFileNames(string $file): string
{
	$file = str_replace(APPPATH, 'APPPATH/', $file);
	$file = str_replace(SYSTEMPATH, 'SYSTEMPATH/', $file);

	return str_replace(FCPATH, 'FCPATH/', $file);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Log/Logger.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/HandlerInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Model.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:17**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>