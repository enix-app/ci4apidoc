


 



<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Exceptions/HTTPException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/DownloadResponse.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/FileCollection.md">next</a></td>
</tr>
</table>







# CodeIgniter\HTTP\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\HTTP\Exceptions</td></tr>
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
<td>framework/system/HTTP/Exceptions/HTTPException.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Exceptions/HTTPException.md">CodeIgniter\HTTP\Exceptions\HTTPException</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ExceptionInterface.md"><strong>CodeIgniter\Exceptions\ExceptionInterface</strong></a>
</td>
<td>ExceptionInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/FrameworkException.md"><strong>CodeIgniter\Exceptions\FrameworkException</strong></a>
</td>
<td>FrameworkException</td>
</tr>
</table>



 
## CodeIgniter\HTTP\Exceptions\HTTPException

<table style="text-align:left">
<tr><th>Class</th><td>HTTPException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\HTTP\Exceptions\HTTPException</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/FrameworkException.md">CodeIgniter\Exceptions\FrameworkException</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ExceptionInterface.md">CodeIgniter\Exceptions\ExceptionInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Things that can go wrong with HTTP
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
<th><a href="#forMissingCurl"><strong>forMissingCurl</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For CurlRequest</td>
</tr>
<tr>
<th><a href="#forSSLCertNotFound"><strong>forSSLCertNotFound</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For CurlRequest</td>
</tr>
<tr>
<th><a href="#forInvalidSSLKey"><strong>forInvalidSSLKey</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For CurlRequest</td>
</tr>
<tr>
<th><a href="#forCurlError"><strong>forCurlError</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For CurlRequest</td>
</tr>
<tr>
<th><a href="#forInvalidNegotiationType"><strong>forInvalidNegotiationType</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For IncomingRequest</td>
</tr>
<tr>
<th><a href="#forInvalidHTTPProtocol"><strong>forInvalidHTTPProtocol</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For Message</td>
</tr>
<tr>
<th><a href="#forEmptySupportedNegotiations"><strong>forEmptySupportedNegotiations</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For Negotiate</td>
</tr>
<tr>
<th><a href="#forInvalidRedirectRoute"><strong>forInvalidRedirectRoute</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For RedirectResponse</td>
</tr>
<tr>
<th><a href="#forMissingResponseStatus"><strong>forMissingResponseStatus</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For Response</td>
</tr>
<tr>
<th><a href="#forInvalidStatusCode"><strong>forInvalidStatusCode</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For Response</td>
</tr>
<tr>
<th><a href="#forUnkownStatusCode"><strong>forUnkownStatusCode</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For Response</td>
</tr>
<tr>
<th><a href="#forUnableToParseURI"><strong>forUnableToParseURI</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For URI</td>
</tr>
<tr>
<th><a href="#forURISegmentOutOfRange"><strong>forURISegmentOutOfRange</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For URI</td>
</tr>
<tr>
<th><a href="#forInvalidPort"><strong>forInvalidPort</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For URI</td>
</tr>
<tr>
<th><a href="#forMalformedQueryString"><strong>forMalformedQueryString</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For URI</td>
</tr>
<tr>
<th><a href="#forAlreadyMoved"><strong>forAlreadyMoved</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For Uploaded file move</td>
</tr>
<tr>
<th><a href="#forInvalidFile"><strong>forInvalidFile</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For Uploaded file move</td>
</tr>
<tr>
<th><a href="#forMoveFailed"><strong>forMoveFailed</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>For Uploaded file move</td>
</tr>

</table>






### Methods


<hr>

#### forMissingCurl()

```php
public static function forMissingCurl()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For CurlRequest
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





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (57 - 60)</small></summary>

```php
public static function forMissingCurl()
{
	return new static(lang('HTTP.missingCurl'));
}
```

</details>


<hr>

#### forSSLCertNotFound()

```php
public static function forSSLCertNotFound(string $cert)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For CurlRequest
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
<td><code>$cert</code></td>
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
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (69 - 72)</small></summary>

```php
public static function forSSLCertNotFound(string $cert)
{
	return new static(lang('HTTP.sslCertNotFound', [$cert]));
}
```

</details>


<hr>

#### forInvalidSSLKey()

```php
public static function forInvalidSSLKey(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For CurlRequest
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
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (81 - 84)</small></summary>

```php
public static function forInvalidSSLKey(string $key)
{
	return new static(lang('HTTP.invalidSSLKey', [$key]));
}
```

</details>


<hr>

#### forCurlError()

```php
public static function forCurlError(string $errorNum, string $error)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For CurlRequest
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
<td><code>$errorNum</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$error</code></td>
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
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (97 - 100)</small></summary>

```php
public static function forCurlError(string $errorNum, string $error)
{
	return new static(lang('HTTP.curlError', [$errorNum, $error]));
}
```

