


 



<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/CLIRequest.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/XMLFormatter.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/CURLRequest.md">next</a></td>
</tr>
</table>







# CodeIgniter\HTTP 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\HTTP</td></tr>
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
<td>framework/system/HTTP/CLIRequest.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/CLIRequest.md">CodeIgniter\HTTP\CLIRequest</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/CURLRequest.md">CodeIgniter\HTTP\CURLRequest</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/ContentSecurityPolicy.md">CodeIgniter\HTTP\ContentSecurityPolicy</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/DownloadResponse.md">CodeIgniter\HTTP\DownloadResponse</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Exceptions/HTTPException.md">CodeIgniter\HTTP\Exceptions\HTTPException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/FileCollection.md">CodeIgniter\HTTP\Files\FileCollection</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFile.md">CodeIgniter\HTTP\Files\UploadedFile</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFileInterface.md">CodeIgniter\HTTP\Files\UploadedFileInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Header.md">CodeIgniter\HTTP\Header</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/IncomingRequest.md">CodeIgniter\HTTP\IncomingRequest</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Message.md">CodeIgniter\HTTP\Message</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Negotiate.md">CodeIgniter\HTTP\Negotiate</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RedirectResponse.md">CodeIgniter\HTTP\RedirectResponse</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Request.md">CodeIgniter\HTTP\Request</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md">CodeIgniter\HTTP\RequestInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Response.md">CodeIgniter\HTTP\Response</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/ResponseInterface.md">CodeIgniter\HTTP\ResponseInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/URI.md">CodeIgniter\HTTP\URI</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/UserAgent.md">CodeIgniter\HTTP\UserAgent</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>Config\App</strong>
</td>
<td>App</td>
</tr>
</table>



 
## CodeIgniter\HTTP\CLIRequest

<table style="text-align:left">
<tr><th>Class</th><td>CLIRequest</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\HTTP\CLIRequest</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Request.md">CodeIgniter\HTTP\Request</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class CLIRequest
</td></tr>
</table>

<table>
<tr><td>
Represents a request from the command-line. Provides additional
tools to interact with that request since CLI requests are not
static like HTTP requests might be.

Portions of this code were initially from the FuelPHP Framework,
version 1.7.x, and used here under the MIT license they were
originally made available under.

<a href="http://fuelphp.com">http://fuelphp.com</a>
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\HTTP
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
<th><a href="#segments"><strong>segments</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores the segments of our cli &quot;URI&quot; command.</td>
</tr>
<tr>
<th><a href="#options"><strong>options</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Command line options and their values.</td>
</tr>
<tr>
<th><a href="#method"><strong>method</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Set the expected HTTP verb</td>
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
<th><a href="#getPath"><strong>getPath</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the &quot;path&quot; of the request script so that it can be used
in routing to the appropriate controller/method.</td>
</tr>
<tr>
<th><a href="#getOptions"><strong>getOptions</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an associative array of all CLI options found, with
their values.</td>
</tr>
<tr>
<th><a href="#getSegments"><strong>getSegments</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the path segments.</td>
</tr>
<tr>
<th><a href="#getOption"><strong>getOption</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the value for a single CLI option that was passed in.</td>
</tr>
<tr>
<th><a href="#getOptionString"><strong>getOptionString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the options as a string, suitable for passing along on
the CLI to other commands.</td>
</tr>
<tr>
<th><a href="#parseCommand"><strong>parseCommand</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Parses the command line it was called from and collects all options
and valid segments.</td>
</tr>
<tr>
<th><a href="#isCLI"><strong>isCLI</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines if this request was made from the command line (CLI).</td>
</tr>

</table>





### Properties


<hr>

#### $segments

```php
protected $segments = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the segments of our cli "URI" command.
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

#### $options

```php
protected $options = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Command line options and their values.
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

#### $method

