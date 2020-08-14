


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/ModelException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/FrameworkException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/PageNotFoundException.md">next</a></td>
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



 

 
## CodeIgniter\Exceptions\ModelException

<table style="text-align:left">
<tr><th>Class</th><td>ModelException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Exceptions\ModelException</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/FrameworkException.md">CodeIgniter\Exceptions\FrameworkException</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Model Exceptions.
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
<th><a href="#forNoPrimaryKey"><strong>forNoPrimaryKey</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forNoDateFormat"><strong>forNoDateFormat</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forNoPrimaryKey()

```php
public static function forNoPrimaryKey(string $modelName)
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
<td><code>$modelName</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (9 - 12)</small></summary>

```php
public static function forNoPrimaryKey(string $modelName)
{
	return new static(lang('Database.noPrimaryKey', [$modelName]));
}
```

</details>


<hr>

#### forNoDateFormat()

```php
public static function forNoDateFormat(string $modelName)
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
<td><code>$modelName</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (14 - 17)</small></summary>

```php
public static function forNoDateFormat(string $modelName)
{
	return new static(lang('Database.noDateFormat', [$modelName]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Exceptions/ModelException.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/FrameworkException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/PageNotFoundException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>