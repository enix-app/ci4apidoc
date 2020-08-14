


 



<table>
<tr>
<td style="width:100%"><em>framework/system/View/Plugins.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Parser.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">next</a></td>
</tr>
</table>







# CodeIgniter\View 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\View</td></tr>
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
<td>framework/system/View/Plugins.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Cell.md">CodeIgniter\View\Cell</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md">CodeIgniter\View\Exceptions\ViewException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Filters.md">CodeIgniter\View\Filters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Parser.md">CodeIgniter\View\Parser</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Plugins.md">CodeIgniter\View\Plugins</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">CodeIgniter\View\RendererInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Table.md">CodeIgniter\View\Table</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/View.md">CodeIgniter\View\View</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\View\Plugins

<table style="text-align:left">
<tr><th>Class</th><td>Plugins</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\View\Plugins</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
View plugins
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
<th><a href="#currentURL"><strong>currentURL</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Wrap helper function to use as view plugin.</td>
</tr>
<tr>
<th><a href="#previousURL"><strong>previousURL</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Wrap helper function to use as view plugin.</td>
</tr>
<tr>
<th><a href="#mailto"><strong>mailto</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Wrap helper function to use as view plugin.</td>
</tr>
<tr>
<th><a href="#safeMailto"><strong>safeMailto</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Wrap helper function to use as view plugin.</td>
</tr>
<tr>
<th><a href="#lang"><strong>lang</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Wrap helper function to use as view plugin.</td>
</tr>
<tr>
<th><a href="#ValidationErrors"><strong>ValidationErrors</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Wrap helper function to use as view plugin.</td>
</tr>
<tr>
<th><a href="#route"><strong>route</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Wrap helper function to use as view plugin.</td>
</tr>
<tr>
<th><a href="#siteURL"><strong>siteURL</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Wrap helper function to use as view plugin.</td>
</tr>

</table>






### Methods


<hr>

#### currentURL()

```php
public static function currentURL()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrap helper function to use as view plugin.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>\CodeIgniter\HTTP\URI
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (53 - 56)</small></summary>

```php
public static function currentURL()
{
	return current_url();
}
```

</details>


<hr>

#### previousURL()

```php
public static function previousURL()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrap helper function to use as view plugin.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\URI<br>mixed<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (65 - 68)</small></summary>

```php
public static function previousURL()
{
	return previous_url();
}
```

</details>


<hr>

#### mailto()

```php
public static function mailto(array $params = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrap helper function to use as view plugin.
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
<td><code>$params</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (79 - 86)</small></summary>

```php
public static function mailto(array $params = []): string
{
	$email = $params['email'] ?? '';
	$title = $params['title'] ?? '';
	$attrs = $params['attributes'] ?? '';

	return mailto($email, $title, $attrs);
}
```

</details>


<hr>

#### safeMailto()

```php
public static function safeMailto(array $params = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrap helper function to use as view plugin.
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
<td><code>$params</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (97 - 104)</small></summary>

```php
public static function safeMailto(array $params = []): string
{
	$email = $params['email'] ?? '';
	$title = $params['title'] ?? '';
	$attrs = $params['attributes'] ?? '';

	return safe_mailto($email, $title, $attrs);
}
```

</details>


<hr>

#### lang()

```php
public static function lang(array $params = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrap helper function to use as view plugin.
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
<td><code>$params</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (115 - 120)</small></summary>

```php
public static function lang(array $params = []): string
{
	$line = array_shift($params);

	return lang($line, $params);
}
```

</details>


<hr>

#### ValidationErrors()

```php
public static function ValidationErrors(array $params = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrap helper function to use as view plugin.
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
<td><code>$params</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (131 - 140)</small></summary>

```php
public static function ValidationErrors(array $params = []): string
{
	$validator = \Config\Services::validation();
	if (empty($params))
	{
		return $validator->listErrors();
	}

	return $validator->showError($params['field']);
}
```

</details>


<hr>

#### route()

```php
public static function route(array $params = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrap helper function to use as view plugin.
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
<td><code>$params</code></td>
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
<td>string<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (151 - 154)</small></summary>

```php
public static function route(array $params = [])
{
	return route_to(...$params);
}
```

</details>


<hr>

#### siteURL()

```php
public static function siteURL(array $params = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrap helper function to use as view plugin.
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
<td><code>$params</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (165 - 168)</small></summary>

```php
public static function siteURL(array $params = []): string
{
	return site_url(...$params);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/View/Plugins.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Parser.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>