


 



<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Request.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RedirectResponse.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md">next</a></td>
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
<td>framework/system/HTTP/Request.php
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



 

 
## CodeIgniter\HTTP\Request

<table style="text-align:left">
<tr><th>Class</th><td>Request</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\HTTP\Request</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Message.md">CodeIgniter\HTTP\Message</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md">CodeIgniter\HTTP\RequestInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Representation of an HTTP request.
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
<th><a href="#ipAddress"><strong>ipAddress</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>IP address of the current user.</td>
</tr>
<tr>
<th><a href="#proxyIPs"><strong>proxyIPs</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Proxy IPs</td>
</tr>
<tr>
<th><a href="#method"><strong>method</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Request method.</td>
</tr>
<tr>
<th><a href="#globals"><strong>globals</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores values we&#039;ve retrieved from
PHP globals.</td>
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
<th><a href="#getIPAddress"><strong>getIPAddress</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Gets the user&#039;s IP address.</td>
</tr>
<tr>
<th><a href="#isValidIP"><strong>isValidIP</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Validate an IP address</td>
</tr>
<tr>
<th><a href="#getMethod"><strong>getMethod</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get the request method.</td>
</tr>
<tr>
<th><a href="#setMethod"><strong>setMethod</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the request method. Used when spoofing the request.</td>
</tr>
<tr>
<th><a href="#getServer"><strong>getServer</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Fetch an item from the $_SERVER array.</td>
</tr>
<tr>
<th><a href="#getEnv"><strong>getEnv</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Fetch an item from the $_ENV array.</td>
</tr>
<tr>
<th><a href="#setGlobal"><strong>setGlobal</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows manually setting the value of PHP global, like $_GET, $_POST, etc.</td>
</tr>
<tr>
<th><a href="#fetchGlobal"><strong>fetchGlobal</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Fetches one or more items from a global, like cookies, get, post, etc.</td>
</tr>
<tr>
<th><a href="#populateGlobals"><strong>populateGlobals</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Saves a copy of the current state of one of several PHP globals
so we can retrieve them later.</td>
</tr>

</table>





### Properties


<hr>

#### $ipAddress

```php
protected $ipAddress = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
IP address of the current user.
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

#### $proxyIPs

```php
protected $proxyIPs;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Proxy IPs
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>string<br>array
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
Request method.
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

#### $globals

```php
protected $globals = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores values we've retrieved from
PHP globals.
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
<td><em>object
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (84 - 92)</small></summary>

```php
public function __construct($config)
{
	$this->proxyIPs = $config->proxyIPs;

	if (empty($this->method))
	{
		$this->method = $this->getServer('REQUEST_METHOD') ?? 'GET';
	}
}
```

</details>


<hr>

#### getIPAddress()

```php
public function getIPAddress() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets the user's IP address.
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
<summary><small>Source: 124 lines (101 - 224)</small></summary>

