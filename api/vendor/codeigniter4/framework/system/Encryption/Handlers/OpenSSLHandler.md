


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Encryption/Handlers/OpenSSLHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/BaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Entity.md">next</a></td>
</tr>
</table>







# CodeIgniter\Encryption\Handlers 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Encryption\Handlers</td></tr>
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
<td>framework/system/Encryption/Handlers/OpenSSLHandler.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/BaseHandler.md">CodeIgniter\Encryption\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/OpenSSLHandler.md">CodeIgniter\Encryption\Handlers\OpenSSLHandler</a></td></tr>
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Exceptions/EncryptionException.md"><strong>CodeIgniter\Encryption\Exceptions\EncryptionException</strong></a>
</td>
<td>EncryptionException</td>
</tr>
</table>



 
## CodeIgniter\Encryption\Handlers\OpenSSLHandler

<table style="text-align:left">
<tr><th>Class</th><td>OpenSSLHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Encryption\Handlers\OpenSSLHandler</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/BaseHandler.md">CodeIgniter\Encryption\Handlers\BaseHandler</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Encryption handling for OpenSSL library
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
<th><a href="#digest"><strong>digest</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>HMAC digest to use</td>
</tr>
<tr>
<th><a href="#cipher"><strong>cipher</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cipher to use</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Initialize OpenSSL, remembering parameters</td>
</tr>
<tr>
<th><a href="#encrypt"><strong>encrypt</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Encrypt plaintext, with optional HMAC and base64 encoding</td>
</tr>
<tr>
<th><a href="#decrypt"><strong>decrypt</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Decrypt ciphertext, with optional HMAC and base64 encoding</td>
</tr>

</table>





### Properties


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

#### $cipher

```php
protected $cipher = 'AES-256-CTR';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cipher to use
</td></tr>
</table>


</details>



<table style="text-align:left">
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
Initialize OpenSSL, remembering parameters
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
<td><em>\CodeIgniter\Config\BaseConfig<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Encryption\Exceptions\EncryptionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (69 - 72)</small></summary>

```php
public function __construct(BaseConfig $config = null)
{
	parent::__construct($config);
}
```

</details>


<hr>

#### encrypt()

```php
public function encrypt($data, $params = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Encrypt plaintext, with optional HMAC and base64 encoding
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
<td><code>$data</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Input data</td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Over-ridden parameters, specifically the key</td>
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
<td>\CodeIgniter\Encryption\Exceptions\EncryptionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 39 lines (83 - 121)</small></summary>

```php
public function encrypt($data, $params = null)
{
	// Allow key override
	if ($params)
	{
		if (isset($params['key']))
		{
			$this->key = $params['key'];
		}
		else
		{
			$this->key = $params;
		}
	}

	if (empty($this->key))
	{
		throw EncryptionException::forNeedsStarterKey();
	}

	// derive a secret key
	$secret = \hash_hkdf($this->digest, $this->key);

	// basic encryption
	$iv = ($iv_size = \openssl_cipher_iv_length($this->cipher)) ? \openssl_random_pseudo_bytes($iv_size) : null;

	$data = \openssl_encrypt($data, $this->cipher, $secret, OPENSSL_RAW_DATA, $iv);

	if ($data === false)
	{
		throw EncryptionException::forEncryptionFailed();
	}

	$result = $iv . $data;

	$hmacKey = \hash_hmac($this->digest, $result, $secret, true);

	return $hmacKey . $result;
}
```

</details>


<hr>

#### decrypt()

```php
public function decrypt($data, $params = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Decrypt ciphertext, with optional HMAC and base64 encoding
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
<td><code>$data</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Encrypted data</td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Over-ridden parameters, specifically the key</td>
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
<td>\CodeIgniter\Encryption\Exceptions\EncryptionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 44 lines (134 - 177)</small></summary>

```php
public function decrypt($data, $params = null)
{
	// Allow key override
	if ($params)
	{
		if (isset($params['key']))
		{
			$this->key = $params['key'];
		}
		else
		{
			$this->key = $params;
		}
	}

	if (empty($this->key))
	{
		throw EncryptionException::forNeedsStarterKey();
	}

	// derive a secret key
	$secret = \hash_hkdf($this->digest, $this->key);

	$hmacLength = self::substr($this->digest, 3) / 8;
	$hmacKey    = self::substr($data, 0, $hmacLength);
	$data       = self::substr($data, $hmacLength);
	$hmacCalc   = \hash_hmac($this->digest, $data, $secret, true);
	if (! hash_equals($hmacKey, $hmacCalc))
	{
		throw EncryptionException::forAuthenticationFailed();
	}

	if ($iv_size = \openssl_cipher_iv_length($this->cipher))
	{
		$iv   = self::substr($data, 0, $iv_size);
		$data = self::substr($data, $iv_size);
	}
	else
	{
		$iv = null;
	}

	return \openssl_decrypt($data, $this->cipher, $secret, OPENSSL_RAW_DATA, $iv);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Encryption/Handlers/OpenSSLHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/BaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Entity.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>