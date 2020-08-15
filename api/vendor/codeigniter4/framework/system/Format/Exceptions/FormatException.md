


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Format/Exceptions/FormatException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Filters/Honeypot.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Format/FormatterInterface.md">next</a></td>
</tr>
</table>







# CodeIgniter\Format\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Format\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Format/Exceptions/FormatException.md">CodeIgniter\Format\Exceptions\FormatException</a></td></tr>
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
</table>



 
## CodeIgniter\Format\Exceptions\FormatException

<table style="text-align:left">
<tr><th>Class</th><td>FormatException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Format\Exceptions\FormatException</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Format\Exceptions\RuntimeException</a></td></tr>
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
<th><a href="#forInvalidJSON"><strong>forInvalidJSON</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forMissingExtension"><strong>forMissingExtension</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>This will never be thrown in travis-ci</td>
</tr>

</table>






### Methods


<hr>

#### forInvalidJSON()

```php
public static function forInvalidJSON(string $error = null)
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
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (7 - 10)</small></summary>

```php
public static function forInvalidJSON(string $error = null)
{
	return new static(lang('Format.invalidJSON', [$error]));
}
```

</details>


<hr>

#### forMissingExtension()

```php
public static function forMissingExtension()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
This will never be thrown in travis-ci
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
</td>
</tr>
</table>










<details>
<summary><small>Source: 4 lines (17 - 20)</small></summary>

```php
public static function forMissingExtension()
{
	return new static(lang('Format.missingExtension'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Format/Exceptions/FormatException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Filters/Honeypot.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Format/FormatterInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>