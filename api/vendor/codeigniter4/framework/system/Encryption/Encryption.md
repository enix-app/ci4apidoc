


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Encryption/Encryption.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/EncrypterInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Exceptions/EncryptionException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Encryption 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Encryption</td></tr>
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

Copyright (c) 2014-2017 British Columbia Institute of Technology
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
<td>2014-2017 British Columbia Institute of Technology (<a href="https://bcit.ca">https://bcit.ca</a>/)
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
<td>framework/system/Encryption/Encryption.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/EncrypterInterface.md">CodeIgniter\Encryption\EncrypterInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Encryption.md">CodeIgniter\Encryption\Encryption</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Exceptions/EncryptionException.md">CodeIgniter\Encryption\Exceptions\EncryptionException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/BaseHandler.md">CodeIgniter\Encryption\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/OpenSSLHandler.md">CodeIgniter\Encryption\Handlers\OpenSSLHandler</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md"><strong>CodeIgniter\Config\BaseConfig</strong></a>
</td>
<td>BaseConfig</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Exceptions/EncryptionException.md"><strong>CodeIgniter\Encryption\Exceptions\EncryptionException</strong></a>
</td>
<td>EncryptionException</td>
</tr>
</table>



 
## CodeIgniter\Encryption\Encryption

<table style="text-align:left">
<tr><th>Class</th><td>Encryption</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Encryption\Encryption</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CodeIgniter Encryption Manager
</td></tr>
</table>

<table>
<tr><td>
Provides two-way keyed encryption via PHP's Sodium and/or OpenSSL extensions.
This class determines the driver, cipher, and mode to use, and then
initializes the appropriate encryption handler.
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
<th><a href="#encrypter"><strong>encrypter</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The encrypter we create</td>
</tr>
<tr>
<th><a href="#driver"><strong>driver</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The driver being used</td>
</tr>
<tr>
<th><a href="#key"><strong>key</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The key/seed being used</td>
</tr>
<tr>
<th><a href="#hmacKey"><strong>hmacKey</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The derived hmac key</td>
</tr>
<tr>
<th><a href="#digest"><strong>digest</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>HMAC digest to use</td>
</tr>
<tr>
<th><a href="#drivers"><strong>drivers</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Map of drivers to handler classes, in preference order</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Class constructor</td>
</tr>
<tr>
<th><a href="#initialize"><strong>initialize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Initialize or re-initialize an encrypter</td>
</tr>
<tr>
<th><a href="#createKey"><strong>createKey</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Create a random key</td>
</tr>
<tr>
<th><a href="#__get"><strong>__get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>__get() magic, providing readonly access to some of our protected properties</td>
</tr>
<tr>
<th><a href="#__isset"><strong>__isset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>__isset() magic, providing checking for some of our protected properties</td>
</tr>

</table>





### Properties


<hr>

#### $encrypter

```php
protected $encrypter;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The encrypter we create
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

#### $driver

```php
protected $driver;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The driver being used
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>






<hr>

#### $key

```php
protected $key;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The key/seed being used
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>






<hr>

#### $hmacKey

```php
protected $hmacKey;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The derived hmac key
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>






<hr>

#### $digest

```php
protected $digest = 'SHA512';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
HMAC digest to use
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>






<hr>

#### $drivers

```php
protected $drivers = [
	'OpenSSL',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Map of drivers to handler classes, in preference order
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
public function __construct(BaseConfig $config = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class constructor
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
<td>Configuration parameters</td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Encryption\Exceptions\EncryptionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 22 lines (100 - 121)</small></summary>

```php
public function __construct(BaseConfig $config = null)
{
	$config = $config ?? new \Config\Encryption();

	$this->key    = $config->key;
	$this->driver = $config->driver;
	$this->digest = $config->digest ?? 'SHA512';

	// determine what is installed
	$this->handlers = [
		'OpenSSL' => extension_loaded('openssl'),
	];

	// if any aren't there, bomb
	if (in_array(false, $this->handlers))
	{
		// this should never happen in travis-ci
		// @codeCoverageIgnoreStart
		throw EncryptionException::forNoHandlerAvailable($this->driver);
		// @codeCoverageIgnoreEnd
	}
}
```

</details>


<hr>

#### initialize()

```php
public function initialize(BaseConfig $config = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Initialize or re-initialize an encrypter
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
<td>Configuration parameters</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Encryption\EncrypterInterface
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Encryption\Exceptions\EncryptionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 34 lines (131 - 164)</small></summary>

```php
public function initialize(BaseConfig $config = null)
{
	// override config?
	if ($config)
	{
		$this->key    = $config->key;
		$this->driver = $config->driver;
		$this->digest = $config->digest ?? 'SHA512';
	}

	// Insist on a driver
	if (empty($this->driver))
	{
		throw EncryptionException::forNoDriverRequested();
	}

	// Check for an unknown driver
	if (! in_array($this->driver, $this->drivers))
	{
		throw EncryptionException::forUnKnownHandler($this->driver);
	}

	if (empty($this->key))
	{
		throw EncryptionException::forNeedsStarterKey();
	}

	// Derive a secret key for the encrypter
	$this->hmacKey = bin2hex(\hash_hkdf($this->digest, $this->key));

	$handlerName     = 'CodeIgniter\\Encryption\\Handlers\\' . $this->driver . 'Handler';
	$this->encrypter = new $handlerName($config);
	return $this->encrypter;
}
```

</details>


<hr>

#### createKey()

```php
public static function createKey($length = 32)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create a random key
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
<td><code>$length</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Output length</td>
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
<summary><small>Source: 4 lines (174 - 177)</small></summary>

```php
public static function createKey($length = 32)
{
	return random_bytes($length);
}
```

</details>


<hr>

#### __get()

```php
public function __get($key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
__get() magic, providing readonly access to some of our protected properties
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
<td>Property name</td>
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
<summary><small>Source: 9 lines (187 - 195)</small></summary>

```php
public function __get($key)
{
	if (in_array($key, ['key', 'digest', 'driver', 'drivers'], true))
	{
		return $this->{$key};
	}

	return null;
}
```

</details>


<hr>

#### __isset()

```php
public function __isset($key) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
__isset() magic, providing checking for some of our protected properties
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
<td>Property name</td>
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
<summary><small>Source: 4 lines (203 - 206)</small></summary>

```php
public function __isset($key): bool
{
	return in_array($key, ['key', 'digest', 'driver', 'drivers'], true);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Encryption/Encryption.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/EncrypterInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Exceptions/EncryptionException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>