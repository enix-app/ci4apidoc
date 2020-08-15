


 



<table>
<tr>
<td style="width:100%"><em>framework/system/API/ResponseTrait.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/cookie_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/Autoloader.md">next</a></td>
</tr>
</table>







# CodeIgniter\API 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\API</td></tr>
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
<td>framework/system/API/ResponseTrait.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/API/ResponseTrait.md">CodeIgniter\API\ResponseTrait</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Response.md"><strong>CodeIgniter\HTTP\Response</strong></a>
</td>
<td>Response</td>
</tr>
<tr>
<td>
<strong>Config\Format</strong>
</td>
<td>Format</td>
</tr>
</table>



 
## CodeIgniter\API\ResponseTrait

<table style="text-align:left">
<tr><th>Trait</th><td>ResponseTrait</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\API\ResponseTrait</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Response trait.
</td></tr>
</table>

<table>
<tr><td>
Provides common, more readable, methods to provide
consistent HTTP responses under a variety of common
situations when working as an API.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\API
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
<th><a href="#codes"><strong>codes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Allows child classes to override the
status code that is used in their API.</td>
</tr>
<tr>
<th><a href="#format"><strong>format</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>How to format the response data.</td>
</tr>

<tr>
<th><a href="#respond"><strong>respond</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Provides a single, simple method to return an API response, formatted
to match the requested format, with proper content-type and status code.</td>
</tr>
<tr>
<th><a href="#fail"><strong>fail</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used for generic failures that no custom methods exist for.</td>
</tr>
<tr>
<th><a href="#respondCreated"><strong>respondCreated</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used after successfully creating a new resource.</td>
</tr>
<tr>
<th><a href="#respondDeleted"><strong>respondDeleted</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used after a resource has been successfully deleted.</td>
</tr>
<tr>
<th><a href="#respondUpdated"><strong>respondUpdated</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used after a resource has been successfully updated.</td>
</tr>
<tr>
<th><a href="#respondNoContent"><strong>respondNoContent</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used after a command has been successfully executed but there is no
meaningful reply to send back to the client.</td>
</tr>
<tr>
<th><a href="#failUnauthorized"><strong>failUnauthorized</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used when the client is either didn&#039;t send authorization information,
or had bad authorization credentials. User is encouraged to try again
with the proper information.</td>
</tr>
<tr>
<th><a href="#failForbidden"><strong>failForbidden</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used when access is always denied to this resource and no amount
of trying again will help.</td>
</tr>
<tr>
<th><a href="#failNotFound"><strong>failNotFound</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used when a specified resource cannot be found.</td>
</tr>
<tr>
<th><a href="#failValidationError"><strong>failValidationError</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used when the data provided by the client cannot be validated.</td>
</tr>
<tr>
<th><a href="#failResourceExists"><strong>failResourceExists</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Use when trying to create a new resource and it already exists.</td>
</tr>
<tr>
<th><a href="#failResourceGone"><strong>failResourceGone</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Use when a resource was previously deleted. This is different than
Not Found, because here we know the data previously existed, but is now gone,
where Not Found means we simply cannot find any information about it.</td>
</tr>
<tr>
<th><a href="#failTooManyRequests"><strong>failTooManyRequests</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used when the user has made too many requests for the resource recently.</td>
</tr>
<tr>
<th><a href="#failServerError"><strong>failServerError</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used when there is a server error.</td>
</tr>
<tr>
<th><a href="#format"><strong>format</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Handles formatting a response. Currently makes some heavy assumptions
and needs updating! :)</td>
</tr>
<tr>
<th><a href="#setResponseFormat"><strong>setResponseFormat</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the format the response should be in.</td>
</tr>

</table>





### Properties


<hr>

#### $codes

```php
protected $codes = [
	'created'                   => 201,
	'deleted'                   => 200,
	'updated'                   => 200,
	'no_content'                => 204,
	'invalid_request'           => 400,
	'unsupported_response_type' => 400,
	'invalid_scope'             => 400,
	'temporarily_unavailable'   => 400,
	'invalid_grant'             => 400,
	'invalid_credentials'       => 400,
	'invalid_refresh'           => 400,
	'no_data'                   => 400,
	'invalid_data'              => 400,
	'access_denied'             => 401,
	'unauthorized'              => 401,
	'invalid_client'            => 401,
	'forbidden'                 => 403,
	'resource_not_found'        => 404,
	'not_acceptable'            => 406,
	'resource_exists'           => 409,
	'conflict'                  => 409,
	'resource_gone'             => 410,
	'payload_too_large'         => 413,
	'unsupported_media_type'    => 415,
	'too_many_requests'         => 429,
	'server_error'              => 500,
	'unsupported_grant_type'    => 501,
	'not_implemented'           => 501,
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows child classes to override the
status code that is used in their API.
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

#### $format

```php
protected $format = 'json';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
How to format the response data.
</td></tr>
</table>

