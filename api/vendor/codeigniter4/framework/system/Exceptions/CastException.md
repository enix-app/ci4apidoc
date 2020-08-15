


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/CastException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/AlertError.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ConfigException.md">next</a></td>
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



 

 
## CodeIgniter\Exceptions\CastException

<table style="text-align:left">
<tr><th>Class</th><td>CastException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Exceptions\CastException</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md">CodeIgniter\Exceptions\CriticalError</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cast Exceptions.
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
<th><a href="#code"><strong>code</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Error code</td>
</tr>

<tr>
<th><a href="#forInvalidJsonFormatException"><strong>forInvalidJsonFormatException</strong>()</a></th>
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
protected $code = 3;
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

#### forInvalidJsonFormatException()

```php
public static function forInvalidJsonFormatException(int $error)
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
<td><code>$error</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 18 lines (17 - 34)</small></summary>

```php
public static function forInvalidJsonFormatException(int $error)
{
	switch($error)
	{
		case JSON_ERROR_DEPTH:
			return new static(lang('Cast.jsonErrorDepth'));
		case JSON_ERROR_STATE_MISMATCH:
			return new static(lang('Cast.jsonErrorStateMismatch'));
		case JSON_ERROR_CTRL_CHAR:
			return new static(lang('Cast.jsonErrorCtrlChar'));
		case JSON_ERROR_SYNTAX:
			return new static(lang('Cast.jsonErrorSyntax'));
		case JSON_ERROR_UTF8:
			return new static(lang('Cast.jsonErrorUtf8'));
		default:
			return new static(lang('Cast.jsonErrorUnknown'));
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/CastException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/AlertError.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ConfigException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>