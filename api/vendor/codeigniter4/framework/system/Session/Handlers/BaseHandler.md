


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/BaseHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/ArrayHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/DatabaseHandler.md">next</a></td>
</tr>
</table>







# CodeIgniter\Session\Handlers 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Session\Handlers</td></tr>
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
<td>framework/system/Session/Handlers/BaseHandler.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/ArrayHandler.md">CodeIgniter\Session\Handlers\ArrayHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">CodeIgniter\Session\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/DatabaseHandler.md">CodeIgniter\Session\Handlers\DatabaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/FileHandler.md">CodeIgniter\Session\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/MemcachedHandler.md">CodeIgniter\Session\Handlers\MemcachedHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/RedisHandler.md">CodeIgniter\Session\Handlers\RedisHandler</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md"><strong>CodeIgniter\Config\BaseConfig</strong></a>
</td>
<td>BaseConfig</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerAwareTrait.md"><strong>Psr\Log\LoggerAwareTrait</strong></a>
</td>
<td>LoggerAwareTrait</td>
</tr>
</table>



 
## CodeIgniter\Session\Handlers\BaseHandler

<table style="text-align:left">
<tr><th>Abstract</th><td>BaseHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Session\Handlers\BaseHandler</td></tr>
<tr><th>Implements</th>
<td>
<a href="">CodeIgniter\Session\Handlers\SessionHandlerInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Base class for session handling
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
<th><a href="#fingerprint"><strong>fingerprint</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Data fingerprint.</td>
</tr>
<tr>
<th><a href="#lock"><strong>lock</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Lock placeholder.</td>
</tr>
<tr>
<th><a href="#cookiePrefix"><strong>cookiePrefix</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cookie prefix</td>
</tr>
<tr>
<th><a href="#cookieDomain"><strong>cookieDomain</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cookie domain</td>
</tr>
<tr>
<th><a href="#cookiePath"><strong>cookiePath</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cookie path</td>
</tr>
<tr>
<th><a href="#cookieSecure"><strong>cookieSecure</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cookie secure?</td>
</tr>
<tr>
<th><a href="#cookieName"><strong>cookieName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cookie name to use</td>
</tr>
<tr>
<th><a href="#matchIP"><strong>matchIP</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Match IP addresses for cookies?</td>
</tr>
<tr>
<th><a href="#sessionID"><strong>sessionID</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Current session ID</td>
</tr>
<tr>
<th><a href="#savePath"><strong>savePath</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The &#039;save path&#039; for the session
varies between</td>
</tr>
<tr>
<th><a href="#ipAddress"><strong>ipAddress</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>User&#039;s IP address.</td>
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
<th><a href="#destroyCookie"><strong>destroyCookie</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Internal method to force removal of a cookie by the client
when session_destroy() is called.</td>
</tr>
<tr>
<th><a href="#lockSession"><strong>lockSession</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A dummy method allowing drivers with no locking functionality
(databases other than PostgreSQL and MySQL) to act as if they
do acquire a lock.</td>
</tr>
<tr>
<th><a href="#releaseLock"><strong>releaseLock</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Releases the lock, if any.</td>
</tr>
<tr>
<th><a href="#fail"><strong>fail</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Fail</td>
</tr>

</table>





### Properties


<hr>

#### $fingerprint

```php
protected $fingerprint;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Data fingerprint.
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

#### $lock

```php
protected $lock = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Lock placeholder.
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

#### $cookiePrefix

```php
protected $cookiePrefix = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cookie prefix
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

#### $cookieDomain

```php
protected $cookieDomain = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cookie domain
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

#### $cookiePath

```php
protected $cookiePath = '/';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cookie path
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

#### $cookieSecure

```php
protected $cookieSecure = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cookie secure?
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

#### $cookieName

```php
protected $cookieName;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cookie name to use
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

#### $matchIP

```php
protected $matchIP = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Match IP addresses for cookies?
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

#### $sessionID

```php
protected $sessionID;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Current session ID
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

#### $savePath

```php
protected $savePath;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The 'save path' for the session
varies between
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

#### $ipAddress

```php
protected $ipAddress;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
User's IP address.
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
public function __construct($config, string $ipAddress)
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
<td><em>\BaseConfig
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$ipAddress</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 11 lines (139 - 149)</small></summary>

```php
public function __construct($config, string $ipAddress)
{
	$this->cookiePrefix = $config->cookiePrefix;
	$this->cookieDomain = $config->cookieDomain;
	$this->cookiePath   = $config->cookiePath;
	$this->cookieSecure = $config->cookieSecure;
	$this->cookieName   = $config->sessionCookieName;
	$this->matchIP      = $config->sessionMatchIP;
	$this->savePath     = $config->sessionSavePath;
	$this->ipAddress    = $ipAddress;
}
```

</details>


<hr>

#### destroyCookie()

```php
protected function destroyCookie() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Internal method to force removal of a cookie by the client
when session_destroy() is called.
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
<summary><small>Source: 6 lines (159 - 164)</small></summary>

```php
protected function destroyCookie(): bool
{
	return setcookie(
			$this->cookieName, null, 1, $this->cookiePath, $this->cookieDomain, $this->cookieSecure, true
	);
}
```

</details>


<hr>

#### lockSession()

```php
protected function lockSession(string $sessionID) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A dummy method allowing drivers with no locking functionality
(databases other than PostgreSQL and MySQL) to act as if they
do acquire a lock.
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
<td><code>$sessionID</code></td>
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
<summary><small>Source: 5 lines (177 - 181)</small></summary>

```php
protected function lockSession(string $sessionID): bool
{
	$this->lock = true;
	return true;
}
```

</details>


<hr>

#### releaseLock()

```php
protected function releaseLock() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Releases the lock, if any.
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
<summary><small>Source: 6 lines (190 - 195)</small></summary>

```php
protected function releaseLock(): bool
{
	$this->lock = false;

	return true;
}
```

</details>


<hr>

#### fail()

```php
protected function fail() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fail
</td></tr>
</table>

<table>
<tr><td>
Drivers other than the 'files' one don't (need to) use the
session.save_path INI setting, but that leads to confusing
error messages emitted by PHP when open() or write() fail,
as the message contains session.save_path ...
To work around the problem, the drivers will call this method
so that the INI is set just in time for the error message to
be properly generated.
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
<summary><small>Source: 6 lines (212 - 217)</small></summary>

```php
protected function fail(): bool
{
	ini_set('session.save_path', $this->savePath);

	return false;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/BaseHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/ArrayHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/DatabaseHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>