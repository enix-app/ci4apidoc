


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Files/Exceptions/FileNotFoundException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/File.md">next</a></td>
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



 
## CodeIgniter\Files\Exceptions\FileNotFoundException

<table style="text-align:left">
<tr><th>Class</th><td>FileNotFoundException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Files\Exceptions\FileNotFoundException</td></tr>
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
<th><a href="#forFileNotFound"><strong>forFileNotFound</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forFileNotFound()

```php
public static function forFileNotFound(string $path)
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
<summary><small>Source: 4 lines (7 - 10)</small></summary>

```php
public static function forFileNotFound(string $path)
{
	return new static(lang('Files.fileNotFound', [$path]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Files/Exceptions/FileNotFoundException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/File.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>