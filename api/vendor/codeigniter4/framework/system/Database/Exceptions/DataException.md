


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Exceptions/DataException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Database.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DatabaseException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Database\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Database\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DataException.md">CodeIgniter\Database\Exceptions\DataException</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DatabaseException.md">CodeIgniter\Database\Exceptions\DatabaseException</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/ExceptionInterface.md">CodeIgniter\Database\Exceptions\ExceptionInterface</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Database\Exceptions\DataException

<table style="text-align:left">
<tr><th>Class</th><td>DataException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\Exceptions\DataException</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Database\Exceptions\RuntimeException</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/ExceptionInterface.md">CodeIgniter\Database\Exceptions\ExceptionInterface</a><br>
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
<th><a href="#forInvalidMethodTriggered"><strong>forInvalidMethodTriggered</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Used by the Model&#039;s trigger() method when the callback cannot be found.</td>
</tr>
<tr>
<th><a href="#forEmptyDataset"><strong>forEmptyDataset</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Used by Model&#039;s insert/update methods when there isn&#039;t
any data to actually work with.</td>
</tr>
<tr>
<th><a href="#forInvalidArgument"><strong>forInvalidArgument</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when an argument for one of the Model&#039;s methods
were empty or otherwise invalid, and they could not be
to work correctly for that method.</td>
</tr>
<tr>
<th><a href="#forInvalidAllowedFields"><strong>forInvalidAllowedFields</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forTableNotFound"><strong>forTableNotFound</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forEmptyInputGiven"><strong>forEmptyInputGiven</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forFindColumnHaveMultipleColumns"><strong>forFindColumnHaveMultipleColumns</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forInvalidMethodTriggered()

```php
public static function forInvalidMethodTriggered(string $method)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used by the Model's trigger() method when the callback cannot be found.
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
<td><code>$method</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Database\Exceptions\DataException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (14 - 17)</small></summary>

```php
public static function forInvalidMethodTriggered(string $method)
{
	return new static(lang('Database.invalidEvent', [$method]));
}
```

</details>


<hr>

#### forEmptyDataset()

```php
public static function forEmptyDataset(string $mode)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used by Model's insert/update methods when there isn't
any data to actually work with.
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
<td><code>$mode</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Database\Exceptions\DataException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (27 - 30)</small></summary>

```php
public static function forEmptyDataset(string $mode)
{
	return new static(lang('Database.emptyDataset', [$mode]));
}
```

</details>


<hr>

#### forInvalidArgument()

```php
public static function forInvalidArgument(string $argument)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when an argument for one of the Model's methods
were empty or otherwise invalid, and they could not be
to work correctly for that method.
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
<td><code>$argument</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Database\Exceptions\DataException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (41 - 44)</small></summary>

```php
public static function forInvalidArgument(string $argument)
{
	return new static(lang('Database.invalidArgument', [$argument]));
}
```

</details>


<hr>

#### forInvalidAllowedFields()

```php
public static function forInvalidAllowedFields(string $model)
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
<td><code>$model</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (46 - 49)</small></summary>

```php
public static function forInvalidAllowedFields(string $model)
{
	return new static(lang('Database.invalidAllowedFields', [$model]));
}
```

</details>


<hr>

#### forTableNotFound()

```php
public static function forTableNotFound(string $table)
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
<td><code>$table</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (51 - 54)</small></summary>

```php
public static function forTableNotFound(string $table)
{
	return new static(lang('Database.tableNotFound', [$table]));
}
```

</details>


<hr>

#### forEmptyInputGiven()

```php
public static function forEmptyInputGiven(string $argument)
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
<td><code>$argument</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (56 - 59)</small></summary>

```php
public static function forEmptyInputGiven(string $argument)
{
	return new static(lang('Database.forEmptyInputGiven', [$argument]));
}
```

</details>


<hr>

#### forFindColumnHaveMultipleColumns()

```php
public static function forFindColumnHaveMultipleColumns()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (61 - 64)</small></summary>

```php
public static function forFindColumnHaveMultipleColumns()
{
	return new static(lang('Database.forFindColumnHaveMultipleColumns'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Exceptions/DataException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Database.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DatabaseException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:09**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>