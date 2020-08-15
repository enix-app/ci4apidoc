


 



<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/ResponseInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Response.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/URI.md">next</a></td>
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
<td>framework/system/HTTP/ResponseInterface.php
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



 

 
## CodeIgniter\HTTP\ResponseInterface

<table style="text-align:left">
<tr><th>Interface</th><td>ResponseInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\HTTP\ResponseInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Representation of an outgoing, getServer-side response.
</td></tr>
</table>

<table>
<tr><td>
Per the HTTP specification, this interface includes properties for
each of the following:

- Protocol version
- Status code and reason phrase
- Headers
- Message body
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\HTTP
</td>
</tr>
<tr style="vertical-align:top;">
<th>mixin</th>
<td>\CodeIgniter\HTTP\RedirectResponse
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
<th><a href="#HTTP_CONTINUE"><strong>HTTP_CONTINUE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_SWITCHING_PROTOCOLS"><strong>HTTP_SWITCHING_PROTOCOLS</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_PROCESSING"><strong>HTTP_PROCESSING</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_EARLY_HINTS"><strong>HTTP_EARLY_HINTS</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_OK"><strong>HTTP_OK</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_CREATED"><strong>HTTP_CREATED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_ACCEPTED"><strong>HTTP_ACCEPTED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NONAUTHORITATIVE_INFORMATION"><strong>HTTP_NONAUTHORITATIVE_INFORMATION</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NO_CONTENT"><strong>HTTP_NO_CONTENT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_RESET_CONTENT"><strong>HTTP_RESET_CONTENT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_PARTIAL_CONTENT"><strong>HTTP_PARTIAL_CONTENT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_MULTI_STATUS"><strong>HTTP_MULTI_STATUS</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_ALREADY_REPORTED"><strong>HTTP_ALREADY_REPORTED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_IM_USED"><strong>HTTP_IM_USED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_MULTIPLE_CHOICES"><strong>HTTP_MULTIPLE_CHOICES</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_MOVED_PERMANENTLY"><strong>HTTP_MOVED_PERMANENTLY</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_FOUND"><strong>HTTP_FOUND</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_SEE_OTHER"><strong>HTTP_SEE_OTHER</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NOT_MODIFIED"><strong>HTTP_NOT_MODIFIED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_USE_PROXY"><strong>HTTP_USE_PROXY</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_SWITCH_PROXY"><strong>HTTP_SWITCH_PROXY</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_TEMPORARY_REDIRECT"><strong>HTTP_TEMPORARY_REDIRECT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_PERMANENT_REDIRECT"><strong>HTTP_PERMANENT_REDIRECT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_BAD_REQUEST"><strong>HTTP_BAD_REQUEST</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_UNAUTHORIZED"><strong>HTTP_UNAUTHORIZED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_PAYMENT_REQUIRED"><strong>HTTP_PAYMENT_REQUIRED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_FORBIDDEN"><strong>HTTP_FORBIDDEN</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NOT_FOUND"><strong>HTTP_NOT_FOUND</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_METHOD_NOT_ALLOWED"><strong>HTTP_METHOD_NOT_ALLOWED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NOT_ACCEPTABLE"><strong>HTTP_NOT_ACCEPTABLE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_PROXY_AUTHENTICATION_REQUIRED"><strong>HTTP_PROXY_AUTHENTICATION_REQUIRED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_REQUEST_TIMEOUT"><strong>HTTP_REQUEST_TIMEOUT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_CONFLICT"><strong>HTTP_CONFLICT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_GONE"><strong>HTTP_GONE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_LENGTH_REQUIRED"><strong>HTTP_LENGTH_REQUIRED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_PRECONDITION_FAILED"><strong>HTTP_PRECONDITION_FAILED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_PAYLOAD_TOO_LARGE"><strong>HTTP_PAYLOAD_TOO_LARGE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_URI_TOO_LONG"><strong>HTTP_URI_TOO_LONG</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_UNSUPPORTED_MEDIA_TYPE"><strong>HTTP_UNSUPPORTED_MEDIA_TYPE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_RANGE_NOT_SATISFIABLE"><strong>HTTP_RANGE_NOT_SATISFIABLE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_EXPECTATION_FAILED"><strong>HTTP_EXPECTATION_FAILED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_IM_A_TEAPOT"><strong>HTTP_IM_A_TEAPOT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_MISDIRECTED_REQUEST"><strong>HTTP_MISDIRECTED_REQUEST</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_UNPROCESSABLE_ENTITY"><strong>HTTP_UNPROCESSABLE_ENTITY</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_LOCKED"><strong>HTTP_LOCKED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_FAILED_DEPENDENCY"><strong>HTTP_FAILED_DEPENDENCY</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_TOO_EARLY"><strong>HTTP_TOO_EARLY</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_UPGRADE_REQUIRED"><strong>HTTP_UPGRADE_REQUIRED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_PRECONDITION_REQUIRED"><strong>HTTP_PRECONDITION_REQUIRED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_TOO_MANY_REQUESTS"><strong>HTTP_TOO_MANY_REQUESTS</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_REQUEST_HEADER_FIELDS_TOO_LARGE"><strong>HTTP_REQUEST_HEADER_FIELDS_TOO_LARGE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_UNAVAILABLE_FOR_LEGAL_REASONS"><strong>HTTP_UNAVAILABLE_FOR_LEGAL_REASONS</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_CLIENT_CLOSED_REQUEST"><strong>HTTP_CLIENT_CLOSED_REQUEST</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_INTERNAL_SERVER_ERROR"><strong>HTTP_INTERNAL_SERVER_ERROR</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NOT_IMPLEMENTED"><strong>HTTP_NOT_IMPLEMENTED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_BAD_GATEWAY"><strong>HTTP_BAD_GATEWAY</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_SERVICE_UNAVAILABLE"><strong>HTTP_SERVICE_UNAVAILABLE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_GATEWAY_TIMEOUT"><strong>HTTP_GATEWAY_TIMEOUT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_HTTP_VERSION_NOT_SUPPORTED"><strong>HTTP_HTTP_VERSION_NOT_SUPPORTED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_VARIANT_ALSO_NEGOTIATES"><strong>HTTP_VARIANT_ALSO_NEGOTIATES</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_INSUFFICIENT_STORAGE"><strong>HTTP_INSUFFICIENT_STORAGE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_LOOP_DETECTED"><strong>HTTP_LOOP_DETECTED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NOT_EXTENDED"><strong>HTTP_NOT_EXTENDED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NETWORK_AUTHENTICATION_REQUIRED"><strong>HTTP_NETWORK_AUTHENTICATION_REQUIRED</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#HTTP_NETWORK_CONNECT_TIMEOUT_ERROR"><strong>HTTP_NETWORK_CONNECT_TIMEOUT_ERROR</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>