```php
public function getIPAddress(): string
{
	if (! empty($this->ipAddress))
	{
		return $this->ipAddress;
	}

	$proxy_ips = $this->proxyIPs;
	if (! empty($this->proxyIPs) && ! is_array($this->proxyIPs))
	{
		$proxy_ips = explode(',', str_replace(' ', '', $this->proxyIPs));
	}

	$this->ipAddress = $this->getServer('REMOTE_ADDR');

	if ($proxy_ips)
	{
		foreach (['HTTP_X_FORWARDED_FOR', 'HTTP_CLIENT_IP', 'HTTP_X_CLIENT_IP', 'HTTP_X_CLUSTER_CLIENT_IP'] as $header)
		{
			if (($spoof = $this->getServer($header)) !== null)
			{
				// Some proxies typically list the whole chain of IP
				// addresses through which the client has reached us.
				// e.g. client_ip, proxy_ip1, proxy_ip2, etc.
				sscanf($spoof, '%[^,]', $spoof);

				if (! $this->isValidIP($spoof))
				{
					$spoof = null;
				}
				else
				{
					break;
				}
			}
		}

		if ($spoof)
		{
			foreach ($proxy_ips as $proxy_ip)
			{
				// Check if we have an IP address or a subnet
				if (strpos($proxy_ip, '/') === false)
				{
					// An IP address (and not a subnet) is specified.
					// We can compare right away.
					if ($proxy_ip === $this->ipAddress)
					{
						$this->ipAddress = $spoof;
						break;
					}

					continue;
				}

				// We have a subnet ... now the heavy lifting begins
				isset($separator) || $separator = $this->isValidIP($this->ipAddress, 'ipv6') ? ':' : '.';

				// If the proxy entry doesn't match the IP protocol - skip it
				if (strpos($proxy_ip, $separator) === false)
				{
					continue;
				}

				// Convert the REMOTE_ADDR IP address to binary, if needed
				if (! isset($ip, $sprintf))
				{
					if ($separator === ':')
					{
						// Make sure we're have the "full" IPv6 format
						$ip = explode(':', str_replace('::', str_repeat(':', 9 - substr_count($this->ipAddress, ':')), $this->ipAddress
								)
						);

						for ($j = 0; $j < 8; $j ++)
						{
							$ip[$j] = intval($ip[$j], 16);
						}

						$sprintf = '%016b%016b%016b%016b%016b%016b%016b%016b';
					}
					else
					{
						$ip      = explode('.', $this->ipAddress);
						$sprintf = '%08b%08b%08b%08b';
					}

					$ip = vsprintf($sprintf, $ip);
				}

				// Split the netmask length off the network address
				sscanf($proxy_ip, '%[^/]/%d', $netaddr, $masklen);

				// Again, an IPv6 address is most likely in a compressed form
				if ($separator === ':')
				{
					$netaddr = explode(':', str_replace('::', str_repeat(':', 9 - substr_count($netaddr, ':')), $netaddr));
					for ($i = 0; $i < 8; $i ++)
					{
						$netaddr[$i] = intval($netaddr[$i], 16);
					}
				}
				else
				{
					$netaddr = explode('.', $netaddr);
				}

				// Convert to binary and finally compare
				if (strncmp($ip, vsprintf($sprintf, $netaddr), $masklen) === 0)
				{
					$this->ipAddress = $spoof;
					break;
				}
			}
		}
	}

	if (! $this->isValidIP($this->ipAddress))
	{
		return $this->ipAddress = '0.0.0.0';
	}

	return empty($this->ipAddress) ? '' : $this->ipAddress;
}
```

</details>


<hr>

#### isValidIP()

