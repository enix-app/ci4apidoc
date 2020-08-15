


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Encryption/EncrypterInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Email/Email.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Encryption.md">next</a></td>
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
<td>framework/system/Encryption/EncrypterInterface.php
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



 

 
## CodeIgniter\Encryption\EncrypterInterface

<table style="text-align:left">
<tr><th>Interface</th><td>EncrypterInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Encryption\EncrypterInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CodeIgniter Encryption Handler
</td></tr>
</table>

<table>
<tr><td>
Provides two-way keyed encryption
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
<th><a href="#encrypt"><strong>encrypt</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Encrypt - convert plaintext into ciphertext</td>
</tr>
<tr>
<th><a href="#decrypt"><strong>decrypt</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Decrypt - convert ciphertext into plaintext</td>
</tr>

</table>






### Methods


<hr>

#### encrypt()

```php
public function encrypt($data, $params = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Encrypt - convert plaintext into ciphertext
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





<details>
<summary><small>Source: line 58</small></summary>

```php
public function encrypt($data, $params = null);
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
Decrypt - convert ciphertext into plaintext
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





<details>
<summary><small>Source: line 68</small></summary>

```php
public function decrypt($data, $params = null);
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Encryption/EncrypterInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Email/Email.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Encryption.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>