<table>
<tr><td>
Either 'json' or 'xml'. If blank will be
determine through content negotiation.
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

#### respond()

```php
public function respond($data = null, int $status = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides a single, simple method to return an API response, formatted
to match the requested format, with proper content-type and status code.
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
<td><em>array<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$status</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 23 lines (117 - 139)</small></summary>

```php
public function respond($data = null, int $status = null, string $message = '')
{
	// If data is null and status code not provided, exit and bail
	if ($data === null && $status === null)
	{
		$status = 404;

		// Create the output var here in case of $this->response([]);
		$output = null;
	} // If data is null but status provided, keep the output empty.
	elseif ($data === null && is_numeric($status))
	{
		$output = null;
	}
	else
	{
		$status = empty($status) ? 200 : $status;
		$output = $this->format($data);
	}

	return $this->response->setBody($output)
					->setStatusCode($status, $message);
}
```

</details>


<hr>

#### fail()

```php
public function fail($messages, int $status = 400, string $code = null, string $customMessage = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used for generic failures that no custom methods exist for.
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
<td><code>$messages</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$status</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td>HTTP status code</td>
</tr>

<tr>
<td>3.</td>
<td><code>$code</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td>Custom, API-specific, error code</td>
</tr>

<tr>
<td>4.</td>
<td><code>$customMessage</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (153 - 167)</small></summary>

```php
public function fail($messages, int $status = 400, string $code = null, string $customMessage = '')
{
	if (! is_array($messages))
	{
		$messages = ['error' => $messages];
	}

	$response = [
		'status'   => $status,
		'error'    => $code === null ? $status : $code,
		'messages' => $messages,
	];

	return $this->respond($response, $status, $customMessage);
}
```

</details>


<hr>

#### respondCreated()

```php
public function respondCreated($data = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used after successfully creating a new resource.
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
<td><em>mixed
</em></td>
<td>false</td>
<td>Data.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Message.</td>
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
<summary><small>Source: 4 lines (182 - 185)</small></summary>

```php
public function respondCreated($data = null, string $message = '')
{
	return $this->respond($data, $this->codes['created'], $message);
}
```

</details>


<hr>

#### respondDeleted()

```php
public function respondDeleted($data = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used after a resource has been successfully deleted.
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
<td><em>mixed
</em></td>
<td>false</td>
<td>Data.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Message.</td>
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
<summary><small>Source: 4 lines (197 - 200)</small></summary>

```php
public function respondDeleted($data = null, string $message = '')
{
	return $this->respond($data, $this->codes['deleted'], $message);
}
```

</details>


<hr>

#### respondUpdated()

```php
public function respondUpdated($data = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used after a resource has been successfully updated.
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
<td><em>mixed
</em></td>
<td>false</td>
<td>Data.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Message.</td>
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
<summary><small>Source: 4 lines (210 - 213)</small></summary>

```php
public function respondUpdated($data = null, string $message = '')
{
	return $this->respond($data, $this->codes['updated'], $message);
}
```

</details>


<hr>

#### respondNoContent()

```php
public function respondNoContent(string $message = 'No Content')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used after a command has been successfully executed but there is no
meaningful reply to send back to the client.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Message.</td>
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
<summary><small>Source: 4 lines (225 - 228)</small></summary>

```php
public function respondNoContent(string $message = 'No Content')
{
	return $this->respond(null, $this->codes['no_content'], $message);
}
```

</details>


<hr>

#### failUnauthorized()

```php
public function failUnauthorized(string $description = 'Unauthorized', string $code = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used when the client is either didn't send authorization information,
or had bad authorization credentials. User is encouraged to try again
with the proper information.
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
<td><code>$description</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$code</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (243 - 246)</small></summary>

```php
public function failUnauthorized(string $description = 'Unauthorized', string $code = null, string $message = '')
{
	return $this->fail($description, $this->codes['unauthorized'], $code, $message);
}
```

</details>


<hr>

#### failForbidden()

```php
public function failForbidden(string $description = 'Forbidden', string $code = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used when access is always denied to this resource and no amount
of trying again will help.
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
<td><code>$description</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$code</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (260 - 263)</small></summary>

```php
public function failForbidden(string $description = 'Forbidden', string $code = null, string $message = '')
{
	return $this->fail($description, $this->codes['forbidden'], $code, $message);
}
```

</details>


<hr>

#### failNotFound()

```php
public function failNotFound(string $description = 'Not Found', string $code = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used when a specified resource cannot be found.
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
<td><code>$description</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$code</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (276 - 279)</small></summary>

```php
public function failNotFound(string $description = 'Not Found', string $code = null, string $message = '')
{
	return $this->fail($description, $this->codes['resource_not_found'], $code, $message);
}
```

</details>


<hr>

#### failValidationError()

```php
public function failValidationError(string $description = 'Bad Request', string $code = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used when the data provided by the client cannot be validated.
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
<td><code>$description</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$code</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (292 - 295)</small></summary>

```php
public function failValidationError(string $description = 'Bad Request', string $code = null, string $message = '')
{
	return $this->fail($description, $this->codes['invalid_data'], $code, $message);
}
```

</details>


<hr>

#### failResourceExists()

```php
public function failResourceExists(string $description = 'Conflict', string $code = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Use when trying to create a new resource and it already exists.
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
<td><code>$description</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$code</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (308 - 311)</small></summary>

```php
public function failResourceExists(string $description = 'Conflict', string $code = null, string $message = '')
{
	return $this->fail($description, $this->codes['resource_exists'], $code, $message);
}
```

</details>


<hr>

#### failResourceGone()

```php
public function failResourceGone(string $description = 'Gone', string $code = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Use when a resource was previously deleted. This is different than
Not Found, because here we know the data previously existed, but is now gone,
where Not Found means we simply cannot find any information about it.
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
<td><code>$description</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$code</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (326 - 329)</small></summary>

```php
public function failResourceGone(string $description = 'Gone', string $code = null, string $message = '')
{
	return $this->fail($description, $this->codes['resource_gone'], $code, $message);
}
```

</details>


<hr>

#### failTooManyRequests()

```php
public function failTooManyRequests(string $description = 'Too Many Requests', string $code = null, string $message = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used when the user has made too many requests for the resource recently.
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
<td><code>$description</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$code</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (342 - 345)</small></summary>

```php
public function failTooManyRequests(string $description = 'Too Many Requests', string $code = null, string $message = '')
{
	return $this->fail($description, $this->codes['too_many_requests'], $code, $message);
}
```

</details>


<hr>

#### failServerError()

```php
public function failServerError(string $description = 'Internal Server Error', string $code = null, string $message = '') : Response
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used when there is a server error.
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
<td><code>$description</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The error message to show the user.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$code</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td>A custom, API-specific, error code.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>A custom "reason" message to return.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Response
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (358 - 361)</small></summary>

```php
public function failServerError(string $description = 'Internal Server Error', string $code = null, string $message = ''): Response
{
	return $this->fail($description, $this->codes['server_error'], $code, $message);
}
```

</details>


<hr>

#### format()

```php
protected function format($data = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles formatting a response. Currently makes some heavy assumptions
and needs updating! :)
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
<td><em>string<br>array<br>null
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
<summary><small>Source: 41 lines (375 - 415)</small></summary>

```php
protected function format($data = null)
{
	// If the data is a string, there's not much we can do to it...
	if (is_string($data))
	{
		// The content type should be text/... and not application/...
		$contentType = $this->response->getHeaderLine('Content-Type');
		$contentType = str_replace('application/json', 'text/html', $contentType);
		$contentType = str_replace('application/', 'text/', $contentType);
		$this->response->setContentType($contentType);

		return $data;
	}

	$config = new Format();
	$format = "application/$this->format";

	// Determine correct response type through content negotiation if not explicitly declared
	if (empty($this->format) || ! in_array($this->format, ['json', 'xml']))
	{
		$format = $this->request->negotiate('media', $config->supportedResponseFormats, false);
	}

	$this->response->setContentType($format);

	// if we don't have a formatter, make one
	if (! isset($this->formatter))
	{
		// if no formatter, use the default
		$this->formatter = $config->getFormatter($format);
	}

	if ($format !== 'application/json')
	{
		// Recursively convert objects into associative arrays
		// Conversion not required for JSONFormatter
		$data = json_decode(json_encode($data), true);
	}

	return $this->formatter->format($data);
}
```

</details>


<hr>

#### setResponseFormat()

```php
public function setResponseFormat(string $format = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the format the response should be in.
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
<td><code>$format</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (424 - 429)</small></summary>

```php
public function setResponseFormat(string $format = null)
{
	$this->format = strtolower($format);

	return $this;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/API/ResponseTrait.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/cookie_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/Autoloader.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>