```php
public function isValidIP(string $ip = null, string $which = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validate an IP address
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
<td><code>$ip</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>IP Address</td>
</tr>

<tr>
<td>2.</td>
<td><code>$which</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>IP protocol: 'ipv4' or 'ipv6'</td>
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
<summary><small>Source: 17 lines (236 - 252)</small></summary>

```php
public function isValidIP(string $ip = null, string $which = null): bool
{
	switch (strtolower( (string) $which))
	{
		case 'ipv4':
			$which = FILTER_FLAG_IPV4;
			break;
		case 'ipv6':
			$which = FILTER_FLAG_IPV6;
			break;
		default:
			$which = null;
			break;
	}

	return (bool) filter_var($ip, FILTER_VALIDATE_IP, $which);
}
```

</details>


<hr>

#### getMethod()

```php
public function getMethod(bool $upper = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get the request method.
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
<td><code>$upper</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to return in upper or lower case.</td>
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
<summary><small>Source: 4 lines (263 - 266)</small></summary>

```php
public function getMethod(bool $upper = false): string
{
	return ($upper) ? strtoupper($this->method) : strtolower($this->method);
}
```

</details>


<hr>

#### setMethod()

```php
public function setMethod(string $method)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the request method. Used when spoofing the request.
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
<td><code>$method</code></td>
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
<td>\Request
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (277 - 282)</small></summary>

```php
public function setMethod(string $method)
{
	$this->method = $method;

	return $this;
}
```

</details>


<hr>

#### getServer()

```php
public function getServer($index = null, $filter = null, $flags = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetch an item from the $_SERVER array.
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
<td><code>$index</code></td>
<td><em>string<br>array<br>null
</em></td>
<td>false</td>
<td>Index for item to be fetched from $_SERVER</td>
</tr>

<tr>
<td>2.</td>
<td><code>$filter</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td>A filter name to be applied</td>
</tr>

<tr>
<td>3.</td>
<td><code>$flags</code></td>
<td><em>null
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
<summary><small>Source: 4 lines (295 - 298)</small></summary>

```php
public function getServer($index = null, $filter = null, $flags = null)
{
	return $this->fetchGlobal('server', $index, $filter, $flags);
}
```

</details>


<hr>

#### getEnv()

```php
public function getEnv($index = null, $filter = null, $flags = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetch an item from the $_ENV array.
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
<td><code>$index</code></td>
<td><em>null
</em></td>
<td>false</td>
<td>Index for item to be fetched from $_ENV</td>
</tr>

<tr>
<td>2.</td>
<td><code>$filter</code></td>
<td><em>null
</em></td>
<td>false</td>
<td>A filter name to be applied</td>
</tr>

<tr>
<td>3.</td>
<td><code>$flags</code></td>
<td><em>null
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
<summary><small>Source: 4 lines (311 - 314)</small></summary>

```php
public function getEnv($index = null, $filter = null, $flags = null)
{
	return $this->fetchGlobal('env', $index, $filter, $flags);
}
```

</details>


<hr>

#### setGlobal()

```php
public function setGlobal(string $method, $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows manually setting the value of PHP global, like $_GET, $_POST, etc.
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
<td><code>$method</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (326 - 331)</small></summary>

```php
public function setGlobal(string $method, $value)
{
	$this->globals[$method] = $value;

	return $this;
}
```

</details>


<hr>

#### fetchGlobal()

```php
public function fetchGlobal($method, $index = null, $filter = null, $flags = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetches one or more items from a global, like cookies, get, post, etc.
</td></tr>
</table>

<table>
<tr><td>
Can optionally filter the input when you retrieve it by passing in
a filter.

If $type is an array, it must conform to the input allowed by the
filter_input_array method.

<a href="http://php.net/manual/en/filter.filters.sanitize.php">http://php.net/manual/en/filter.filters.sanitize.php</a>
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
<td><code>$method</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Input filter constant</td>
</tr>

<tr>
<td>2.</td>
<td><code>$index</code></td>
<td><em>string<br>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$filter</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td>Filter constant</td>
</tr>

<tr>
<td>4.</td>
<td><code>$flags</code></td>
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
<summary><small>Source: 89 lines (352 - 440)</small></summary>

```php
public function fetchGlobal($method, $index = null, $filter = null, $flags = null)
{
	$method = strtolower($method);

	if (! isset($this->globals[$method]))
	{
		$this->populateGlobals($method);
	}

	// Null filters cause null values to return.
	if (is_null($filter))
	{
		$filter = FILTER_DEFAULT;
	}

	// Return all values when $index is null
	if (is_null($index))
	{
		$values = [];
		foreach ($this->globals[$method] as $key => $value)
		{
			$values[$key] = is_array($value)
				? $this->fetchGlobal($method, $key, $filter, $flags)
				: filter_var($value, $filter, $flags);
		}

		return $values;
	}

	// allow fetching multiple keys at once
	if (is_array($index))
	{
		$output = [];

		foreach ($index as $key)
		{
			$output[$key] = $this->fetchGlobal($method, $key, $filter, $flags);
		}

		return $output;
	}

	// Does the index contain array notation?
	if (($count = preg_match_all('/(?:^[^\[]+)|\[[^]]*\]/', $index, $matches)) > 1)
	{
		$value = $this->globals[$method];
		for ($i = 0; $i < $count; $i++)
		{
			$key = trim($matches[0][$i], '[]');

			if ($key === '') // Empty notation will return the value as array
			{
				break;
			}

			if (isset($value[$key]))
			{
				$value = $value[$key];
			}
			else
			{
				return null;
			}
		}
	}

	if (! isset($value))
	{
		$value = $this->globals[$method][$index] ?? null;
	}

	if (is_array($value) && ($filter !== null || $flags !== null))
	{
		// Iterate over array and append filter and flags
		array_walk_recursive($value, function (&$val) use ($filter, $flags) {
			$val = filter_var($val, $filter, $flags);
		});

		return $value;
	}

	// Cannot filter these types of data automatically...
	if (is_array($value) || is_object($value) || is_null($value))
	{
		return $value;
	}

	return filter_var($value, $filter, $flags);
}
```

</details>


<hr>

#### populateGlobals()

```php
protected function populateGlobals(string $method)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Saves a copy of the current state of one of several PHP globals
so we can retrieve them later.
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
<td><code>$method</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 28 lines (450 - 477)</small></summary>

```php
protected function populateGlobals(string $method)
{
	if (! isset($this->globals[$method]))
	{
		$this->globals[$method] = [];
	}

	// Don't populate ENV as it might contain
	// sensitive data that we don't want to get logged.
	switch($method)
	{
		case 'get':
			$this->globals['get'] = $_GET;
			break;
		case 'post':
			$this->globals['post'] = $_POST;
			break;
		case 'request':
			$this->globals['request'] = $_REQUEST;
			break;
		case 'cookie':
			$this->globals['cookie'] = $_COOKIE;
			break;
		case 'server':
			$this->globals['server'] = $_SERVER;
			break;
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Request.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RedirectResponse.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>