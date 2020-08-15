


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Log/Handlers/FileHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/ChromeLoggerHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/HandlerInterface.md">next</a></td>
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
<td>framework/system/Log/Handlers/FileHandler.php
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



 

 
## CodeIgniter\Log\Handlers\FileHandler

<table style="text-align:left">
<tr><th>Class</th><td>FileHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Log\Handlers\FileHandler</td></tr>
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
Log error messages to file system
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
<th><a href="#path"><strong>path</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Folder to hold logs</td>
</tr>
<tr>
<th><a href="#fileExtension"><strong>fileExtension</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Extension to use for log files</td>
</tr>
<tr>
<th><a href="#filePermissions"><strong>filePermissions</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Permissions for new log files</td>
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

</table>





### Properties


<hr>

#### $path

```php
protected $path;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Folder to hold logs
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

#### $fileExtension

```php
protected $fileExtension;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Extension to use for log files
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

#### $filePermissions

```php
protected $filePermissions;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Permissions for new log files
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
<summary><small>Source: 11 lines (76 - 86)</small></summary>

```php
public function __construct(array $config = [])
{
	parent::__construct($config);

	$this->path = empty($config['path']) ? WRITEPATH . 'logs/' : $config['path'];

	$this->fileExtension = empty($config['fileExtension']) ? 'log' : $config['fileExtension'];
	$this->fileExtension = ltrim($this->fileExtension, '.');

	$this->filePermissions = $config['filePermissions'] ?? 0644;
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 60 lines (102 - 161)</small></summary>

```php
public function handle($level, $message): bool
{
	$filepath = $this->path . 'log-' . date('Y-m-d') . '.' . $this->fileExtension;

	$msg = '';

	if (! is_file($filepath))
	{
		$newfile = true;

		// Only add protection to php files
		if ($this->fileExtension === 'php')
		{
			$msg .= "<?php defined('SYSTEMPATH') || exit('No direct script access allowed'); ?>\n\n";
		}
	}

	if (! $fp = @fopen($filepath, 'ab'))
	{
		return false;
	}

	// Instantiating DateTime with microseconds appended to initial date is needed for proper support of this format
	if (strpos($this->dateFormat, 'u') !== false)
	{
		$microtime_full  = microtime(true);
		$microtime_short = sprintf('%06d', ($microtime_full - floor($microtime_full)) * 1000000);
		$date            = new \DateTime(date('Y-m-d H:i:s.' . $microtime_short, $microtime_full));
		$date            = $date->format($this->dateFormat);
	}
	else
	{
		$date = date($this->dateFormat);
	}

	$msg .= strtoupper($level) . ' - ' . $date . ' --> ' . $message . "\n";

	flock($fp, LOCK_EX);

	for ($written = 0, $length = strlen($msg); $written < $length; $written += $result)
	{
		if (($result = fwrite($fp, substr($msg, $written))) === false)
		{
			// if we get this far, we'll never see this during travis-ci
			// @codeCoverageIgnoreStart
			break;
			// @codeCoverageIgnoreEnd
		}
	}

	flock($fp, LOCK_UN);
	fclose($fp);

	if (isset($newfile) && $newfile === true)
	{
		chmod($filepath, $this->filePermissions);
	}

	return is_int($result);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Log/Handlers/FileHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/ChromeLoggerHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/HandlerInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:17**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>