<tr>
<th><a href="#getStatusCode"><strong>getStatusCode</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Gets the response status code.</td>
</tr>
<tr>
<th><a href="#setStatusCode"><strong>setStatusCode</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return an instance with the specified status code and, optionally, reason phrase.</td>
</tr>
<tr>
<th><a href="#getReason"><strong>getReason</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Gets the response response phrase associated with the status code.</td>
</tr>
<tr>
<th><a href="#setDate"><strong>setDate</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the date header</td>
</tr>
<tr>
<th><a href="#setContentType"><strong>setContentType</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the Content Type header for this response with the mime type
and, optionally, the charset.</td>
</tr>
<tr>
<th><a href="#noCache"><strong>noCache</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the appropriate headers to ensure this response
is not cached by the browsers.</td>
</tr>
<tr>
<th><a href="#setCache"><strong>setCache</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>A shortcut method that allows the developer to set all of the
cache-control headers in one method call.</td>
</tr>
<tr>
<th><a href="#setLastModified"><strong>setLastModified</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the Last-Modified date header.</td>
</tr>
<tr>
<th><a href="#send"><strong>send</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sends the output to the browser.</td>
</tr>

</table>




### Class Constants


#### ::HTTP_CONTINUE

```php
const HTTP_CONTINUE            = 100;
```

