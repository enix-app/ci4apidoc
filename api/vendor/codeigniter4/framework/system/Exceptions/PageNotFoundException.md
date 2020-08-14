


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/PageNotFoundException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ModelException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/AlertError.md">CodeIgniter\Exceptions\AlertError</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CastException.md">CodeIgniter\Exceptions\CastException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ConfigException.md">CodeIgniter\Exceptions\ConfigException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md">CodeIgniter\Exceptions\CriticalError</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/DownloadException.md">CodeIgniter\Exceptions\DownloadException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/EmergencyError.md">CodeIgniter\Exceptions\EmergencyError</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ExceptionInterface.md">CodeIgniter\Exceptions\ExceptionInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/FrameworkException.md">CodeIgniter\Exceptions\FrameworkException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ModelException.md">CodeIgniter\Exceptions\ModelException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/PageNotFoundException.md">CodeIgniter\Exceptions\PageNotFoundException</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Exceptions\PageNotFoundException

<table style="text-align:left">
<tr><th>Class</th><td>PageNotFoundException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Exceptions\PageNotFoundException</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Exceptions\OutOfBoundsException</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ExceptionInterface.md">CodeIgniter\Exceptions\ExceptionInterface</a><br>
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
<th><a href="#code"><strong>code</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Error code</td>
</tr>

<tr>
<th><a href="#forPageNotFound"><strong>forPageNotFound</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forEmptyController"><strong>forEmptyController</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forControllerNotFound"><strong>forControllerNotFound</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forMethodNotFound"><strong>forMethodNotFound</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>





### Properties


<hr>

#### $code

```php
protected $code = 404;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Error code
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







### Methods


<hr>

#### forPageNotFound()

```php
public static function forPageNotFound(string $message = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (12 - 15)</small></summary>

```php
public static function forPageNotFound(string $message = null)
{
	return new static($message ?? lang('HTTP.pageNotFound'));
}
```

</details>


<hr>

#### forEmptyController()

```php
public static function forEmptyController()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (17 - 20)</small></summary>

```php
public static function forEmptyController()
{
	return new static(lang('HTTP.emptyController'));
}
```

</details>


<hr>

#### forControllerNotFound()

```php
public static function forControllerNotFound(string $controller, string $method)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td><code>$controller</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$method</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (22 - 25)</small></summary>

```php
public static function forControllerNotFound(string $controller, string $method)
{
	return new static(lang('HTTP.controllerNotFound', [$controller, $method]));
}
```

</details>


<hr>

#### forMethodNotFound()

```php
public static function forMethodNotFound(string $method)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td><code>$method</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (27 - 30)</small></summary>

```php
public static function forMethodNotFound(string $method)
{
	return new static(lang('HTTP.methodNotFound', [$method]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/PageNotFoundException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ModelException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>