


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Filters/Honeypot.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Filters.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/Exceptions/FormatException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Filters 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Filters</td></tr>
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
<td>framework/system/Filters/Honeypot.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/CSRF.md">CodeIgniter\Filters\CSRF</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/DebugToolbar.md">CodeIgniter\Filters\DebugToolbar</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Exceptions/FilterException.md">CodeIgniter\Filters\Exceptions\FilterException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/FilterInterface.md">CodeIgniter\Filters\FilterInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Filters.md">CodeIgniter\Filters\Filters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Honeypot.md">CodeIgniter\Filters\Honeypot</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
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
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
</table>



 
## CodeIgniter\Filters\Honeypot

<table style="text-align:left">
<tr><th>Class</th><td>Honeypot</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Filters\Honeypot</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/FilterInterface.md">CodeIgniter\Filters\FilterInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Honeypot filter
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
<th><a href="#before"><strong>before</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks if Honeypot field is empty; if not
then the requester is a bot</td>
</tr>
<tr>
<th><a href="#after"><strong>after</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attach a honeypot to the current response.</td>
</tr>

</table>






### Methods


<hr>

#### before()

```php
public function before(RequestInterface $request, $arguments = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks if Honeypot field is empty; if not
then the requester is a bot
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

<tr>
<td>2.</td>
<td><code>$arguments</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
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





<details>
<summary><small>Source: 8 lines (62 - 69)</small></summary>

```php
public function before(RequestInterface $request, $arguments = null)
{
	$honeypot = Services::honeypot(new \Config\Honeypot());
	if ($honeypot->hasContent($request))
	{
		throw HoneypotException::isBot();
	}
}
```

</details>


<hr>

#### after()

```php
public function after(RequestInterface $request, ResponseInterface $response, $arguments = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attach a honeypot to the current response.
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

<tr>
<td>2.</td>
<td><code>$response</code></td>
<td><em>\CodeIgniter\HTTP\ResponseInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$arguments</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
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





<details>
<summary><small>Source: 5 lines (80 - 84)</small></summary>

```php
public function after(RequestInterface $request, ResponseInterface $response, $arguments = null)
{
	$honeypot = Services::honeypot(new \Config\Honeypot());
	$honeypot->attachHoneypot($response);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Filters/Honeypot.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Filters.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/Exceptions/FormatException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>