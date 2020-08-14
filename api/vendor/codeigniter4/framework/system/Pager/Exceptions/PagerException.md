


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Pager/Exceptions/PagerException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Modules/Modules.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Pager/Pager.md">next</a></td>
</tr>
</table>







# CodeIgniter\Pager\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Pager\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Pager/Exceptions/PagerException.md">CodeIgniter\Pager\Exceptions\PagerException</a></td></tr>
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



 
## CodeIgniter\Pager\Exceptions\PagerException

<table style="text-align:left">
<tr><th>Class</th><td>PagerException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Pager\Exceptions\PagerException</td></tr>
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
<th><a href="#forInvalidTemplate"><strong>forInvalidTemplate</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forInvalidPaginationGroup"><strong>forInvalidPaginationGroup</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forInvalidTemplate()

```php
public static function forInvalidTemplate(string $template = null)
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
<td><code>$template</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (8 - 11)</small></summary>

```php
public static function forInvalidTemplate(string $template = null)
{
	return new static(lang('Pager.invalidTemplate', [$template]));
}
```

</details>


<hr>

#### forInvalidPaginationGroup()

```php
public static function forInvalidPaginationGroup(string $group = null)
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
<td><code>$group</code></td>
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
public static function forInvalidPaginationGroup(string $group = null)
{
	return new static(lang('Pager.invalidPaginationGroup', [$group]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Pager/Exceptions/PagerException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Modules/Modules.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Pager/Pager.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>