#### ::HTTP_SWITCHING_PROTOCOLS

```php
const HTTP_SWITCHING_PROTOCOLS = 101;
```

#### ::HTTP_PROCESSING

```php
const HTTP_PROCESSING          = 102;
```

#### ::HTTP_EARLY_HINTS

```php
const HTTP_EARLY_HINTS         = 103;
```

#### ::HTTP_OK

```php
const HTTP_OK                           = 200;
```

#### ::HTTP_CREATED

```php
const HTTP_CREATED                      = 201;
```

#### ::HTTP_ACCEPTED

```php
const HTTP_ACCEPTED                     = 202;
```

#### ::HTTP_NONAUTHORITATIVE_INFORMATION

```php
const HTTP_NONAUTHORITATIVE_INFORMATION = 203;
```

#### ::HTTP_NO_CONTENT

```php
const HTTP_NO_CONTENT                   = 204;
```

#### ::HTTP_RESET_CONTENT

```php
const HTTP_RESET_CONTENT                = 205;
```

#### ::HTTP_PARTIAL_CONTENT

```php
const HTTP_PARTIAL_CONTENT              = 206;
```

#### ::HTTP_MULTI_STATUS

```php
const HTTP_MULTI_STATUS                 = 207;
```

#### ::HTTP_ALREADY_REPORTED

```php
const HTTP_ALREADY_REPORTED             = 208;
```

#### ::HTTP_IM_USED

```php
const HTTP_IM_USED                      = 226;
```

#### ::HTTP_MULTIPLE_CHOICES

```php
const HTTP_MULTIPLE_CHOICES   = 300;
```

#### ::HTTP_MOVED_PERMANENTLY

```php
const HTTP_MOVED_PERMANENTLY  = 301;
```

#### ::HTTP_FOUND

```php
const HTTP_FOUND              = 302;
```

#### ::HTTP_SEE_OTHER

```php
const HTTP_SEE_OTHER          = 303;
```

#### ::HTTP_NOT_MODIFIED

```php
const HTTP_NOT_MODIFIED       = 304;
```

#### ::HTTP_USE_PROXY

```php
const HTTP_USE_PROXY          = 305;
```

#### ::HTTP_SWITCH_PROXY

```php
const HTTP_SWITCH_PROXY       = 306;
```

#### ::HTTP_TEMPORARY_REDIRECT

```php
const HTTP_TEMPORARY_REDIRECT = 307;
```

#### ::HTTP_PERMANENT_REDIRECT

```php
const HTTP_PERMANENT_REDIRECT = 308;
```

#### ::HTTP_BAD_REQUEST

```php
const HTTP_BAD_REQUEST                     = 400;
```

#### ::HTTP_UNAUTHORIZED

```php
const HTTP_UNAUTHORIZED                    = 401;
```

#### ::HTTP_PAYMENT_REQUIRED

```php
const HTTP_PAYMENT_REQUIRED                = 402;
```

#### ::HTTP_FORBIDDEN

```php
const HTTP_FORBIDDEN                       = 403;
```

#### ::HTTP_NOT_FOUND

```php
const HTTP_NOT_FOUND                       = 404;
```

#### ::HTTP_METHOD_NOT_ALLOWED

```php
const HTTP_METHOD_NOT_ALLOWED              = 405;
```

#### ::HTTP_NOT_ACCEPTABLE

```php
const HTTP_NOT_ACCEPTABLE                  = 406;
```

#### ::HTTP_PROXY_AUTHENTICATION_REQUIRED

```php
const HTTP_PROXY_AUTHENTICATION_REQUIRED   = 407;
```

#### ::HTTP_REQUEST_TIMEOUT

```php
const HTTP_REQUEST_TIMEOUT                 = 408;
```

