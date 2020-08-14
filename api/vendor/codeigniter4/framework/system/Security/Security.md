


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Security/Security.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Security/Exceptions/SecurityException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Exceptions/SessionException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Security 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Security</td></tr>
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
<td>framework/system/Security/Security.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Security/Exceptions/SecurityException.md">CodeIgniter\Security\Exceptions\SecurityException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Security/Security.md">CodeIgniter\Security\Security</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md"><strong>CodeIgniter\HTTP\RequestInterface</strong></a>
</td>
<td>RequestInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Security/Exceptions/SecurityException.md"><strong>CodeIgniter\Security\Exceptions\SecurityException</strong></a>
</td>
<td>SecurityException</td>
</tr>
</table>



 
## CodeIgniter\Security\Security

<table style="text-align:left">
<tr><th>Class</th><td>Security</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Security\Security</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
HTTP security handler.
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
<th><a href="#CSRFHash"><strong>CSRFHash</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CSRF Hash</td>
</tr>
<tr>
<th><a href="#CSRFExpire"><strong>CSRFExpire</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CSRF Expire time</td>
</tr>
<tr>
<th><a href="#CSRFTokenName"><strong>CSRFTokenName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CSRF Token name</td>
</tr>
<tr>
<th><a href="#CSRFHeaderName"><strong>CSRFHeaderName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CSRF Header name</td>
</tr>
<tr>
<th><a href="#CSRFCookieName"><strong>CSRFCookieName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CSRF Cookie name</td>
</tr>
<tr>
<th><a href="#CSRFRegenerate"><strong>CSRFRegenerate</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CSRF Regenerate</td>
</tr>
<tr>
<th><a href="#cookiePath"><strong>cookiePath</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Typically will be a forward slash</td>
</tr>
<tr>
<th><a href="#cookieDomain"><strong>cookieDomain</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Set to .your-domain.com for site-wide cookies</td>
</tr>
<tr>
<th><a href="#cookieSecure"><strong>cookieSecure</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cookie will only be set if a secure HTTPS connection exists.</td>
</tr>
<tr>
<th><a href="#filenameBadChars"><strong>filenameBadChars</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>List of sanitize filename strings</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Security constructor.</td>
</tr>
<tr>
<th><a href="#CSRFVerify"><strong>CSRFVerify</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>CSRF Verify</td>
</tr>
<tr>
<th><a href="#CSRFSetCookie"><strong>CSRFSetCookie</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>CSRF Set Cookie</td>
</tr>
<tr>
<th><a href="#getCSRFHash"><strong>getCSRFHash</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the current CSRF Hash.</td>
</tr>
<tr>
<th><a href="#getCSRFTokenName"><strong>getCSRFTokenName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the CSRF Token Name.</td>
</tr>
<tr>
<th><a href="#CSRFSetHash"><strong>CSRFSetHash</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Sets the CSRF Hash and cookie.</td>
</tr>
<tr>
<th><a href="#sanitizeFilename"><strong>sanitizeFilename</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sanitize Filename</td>
</tr>

</table>





### Properties


<hr>

#### $CSRFHash

```php
protected $CSRFHash;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CSRF Hash
</td></tr>
</table>

<table>
<tr><td>
Random hash for Cross Site Request Forgery protection cookie
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

#### $CSRFExpire

```php
protected $CSRFExpire = 7200;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CSRF Expire time
</td></tr>
</table>

<table>
<tr><td>
Expiration time for Cross Site Request Forgery protection cookie.
Defaults to two hours (in seconds).
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

#### $CSRFTokenName

```php
protected $CSRFTokenName = 'CSRFToken';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CSRF Token name
</td></tr>
</table>

<table>
<tr><td>
Token name for Cross Site Request Forgery protection cookie.
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

#### $CSRFHeaderName

```php
protected $CSRFHeaderName = 'CSRFToken';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CSRF Header name
</td></tr>
</table>

<table>
<tr><td>
Token name for Cross Site Request Forgery protection cookie.
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

#### $CSRFCookieName

