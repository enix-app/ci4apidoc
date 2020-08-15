


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Files/Exceptions/FileException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/PageNotFoundException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileNotFoundException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Files\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Files\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileException.md">CodeIgniter\Files\Exceptions\FileException</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileNotFoundException.md">CodeIgniter\Files\Exceptions\FileNotFoundException</a></td></tr>
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



 
## CodeIgniter\Files\Exceptions\FileException

<table style="text-align:left">
<tr><th>Class</th><td>FileException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Files\Exceptions\FileException</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Files\Exceptions\RuntimeException</a></td></tr>
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
<th><a href="#forUnableToMove"><strong>forUnableToMove</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forUnableToMove()

```php
public static function forUnableToMove(string $from = null, string $to = null, string $error = null)
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
<td><code>$from</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$to</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$error</code></td>
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
public static function forUnableToMove(string $from = null, string $to = null, string $error = null)
{
	return new static(lang('Files.cannotMove', [$from, $to, $error]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Files/Exceptions/FileException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/PageNotFoundException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileNotFoundException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>