#### ::HTTP_CONFLICT

```php
const HTTP_CONFLICT                        = 409;
```

#### ::HTTP_GONE

```php
const HTTP_GONE                            = 410;
```

#### ::HTTP_LENGTH_REQUIRED

```php
const HTTP_LENGTH_REQUIRED                 = 411;
```

#### ::HTTP_PRECONDITION_FAILED

```php
const HTTP_PRECONDITION_FAILED             = 412;
```

#### ::HTTP_PAYLOAD_TOO_LARGE

```php
const HTTP_PAYLOAD_TOO_LARGE               = 413;
```

#### ::HTTP_URI_TOO_LONG

```php
const HTTP_URI_TOO_LONG                    = 414;
```

#### ::HTTP_UNSUPPORTED_MEDIA_TYPE

```php
const HTTP_UNSUPPORTED_MEDIA_TYPE          = 415;
```

#### ::HTTP_RANGE_NOT_SATISFIABLE

```php
const HTTP_RANGE_NOT_SATISFIABLE           = 416;
```

#### ::HTTP_EXPECTATION_FAILED

```php
const HTTP_EXPECTATION_FAILED              = 417;
```

#### ::HTTP_IM_A_TEAPOT

```php
const HTTP_IM_A_TEAPOT                     = 418;
```

#### ::HTTP_MISDIRECTED_REQUEST

```php
const HTTP_MISDIRECTED_REQUEST             = 421;
```

#### ::HTTP_UNPROCESSABLE_ENTITY

```php
const HTTP_UNPROCESSABLE_ENTITY            = 422;
```

#### ::HTTP_LOCKED

```php
const HTTP_LOCKED                          = 423;
```

#### ::HTTP_FAILED_DEPENDENCY

```php
const HTTP_FAILED_DEPENDENCY               = 424;
```

#### ::HTTP_TOO_EARLY

```php
const HTTP_TOO_EARLY                       = 425;
```

#### ::HTTP_UPGRADE_REQUIRED

```php
const HTTP_UPGRADE_REQUIRED                = 426;
```

#### ::HTTP_PRECONDITION_REQUIRED

```php
const HTTP_PRECONDITION_REQUIRED           = 428;
```

#### ::HTTP_TOO_MANY_REQUESTS

```php
const HTTP_TOO_MANY_REQUESTS               = 429;
```

#### ::HTTP_REQUEST_HEADER_FIELDS_TOO_LARGE

```php
const HTTP_REQUEST_HEADER_FIELDS_TOO_LARGE = 431;
```

#### ::HTTP_UNAVAILABLE_FOR_LEGAL_REASONS

```php
const HTTP_UNAVAILABLE_FOR_LEGAL_REASONS   = 451;
```

#### ::HTTP_CLIENT_CLOSED_REQUEST

```php
const HTTP_CLIENT_CLOSED_REQUEST           = 499;
```

#### ::HTTP_INTERNAL_SERVER_ERROR

```php
const HTTP_INTERNAL_SERVER_ERROR           = 500;
```

#### ::HTTP_NOT_IMPLEMENTED

```php
const HTTP_NOT_IMPLEMENTED                 = 501;
```

#### ::HTTP_BAD_GATEWAY

```php
const HTTP_BAD_GATEWAY                     = 502;
```

#### ::HTTP_SERVICE_UNAVAILABLE

```php
const HTTP_SERVICE_UNAVAILABLE             = 503;
```

#### ::HTTP_GATEWAY_TIMEOUT

```php
const HTTP_GATEWAY_TIMEOUT                 = 504;
```

#### ::HTTP_HTTP_VERSION_NOT_SUPPORTED

```php
const HTTP_HTTP_VERSION_NOT_SUPPORTED      = 505;
```

#### ::HTTP_VARIANT_ALSO_NEGOTIATES

```php
const HTTP_VARIANT_ALSO_NEGOTIATES         = 506;
```