```php
protected $CSRFCookieName = 'CSRFToken';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CSRF Cookie name
</td></tr>
</table>

<table>
<tr><td>
Cookie name for Cross Site Request Forgery protection cookie.
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

#### $CSRFRegenerate

```php
protected $CSRFRegenerate = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CSRF Regenerate
</td></tr>
</table>

<table>
<tr><td>
If true, the CSRF Token will be regenerated on every request.
If false, will stay the same for the life of the cookie.
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

#### $cookiePath

```php
protected $cookiePath = '/';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Typically will be a forward slash
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
Set to .your-domain.com for site-wide cookies
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
Cookie will only be set if a secure HTTPS connection exists.
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

#### $filenameBadChars

```php
public $filenameBadChars = [
	'../',
	'<!--',
	'-->',
	'<',
	'>',
	"'",
	'"',
	'&',
	'$',
	'#',
	'{',
	'}',
	'[',
	']',
	'=',
	';',
	'?',
	'%20',
	'%22',
	'%3c', // <
	'%253c', // <
	'%3e', // >
	'%0e', // >
	'%28', // (
	'%29', // )
	'%2528', // (
	'%26', // &
	'%24', // $
	'%3f', // ?
	'%3b', // ;
	'%3d',       // =
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
List of sanitize filename strings
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
Security constructor.
</td></tr>
</table>

<table>
<tr><td>
Stores our configuration and fires off the init() method to
setup initial state.
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
<td><em>\Config\App
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 23 lines (179 - 201)</small></summary>

```php
public function __construct($config)
{
	// Store our CSRF-related settings
	$this->CSRFExpire     = $config->CSRFExpire;
	$this->CSRFTokenName  = $config->CSRFTokenName;
	$this->CSRFHeaderName = $config->CSRFHeaderName;
	$this->CSRFCookieName = $config->CSRFCookieName;
	$this->CSRFRegenerate = $config->CSRFRegenerate;

	if (isset($config->cookiePrefix))
	{
		$this->CSRFCookieName = $config->cookiePrefix . $this->CSRFCookieName;
	}

	// Store cookie-related settings
	$this->cookiePath   = $config->cookiePath;
	$this->cookieDomain = $config->cookieDomain;
	$this->cookieSecure = $config->cookieSecure;

	$this->CSRFSetHash();

	unset($config);
}
```

</details>


<hr>

#### CSRFVerify()

```php
public function CSRFVerify(RequestInterface $request)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CSRF Verify
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
<td><em>\RequestInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>$this<br>false
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
<summary><small>Source: 51 lines (213 - 263)</small></summary>

```php
public function CSRFVerify(RequestInterface $request)
{
	// If it's not a POST request we will set the CSRF cookie
	if (strtoupper($_SERVER['REQUEST_METHOD']) !== 'POST')
	{
		return $this->CSRFSetCookie($request);
	}

	// Do the tokens exist in _POST, HEADER or optionally php:://input - json data
	$CSRFTokenValue = $_POST[$this->CSRFTokenName] ??
		(! is_null($request->getHeader($this->CSRFHeaderName)) && ! empty($request->getHeader($this->CSRFHeaderName)->getValue()) ?
			$request->getHeader($this->CSRFHeaderName)->getValue() :
			(! empty($request->getBody()) && ! empty($json = json_decode($request->getBody())) && json_last_error() === JSON_ERROR_NONE ?
				($json->{$this->CSRFTokenName} ?? null) :
				null));

	// Do the tokens exist in both the _POST/POSTed JSON and _COOKIE arrays?
	if (! isset($CSRFTokenValue, $_COOKIE[$this->CSRFCookieName]) || $CSRFTokenValue !== $_COOKIE[$this->CSRFCookieName]
	) // Do the tokens match?
	{
		throw SecurityException::forDisallowedAction();
	}

	// We kill this since we're done and we don't want to pollute the _POST array
	if (isset($_POST[$this->CSRFTokenName]))
	{
		unset($_POST[$this->CSRFTokenName]);
		$request->setGlobal('post', $_POST);
	}
	// We kill this since we're done and we don't want to pollute the JSON data
	elseif (isset($json->{$this->CSRFTokenName}))
	{
		unset($json->{$this->CSRFTokenName});
		$request->setBody(json_encode($json));
	}

	// Regenerate on every submission?
	if ($this->CSRFRegenerate)
	{
		// Nothing should last forever
		$this->CSRFHash = null;
		unset($_COOKIE[$this->CSRFCookieName]);
	}

	$this->CSRFSetHash();
	$this->CSRFSetCookie($request);

	log_message('info', 'CSRF token verified');

	return $this;
}
```

</details>


<hr>

#### CSRFSetCookie()

```php
public function CSRFSetCookie(RequestInterface $request)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CSRF Set Cookie
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
</td>
</tr>
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
<td><em>\RequestInterface<br>\CodeIgniter\HTTP\IncomingRequest
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Security<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (276 - 293)</small></summary>

```php
public function CSRFSetCookie(RequestInterface $request)
{
	$expire        = time() + $this->CSRFExpire;
	$secure_cookie = (bool) $this->cookieSecure;

	if ($secure_cookie && ! $request->isSecure())
	{
		return false;
	}

	setcookie(
			$this->CSRFCookieName, $this->CSRFHash, $expire, $this->cookiePath, $this->cookieDomain, $secure_cookie, true                // Enforce HTTP only cookie for security
	);

	log_message('info', 'CSRF cookie sent');

	return $this;
}
```

</details>


<hr>

#### getCSRFHash()

```php
public function getCSRFHash() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the current CSRF Hash.
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
<summary><small>Source: 4 lines (302 - 305)</small></summary>

```php
public function getCSRFHash(): string
{
	return $this->CSRFHash;
}
```

</details>


<hr>

#### getCSRFTokenName()

```php
public function getCSRFTokenName() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the CSRF Token Name.
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
<summary><small>Source: 4 lines (314 - 317)</small></summary>

```php
public function getCSRFTokenName(): string
{
	return $this->CSRFTokenName;
}
```

</details>


<hr>

#### CSRFSetHash()

```php
protected function CSRFSetHash() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the CSRF Hash and cookie.
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 20 lines (327 - 346)</small></summary>

```php
protected function CSRFSetHash(): string
{
	if ($this->CSRFHash === null)
	{
		// If the cookie exists we will use its value.
		// We don't necessarily want to regenerate it with
		// each page load since a page could contain embedded
		// sub-pages causing this feature to fail
		if (isset($_COOKIE[$this->CSRFCookieName]) && is_string($_COOKIE[$this->CSRFCookieName]) && preg_match('#^[0-9a-f]{32}$#iS', $_COOKIE[$this->CSRFCookieName]) === 1
		)
		{
			return $this->CSRFHash = $_COOKIE[$this->CSRFCookieName];
		}

		$rand           = random_bytes(16);
		$this->CSRFHash = bin2hex($rand);
	}

	return $this->CSRFHash;
}
```

</details>


<hr>

#### sanitizeFilename()

```php
public function sanitizeFilename(string $str, bool $relative_path = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sanitize Filename
</td></tr>
</table>

<table>
<tr><td>
Tries to sanitize filenames in order to prevent directory traversal attempts
and other security threats, which is particularly useful for files that
were supplied via user input.

If it is acceptable for the user input to include relative paths,
e.g. file/in/some/approved/folder.txt, you can set the second optional
parameter, $relative_path to TRUE.
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Input file name</td>
</tr>

<tr>
<td>2.</td>
<td><code>$relative_path</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to preserve paths</td>
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
<summary><small>Source: 21 lines (366 - 386)</small></summary>

```php
public function sanitizeFilename(string $str, bool $relative_path = false): string
{
	$bad = $this->filenameBadChars;

	if (! $relative_path)
	{
		$bad[] = './';
		$bad[] = '/';
	}

	$str = remove_invisible_characters($str, false);

	do
	{
		$old = $str;
		$str = str_replace($bad, '', $str);
	}
	while ($old !== $str);

	return stripslashes($str);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Security/Security.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Security/Exceptions/SecurityException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Exceptions/SessionException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>