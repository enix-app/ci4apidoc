


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/ConfigException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CastException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md">next</a></td>
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



 

 
## CodeIgniter\Exceptions\ConfigException

<table style="text-align:left">
<tr><th>Class</th><td>ConfigException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Exceptions\ConfigException</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md">CodeIgniter\Exceptions\CriticalError</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Exception for automatic logging.
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
<th><a href="#forDisabledMigrations"><strong>forDisabledMigrations</strong>()</a></th>
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

#### forDisabledMigrations()

```php
public static function forDisabledMigrations()
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
public static function forDisabledMigrations()
{
	return new static(lang('Migrations.disabled'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/ConfigException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CastException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>