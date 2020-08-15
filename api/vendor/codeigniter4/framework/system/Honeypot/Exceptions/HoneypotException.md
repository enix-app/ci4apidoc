


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Honeypot/Exceptions/HoneypotException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/UserAgent.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Honeypot.md">next</a></td>
</tr>
</table>







# CodeIgniter\Honeypot\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Honeypot\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Exceptions/HoneypotException.md">CodeIgniter\Honeypot\Exceptions\HoneypotException</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ConfigException.md"><strong>CodeIgniter\Exceptions\ConfigException</strong></a>
</td>
<td>ConfigException</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ExceptionInterface.md"><strong>CodeIgniter\Exceptions\ExceptionInterface</strong></a>
</td>
<td>ExceptionInterface</td>
</tr>
</table>



 
## CodeIgniter\Honeypot\Exceptions\HoneypotException

<table style="text-align:left">
<tr><th>Class</th><td>HoneypotException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Honeypot\Exceptions\HoneypotException</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ConfigException.md">CodeIgniter\Exceptions\ConfigException</a></td></tr>
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
<th><a href="#forNoTemplate"><strong>forNoTemplate</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forNoNameField"><strong>forNoNameField</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forNoHiddenValue"><strong>forNoHiddenValue</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#isBot"><strong>isBot</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forNoTemplate()

```php
public static function forNoTemplate()
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
public static function forNoTemplate()
{
	return new static(lang('Honeypot.noTemplate'));
}
```

</details>


<hr>

#### forNoNameField()

```php
public static function forNoNameField()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (13 - 16)</small></summary>

```php
public static function forNoNameField()
{
	return new static(lang('Honeypot.noNameField'));
}
```

</details>


<hr>

#### forNoHiddenValue()

```php
public static function forNoHiddenValue()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (18 - 21)</small></summary>

```php
public static function forNoHiddenValue()
{
	return new static(lang('Honeypot.noHiddenValue'));
}
```

</details>


<hr>

#### isBot()

```php
public static function isBot()
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
public static function isBot()
{
	return new static(lang('Honeypot.theClientIsABot'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Honeypot/Exceptions/HoneypotException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/UserAgent.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Honeypot.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>