```php
protected $method = 'cli';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the expected HTTP verb
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
public function __construct(App $config)
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
<td><em>\App
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (89 - 97)</small></summary>

```php
public function __construct(App $config)
{
	parent::__construct($config);

	// Don't terminate the script when the cli's tty goes away
	ignore_user_abort(true);

	$this->parseCommand();
}
```

</details>


<hr>

#### getPath()

```php
public function getPath() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the "path" of the request script so that it can be used
in routing to the appropriate controller/method.
</td></tr>
</table>

<table>
<tr><td>
The path is determined by treating the command line arguments
as if it were a URL - up until we hit our first option.

Example:
     php index.php users 21 profile -foo bar

     // Routes to /users/21/profile (index is removed for routing sake)
     // with the option foo = bar.
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
<summary><small>Source: 6 lines (116 - 121)</small></summary>

```php
public function getPath(): string
{
	$path = implode('/', $this->segments);

	return empty($path) ? '' : $path;
}
```

</details>


<hr>

#### getOptions()

```php
public function getOptions() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an associative array of all CLI options found, with
their values.
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
<summary><small>Source: 4 lines (131 - 134)</small></summary>

```php
public function getOptions(): array
{
	return $this->options;
}
```

</details>


<hr>

#### getSegments()

```php
public function getSegments() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the path segments.
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
<summary><small>Source: 4 lines (143 - 146)</small></summary>

```php
public function getSegments(): array
{
	return $this->segments;
}
```

</details>


<hr>

#### getOption()

```php
public function getOption(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the value for a single CLI option that was passed in.
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
<td><code>$key</code></td>
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
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (157 - 160)</small></summary>

```php
public function getOption(string $key)
{
	return $this->options[$key] ?? null;
}
```

</details>


<hr>

#### getOptionString()

```php
public function getOptionString() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the options as a string, suitable for passing along on
the CLI to other commands.
</td></tr>
</table>

<table>
<tr><td>
Example:
$options = [
    'foo' => 'bar',
    'baz' => 'queue some stuff'
];

getOptionString() = '-foo bar -baz "queue some stuff"'
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
<summary><small>Source: 23 lines (178 - 200)</small></summary>

```php
public function getOptionString(): string
{
	if (empty($this->options))
	{
		return '';
	}

	$out = '';

	foreach ($this->options as $name => $value)
	{
		// If there's a space, we need to group
		// so it will pass correctly.
		if (strpos($value, ' ') !== false)
		{
			$value = '"' . $value . '"';
		}

		$out .= "-{$name} $value ";
	}

	return trim($out);
}
```

</details>


<hr>

#### parseCommand()

```php
protected function parseCommand()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses the command line it was called from and collects all options
and valid segments.
</td></tr>
</table>

<table>
<tr><td>
NOTE: I tried to use getopt but had it fail occasionally to find
any options, where argv has always had our back.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 35 lines (211 - 245)</small></summary>

```php
protected function parseCommand()
{
	$args = $this->getServer('argv');
	array_shift($args); // Scrap index.php

	$optionValue = false;

	foreach ($args as $i => $arg)
	{
		if (mb_strpos($arg, '-') !== 0)
		{
			if ($optionValue)
			{
				$optionValue = false;
			}
			else
			{
				$this->segments[] = filter_var($arg, FILTER_SANITIZE_STRING);
			}

			continue;
		}

		$arg   = filter_var(ltrim($arg, '-'), FILTER_SANITIZE_STRING);
		$value = null;

		if (isset($args[$i + 1]) && mb_strpos($args[$i + 1], '-') !== 0)
		{
			$value       = filter_var($args[$i + 1], FILTER_SANITIZE_STRING);
			$optionValue = true;
		}

		$this->options[$arg] = $value;
	}
}
```

</details>


<hr>

#### isCLI()

```php
public function isCLI() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines if this request was made from the command line (CLI).
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
<summary><small>Source: 4 lines (254 - 257)</small></summary>

```php
public function isCLI(): bool
{
	return is_cli();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/CLIRequest.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/XMLFormatter.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/CURLRequest.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>