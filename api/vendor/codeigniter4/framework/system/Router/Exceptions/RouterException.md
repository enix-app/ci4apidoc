


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Router/Exceptions/RouterException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RedirectException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollection.md">next</a></td>
</tr>
</table>







# CodeIgniter\Router\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Router\Exceptions</td></tr>
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
<td>framework/system/Router/Exceptions/RouterException.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RedirectException.md">CodeIgniter\Router\Exceptions\RedirectException</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RouterException.md">CodeIgniter\Router\Exceptions\RouterException</a></td></tr>
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



 
## CodeIgniter\Router\Exceptions\RouterException

<table style="text-align:left">
<tr><th>Class</th><td>RouterException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Router\Exceptions\RouterException</td></tr>
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
RouterException
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
<th><a href="#forInvalidParameterType"><strong>forInvalidParameterType</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when the actual parameter type does not match
the expected types.</td>
</tr>
<tr>
<th><a href="#forMissingDefaultRoute"><strong>forMissingDefaultRoute</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when a default route is not set.</td>
</tr>

</table>






### Methods


<hr>

#### forInvalidParameterType()

```php
public static function forInvalidParameterType()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when the actual parameter type does not match
the expected types.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\Exceptions\RouterException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (56 - 59)</small></summary>

```php
public static function forInvalidParameterType()
{
	return new static(lang('Router.invalidParameterType'));
}
```

</details>


<hr>

#### forMissingDefaultRoute()

```php
public static function forMissingDefaultRoute()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when a default route is not set.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Router\Exceptions\RouterException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (66 - 69)</small></summary>

```php
public static function forMissingDefaultRoute()
{
	return new static(lang('Router.missingDefaultRoute'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Router/Exceptions/RouterException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RedirectException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Router/RouteCollection.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>