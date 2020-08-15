


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Controller.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Config/View.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Database/BaseBuilder.md">next</a></td>
</tr>
</table>







# CodeIgniter 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter</td></tr>
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
<td>framework/system/Controller.php
</td>
</tr>
</table>

 


 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md"><strong>CodeIgniter\HTTP\RequestInterface</strong></a>
</td>
<td>RequestInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/HTTP/ResponseInterface.md"><strong>CodeIgniter\HTTP\ResponseInterface</strong></a>
</td>
<td>ResponseInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md"><strong>CodeIgniter\Validation\Exceptions\ValidationException</strong></a>
</td>
<td>ValidationException</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md"><strong>CodeIgniter\Validation\Validation</strong></a>
</td>
<td>Validation</td>
</tr>
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
<tr>
<td>
<strong>Psr\Log\LoggerInterface</strong>
</td>
<td>LoggerInterface</td>
</tr>
</table>



 
## CodeIgniter\Controller

<table style="text-align:left">
<tr><th>Class</th><td>Controller</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Controller</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Controller
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter
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
<th><a href="#helpers"><strong>helpers</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>An array of helpers to be automatically loaded
upon class instantiation.</td>
</tr>
<tr>
<th><a href="#request"><strong>request</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Instance of the main Request object.</td>
</tr>
<tr>
<th><a href="#response"><strong>response</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Instance of the main response object.</td>
</tr>
<tr>
<th><a href="#logger"><strong>logger</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Instance of logger to use.</td>
</tr>
<tr>
<th><a href="#forceHTTPS"><strong>forceHTTPS</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether HTTPS access should be enforced
for all methods in this controller.</td>
</tr>
<tr>
<th><a href="#validator"><strong>validator</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Once validation has been run,
will hold the Validation instance.</td>
</tr>

<tr>
<th><a href="#initController"><strong>initController</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor.</td>
</tr>
<tr>
<th><a href="#forceHTTPS"><strong>forceHTTPS</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A convenience method to use when you need to ensure that a single
method is reached only via HTTPS. If it isn&#039;t, then a redirect
will happen back to this method and HSTS header will be sent
to have modern browsers transform requests automatically.</td>
</tr>
<tr>
<th><a href="#cachePage"><strong>cachePage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Provides a simple way to tie into the main CodeIgniter class
and tell it how long to cache the current page for.</td>
</tr>
<tr>
<th><a href="#loadHelpers"><strong>loadHelpers</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Handles &quot;auto-loading&quot; helper files.</td>
</tr>
<tr>
<th><a href="#validate"><strong>validate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A shortcut to performing validation on input data. If validation
is not successful, a $errors property will be set on this class.</td>
</tr>

</table>





### Properties


<hr>

#### $helpers

```php
protected $helpers = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
An array of helpers to be automatically loaded
upon class instantiation.
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

#### $request

```php
protected $request;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instance of the main Request object.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\HTTP\IncomingRequest
</td>
</tr>
</table>


<hr>

#### $response

```php
protected $response;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instance of the main response object.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\HTTP\Response
</td>
</tr>
</table>


<hr>

#### $logger

```php
protected $logger;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instance of logger to use.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Log\Logger
</td>
</tr>
</table>


<hr>

#### $forceHTTPS

```php
protected $forceHTTPS = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether HTTPS access should be enforced
for all methods in this controller.
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

#### $validator

```php
protected $validator;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Once validation has been run,
will hold the Validation instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Validation
</td>
</tr>
</table>







### Methods


<hr>

#### initController()

```php
public function initController(RequestInterface $request, ResponseInterface $response, LoggerInterface $logger)
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
<td><code>$request</code></td>
<td><em>\RequestInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$response</code></td>
<td><em>\ResponseInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$logger</code></td>
<td><em>\Psr\Log\LoggerInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>



<details>
<summary><small>Source: 13 lines (115 - 127)</small></summary>

```php
public function initController(RequestInterface $request, ResponseInterface $response, LoggerInterface $logger)
{
	$this->request  = $request;
	$this->response = $response;
	$this->logger   = $logger;

	if ($this->forceHTTPS > 0)
	{
		$this->forceHTTPS($this->forceHTTPS);
	}

	$this->loadHelpers();
}
```

</details>


<hr>

#### forceHTTPS()

```php
protected function forceHTTPS(int $duration = 31536000)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A convenience method to use when you need to ensure that a single
method is reached only via HTTPS. If it isn't, then a redirect
will happen back to this method and HSTS header will be sent
to have modern browsers transform requests automatically.
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
<td><code>$duration</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The number of seconds this link should be
considered secure for. Only with HSTS header.
Default value is 1 year.</td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (143 - 146)</small></summary>

```php
protected function forceHTTPS(int $duration = 31536000)
{
	force_https($duration, $this->request, $this->response);
}
```

</details>


<hr>

#### cachePage()

```php
protected function cachePage(int $time)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides a simple way to tie into the main CodeIgniter class
and tell it how long to cache the current page for.
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
<td><code>$time</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (156 - 159)</small></summary>

```php
protected function cachePage(int $time)
{
	CodeIgniter::cache($time);
}
```

</details>


<hr>

#### loadHelpers()

```php
protected function loadHelpers()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles "auto-loading" helper files.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 12 lines (166 - 177)</small></summary>

```php
protected function loadHelpers()
{
	if (empty($this->helpers))
	{
		return;
	}

	foreach ($this->helpers as $helper)
	{
		helper($helper);
	}
}
```

</details>


<hr>

#### validate()

```php
protected function validate($rules, array $messages = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A shortcut to performing validation on input data. If validation
is not successful, a $errors property will be set on this class.
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
<td><code>$rules</code></td>
<td><em>array<br>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$messages</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>An array of custom error messages</td>
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
<summary><small>Source: 31 lines (190 - 220)</small></summary>

```php
protected function validate($rules, array $messages = []): bool
{
	$this->validator = Services::validation();

	// If you replace the $rules array with the name of the group
	if (is_string($rules))
	{
		$validation = config('Validation');

		// If the rule wasn't found in the \Config\Validation, we
		// should throw an exception so the developer can find it.
		if (! isset($validation->$rules))
		{
			throw ValidationException::forRuleNotFound($rules);
		}

		// If no error message is defined, use the error message in the Config\Validation file
		if (! $messages)
		{
			$errorName = $rules . '_errors';
			$messages  = $validation->$errorName ?? [];
		}

		$rules = $validation->$rules;
	}

	return $this->validator
		->withRequest($this->request)
		->setRules($rules, $messages)
		->run();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Controller.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Config/View.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Database/BaseBuilder.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>