


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Security/Exceptions/SecurityException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Router/RouterInterface.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Security/Security.md">next</a></td>
</tr>
</table>







# CodeIgniter\Security\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Security\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Security/Exceptions/SecurityException.md">CodeIgniter\Security\Exceptions\SecurityException</a></td></tr>
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



 
## CodeIgniter\Security\Exceptions\SecurityException

<table style="text-align:left">
<tr><th>Class</th><td>SecurityException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Security\Exceptions\SecurityException</td></tr>
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
<th><a href="#forDisallowedAction"><strong>forDisallowedAction</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forDisallowedAction()

```php
public static function forDisallowedAction()
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
public static function forDisallowedAction()
{
	return new static(lang('HTTP.disallowedAction'), 403);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Security/Exceptions/SecurityException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Router/RouterInterface.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Security/Security.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>