</details>


<hr>

#### forInvalidNegotiationType()

```php
public static function forInvalidNegotiationType(string $type)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For IncomingRequest
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
<td><code>$type</code></td>
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
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (109 - 112)</small></summary>

```php
public static function forInvalidNegotiationType(string $type)
{
	return new static(lang('HTTP.invalidNegotiationType', [$type]));
}
```

</details>


<hr>

#### forInvalidHTTPProtocol()

```php
public static function forInvalidHTTPProtocol(string $protocols)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For Message
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
<td><code>$protocols</code></td>
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
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (121 - 124)</small></summary>

```php
public static function forInvalidHTTPProtocol(string $protocols)
{
	return new static(lang('HTTP.invalidHTTPProtocol', [$protocols]));
}
```

</details>


<hr>

#### forEmptySupportedNegotiations()

```php
public static function forEmptySupportedNegotiations()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For Negotiate
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (131 - 134)</small></summary>

```php
public static function forEmptySupportedNegotiations()
{
	return new static(lang('HTTP.emptySupportedNegotiations'));
}
```

</details>


<hr>

#### forInvalidRedirectRoute()

```php
public static function forInvalidRedirectRoute(string $route)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For RedirectResponse
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
<td><code>$route</code></td>
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
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (143 - 146)</small></summary>

```php
public static function forInvalidRedirectRoute(string $route)
{
	return new static(lang('HTTP.invalidRoute', [$route]));
}
```

</details>


<hr>

#### forMissingResponseStatus()

```php
public static function forMissingResponseStatus()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For Response
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (153 - 156)</small></summary>

```php
public static function forMissingResponseStatus()
{
	return new static(lang('HTTP.missingResponseStatus'));
}
```

</details>


<hr>

#### forInvalidStatusCode()

```php
public static function forInvalidStatusCode(int $code)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For Response
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
<td><code>$code</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (165 - 168)</small></summary>

```php
public static function forInvalidStatusCode(int $code)
{
	return new static(lang('HTTP.invalidStatusCode', [$code]));
}
```

</details>


<hr>

#### forUnkownStatusCode()

```php
public static function forUnkownStatusCode(int $code)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For Response
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
<td><code>$code</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (177 - 180)</small></summary>

```php
public static function forUnkownStatusCode(int $code)
{
	return new static(lang('HTTP.unknownStatusCode', [$code]));
}
```

</details>


<hr>

#### forUnableToParseURI()

```php
public static function forUnableToParseURI(string $uri)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For URI
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
<td><code>$uri</code></td>
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
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (189 - 192)</small></summary>

```php
public static function forUnableToParseURI(string $uri)
{
	return new static(lang('HTTP.cannotParseURI', [$uri]));
}
```

</details>


<hr>

#### forURISegmentOutOfRange()

```php
public static function forURISegmentOutOfRange(int $segment)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For URI
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
<td><code>$segment</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (201 - 204)</small></summary>

```php
public static function forURISegmentOutOfRange(int $segment)
{
	return new static(lang('HTTP.segmentOutOfRange', [$segment]));
}
```

</details>


<hr>

#### forInvalidPort()

```php
public static function forInvalidPort(int $port)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For URI
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
<td><code>$port</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (213 - 216)</small></summary>

```php
public static function forInvalidPort(int $port)
{
	return new static(lang('HTTP.invalidPort', [$port]));
}
```

</details>


<hr>

#### forMalformedQueryString()

```php
public static function forMalformedQueryString()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For URI
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (223 - 226)</small></summary>

```php
public static function forMalformedQueryString()
{
	return new static(lang('HTTP.malformedQueryString'));
}
```

</details>


<hr>

#### forAlreadyMoved()

```php
public static function forAlreadyMoved()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For Uploaded file move
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (233 - 236)</small></summary>

```php
public static function forAlreadyMoved()
{
	return new static(lang('HTTP.alreadyMoved'));
}
```

</details>


<hr>

#### forInvalidFile()

```php
public static function forInvalidFile(string $path = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For Uploaded file move
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
<td><code>$path</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (245 - 248)</small></summary>

```php
public static function forInvalidFile(string $path = null)
{
	return new static(lang('HTTP.invalidFile'));
}
```

</details>


<hr>

#### forMoveFailed()

```php
public static function forMoveFailed(string $source, string $target, string $error)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
For Uploaded file move
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
<td><code>$source</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$target</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$error</code></td>
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
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (259 - 262)</small></summary>

```php
public static function forMoveFailed(string $source, string $target, string $error)
{
	return new static(lang('HTTP.moveFailed', [$source, $target, $error]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Exceptions/HTTPException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/DownloadResponse.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/FileCollection.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>