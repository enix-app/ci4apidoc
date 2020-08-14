


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Honeypot/Honeypot.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Exceptions/HoneypotException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Exceptions/I18nException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Honeypot 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Honeypot</td></tr>
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
<td>framework/system/Honeypot/Honeypot.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Exceptions/HoneypotException.md">CodeIgniter\Honeypot\Exceptions\HoneypotException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Honeypot.md">CodeIgniter\Honeypot\Honeypot</a></td></tr>
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
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Exceptions/HoneypotException.md"><strong>CodeIgniter\Honeypot\Exceptions\HoneypotException</strong></a>
</td>
<td>HoneypotException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md"><strong>CodeIgniter\HTTP\RequestInterface</strong></a>
</td>
<td>RequestInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/ResponseInterface.md"><strong>CodeIgniter\HTTP\ResponseInterface</strong></a>
</td>
<td>ResponseInterface</td>
</tr>
</table>



 
## CodeIgniter\Honeypot\Honeypot

<table style="text-align:left">
<tr><th>Class</th><td>Honeypot</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Honeypot\Honeypot</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
class Honeypot
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
<th><a href="#config"><strong>config</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Our configuration.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>


</td>
<td>Constructor.</td>
</tr>
<tr>
<th><a href="#hasContent"><strong>hasContent</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks the request if honeypot field has data.</td>
</tr>
<tr>
<th><a href="#attachHoneypot"><strong>attachHoneypot</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attaches Honeypot template to response.</td>
</tr>
<tr>
<th><a href="#prepareTemplate"><strong>prepareTemplate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Prepares the template by adding label
content and field name.</td>
</tr>

</table>





### Properties


<hr>

#### $config

```php
protected $config;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Our configuration.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\BaseConfig
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
function __construct(BaseConfig $config)
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
<td><em>\BaseConfig
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\type
</td>
</tr>
</table>



<details>
<summary><small>Source: 24 lines (67 - 90)</small></summary>

```php
function __construct(BaseConfig $config)
{
	$this->config = $config;

	if ($this->config->hidden === '')
	{
		throw HoneypotException::forNoHiddenValue();
	}

	if (empty($this->config->container) || strpos($this->config->container, '{template}') === false)
	{
		$this->config->container = '<div style="display:none">{template}</div>';
	}

	if ($this->config->template === '')
	{
		throw HoneypotException::forNoTemplate();
	}

	if ($this->config->name === '')
	{
		throw HoneypotException::forNoNameField();
	}
}
```

</details>


<hr>

#### hasContent()

```php
public function hasContent(RequestInterface $request)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks the request if honeypot field has data.
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
<td><em>\CodeIgniter\HTTP\RequestInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (99 - 102)</small></summary>

```php
public function hasContent(RequestInterface $request)
{
	return ! empty($request->getPost($this->config->name));
}
```

</details>


<hr>

#### attachHoneypot()

```php
public function attachHoneypot(ResponseInterface $response)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attaches Honeypot template to response.
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
<td><code>$response</code></td>
<td><em>\CodeIgniter\HTTP\ResponseInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 8 lines (109 - 116)</small></summary>

```php
public function attachHoneypot(ResponseInterface $response)
{
	$prep_field = $this->prepareTemplate($this->config->template);

	$body = $response->getBody();
	$body = str_ireplace('</form>', $prep_field . '</form>', $body);
	$response->setBody($body);
}
```

</details>


<hr>

#### prepareTemplate()

```php
protected function prepareTemplate(string $template) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prepares the template by adding label
content and field name.
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
<td><code>$template</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 12 lines (125 - 136)</small></summary>

```php
protected function prepareTemplate(string $template): string
{
	$template = str_ireplace('{label}', $this->config->label, $template);
	$template = str_ireplace('{name}', $this->config->name, $template);

	if ($this->config->hidden)
	{
		$template = str_ireplace('{template}', $template, $this->config->container);
	}

	return $template;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Honeypot/Honeypot.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Exceptions/HoneypotException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Exceptions/I18nException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>