


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Exceptions/SessionException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Security/Security.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/ArrayHandler.md">next</a></td>
</tr>
</table>







# CodeIgniter\Session\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Session\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Exceptions/SessionException.md">CodeIgniter\Session\Exceptions\SessionException</a></td></tr>
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



 
## CodeIgniter\Session\Exceptions\SessionException

<table style="text-align:left">
<tr><th>Class</th><td>SessionException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Session\Exceptions\SessionException</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/FrameworkException.md">CodeIgniter\Exceptions\FrameworkException</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ExceptionInterface.md">CodeIgniter\Exceptions\ExceptionInterface</a><br>
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
<th><a href="#forMissingDatabaseTable"><strong>forMissingDatabaseTable</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forInvalidSavePath"><strong>forInvalidSavePath</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forWriteProtectedSavePath"><strong>forWriteProtectedSavePath</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forEmptySavepath"><strong>forEmptySavepath</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forInvalidSavePathFormat"><strong>forInvalidSavePathFormat</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forMissingDatabaseTable()

```php
public static function forMissingDatabaseTable()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (8 - 11)</small></summary>

```php
public static function forMissingDatabaseTable()
{
	return new static(lang('Session.missingDatabaseTable'));
}
```

</details>


<hr>

#### forInvalidSavePath()

```php
public static function forInvalidSavePath(string $path = null)
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
<summary><small>Source: 4 lines (13 - 16)</small></summary>

```php
public static function forInvalidSavePath(string $path = null)
{
	return new static(lang('Session.invalidSavePath', [$path]));
}
```

</details>


<hr>

#### forWriteProtectedSavePath()

```php
public static function forWriteProtectedSavePath(string $path = null)
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
<summary><small>Source: 4 lines (18 - 21)</small></summary>

```php
public static function forWriteProtectedSavePath(string $path = null)
{
	return new static(lang('Session.writeProtectedSavePath', [$path]));
}
```

</details>


<hr>

#### forEmptySavepath()

```php
public static function forEmptySavepath()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (23 - 26)</small></summary>

```php
public static function forEmptySavepath()
{
	return new static(lang('Session.emptySavePath'));
}
```

</details>


<hr>

#### forInvalidSavePathFormat()

```php
public static function forInvalidSavePathFormat(string $path)
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
<summary><small>Source: 4 lines (28 - 31)</small></summary>

```php
public static function forInvalidSavePathFormat(string $path)
{
	return new static(lang('Session.invalidSavePathFormat', [$path]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Exceptions/SessionException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Security/Security.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/ArrayHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>