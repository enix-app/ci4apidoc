


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/DownloadException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/EmergencyError.md">next</a></td>
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



 

 
## CodeIgniter\Exceptions\DownloadException

<table style="text-align:left">
<tr><th>Class</th><td>DownloadException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Exceptions\DownloadException</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Exceptions\RuntimeException</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ExceptionInterface.md">CodeIgniter\Exceptions\ExceptionInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class DownloadException
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Exceptions
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
<th><a href="#forCannotSetFilePath"><strong>forCannotSetFilePath</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forCannotSetBinary"><strong>forCannotSetBinary</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forNotFoundDownloadSource"><strong>forNotFoundDownloadSource</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forCannotSetCache"><strong>forCannotSetCache</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forCannotSetStatusCode"><strong>forCannotSetStatusCode</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forCannotSetFilePath()

```php
public static function forCannotSetFilePath(string $path)
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
<td><code>$path</code></td>
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
public static function forCannotSetFilePath(string $path)
{
	return new static(lang('HTTP.cannotSetFilepath', [$path]));
}
```

</details>


<hr>

#### forCannotSetBinary()

```php
public static function forCannotSetBinary()
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
public static function forCannotSetBinary()
{
	return new static(lang('HTTP.cannotSetBinary'));
}
```

</details>


<hr>

#### forNotFoundDownloadSource()

```php
public static function forNotFoundDownloadSource()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (22 - 25)</small></summary>

```php
public static function forNotFoundDownloadSource()
{
	return new static(lang('HTTP.notFoundDownloadSource'));
}
```

</details>


<hr>

#### forCannotSetCache()

```php
public static function forCannotSetCache()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (27 - 30)</small></summary>

```php
public static function forCannotSetCache()
{
	return new static(lang('HTTP.cannotSetCache'));
}
```

</details>


<hr>

#### forCannotSetStatusCode()

```php
public static function forCannotSetStatusCode(int $code, string $reason)
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
<td><code>$code</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$reason</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (32 - 35)</small></summary>

```php
public static function forCannotSetStatusCode(int $code, string $reason)
{
	return new static(lang('HTTP.cannotSetStatusCode', [$code, $reason]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/DownloadException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/EmergencyError.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>