#### ::HTTP_INSUFFICIENT_STORAGE

```php
const HTTP_INSUFFICIENT_STORAGE            = 507;
```

#### ::HTTP_LOOP_DETECTED

```php
const HTTP_LOOP_DETECTED                   = 508;
```

#### ::HTTP_NOT_EXTENDED

```php
const HTTP_NOT_EXTENDED                    = 510;
```

#### ::HTTP_NETWORK_AUTHENTICATION_REQUIRED

```php
const HTTP_NETWORK_AUTHENTICATION_REQUIRED = 511;
```

#### ::HTTP_NETWORK_CONNECT_TIMEOUT_ERROR

```php
const HTTP_NETWORK_CONNECT_TIMEOUT_ERROR   = 599;
```







### Methods


<hr>

#### getStatusCode()

```php
public function getStatusCode() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets the response status code.
</td></tr>
</table>

<table>
<tr><td>
The status code is a 3-digit integer result code of the getServer's attempt
to understand and satisfy the request.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: line 142</small></summary>

```php
public function getStatusCode(): int;
```

</details>


<hr>

#### setStatusCode()

```php
public function setStatusCode(int $code, string $reason = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return an instance with the specified status code and, optionally, reason phrase.
</td></tr>
</table>

<table>
<tr><td>
If no reason phrase is specified, will default recommended reason phrase for
the response's status code.
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
<td>The 3-digit integer result code to set.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$reason</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The reason phrase to use with the
provided status code; if none is provided, will
default to the IANA name.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>self
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\InvalidArgumentException
</td>
</tr>
</table>



<details>
<summary><small>Source: line 163</small></summary>

```php
public function setStatusCode(int $code, string $reason = '');
```

</details>


<hr>

#### getReason()

```php
public function getReason() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets the response response phrase associated with the status code.
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
<summary><small>Source: line 175</small></summary>

```php
public function getReason(): string;
```

</details>


<hr>

#### setDate()

```php
public function setDate(\DateTime $date)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the date header
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
<td><code>$date</code></td>
<td><em>\DateTime
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\ResponseInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 189</small></summary>

```php
public function setDate(\DateTime $date);
```

</details>


<hr>

#### setContentType()

```php
public function setContentType(string $mime, string $charset = 'UTF-8')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the Content Type header for this response with the mime type
and, optionally, the charset.
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
<td><code>$mime</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$charset</code></td>
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
<td>\ResponseInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 202</small></summary>

```php
public function setContentType(string $mime, string $charset = 'UTF-8');
```

</details>


<hr>

#### noCache()

```php
public function noCache()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the appropriate headers to ensure this response
is not cached by the browsers.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: line 215</small></summary>

```php
public function noCache();
```

</details>


<hr>

#### setCache()

```php
public function setCache(array $options = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A shortcut method that allows the developer to set all of the
cache-control headers in one method call.
</td></tr>
</table>

<table>
<tr><td>
The options array is used to provide the cache-control directives
for the header. It might look something like:

     $options = [
         'max-age'  => 300,
         's-maxage' => 900
         'etag'     => 'abcde',
     ];

Typical options are:
 - etag
 - last-modified
 - max-age
 - s-maxage
 - private
 - public
 - must-revalidate
 - proxy-revalidate
 - no-transform
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
<td><code>$options</code></td>
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
<td>\ResponseInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 247</small></summary>

```php
public function setCache(array $options = []);
```

</details>


<hr>

#### setLastModified()

```php
public function setLastModified($date)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the Last-Modified date header.
</td></tr>
</table>

<table>
<tr><td>
$date can be either a string representation of the date or,
preferably, an instance of DateTime.
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
<td><code>$date</code></td>
<td><em>string<br>\DateTime
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 259</small></summary>

```php
public function setLastModified($date);
```

</details>


<hr>

#### send()

```php
public function send()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sends the output to the browser.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\ResponseInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 271</small></summary>

```php
public function send();
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/ResponseInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Response.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/URI.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>