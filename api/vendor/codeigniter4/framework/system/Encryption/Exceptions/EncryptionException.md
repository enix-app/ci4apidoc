


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Encryption/Exceptions/EncryptionException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Encryption.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/BaseHandler.md">next</a></td>
</tr>
</table>







# CodeIgniter\Encryption\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Encryption\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Exceptions/EncryptionException.md">CodeIgniter\Encryption\Exceptions\EncryptionException</a></td></tr>
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



 
## CodeIgniter\Encryption\Exceptions\EncryptionException

<table style="text-align:left">
<tr><th>Class</th><td>EncryptionException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Encryption\Exceptions\EncryptionException</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Encryption\Exceptions\RuntimeException</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ExceptionInterface.md">CodeIgniter\Exceptions\ExceptionInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Encryption exception
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
<th><a href="#forNoDriverRequested"><strong>forNoDriverRequested</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forNoHandlerAvailable"><strong>forNoHandlerAvailable</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forUnKnownHandler"><strong>forUnKnownHandler</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forNeedsStarterKey"><strong>forNeedsStarterKey</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forAuthenticationFailed"><strong>forAuthenticationFailed</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forEncryptionFailed"><strong>forEncryptionFailed</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forNoDriverRequested()

```php
public static function forNoDriverRequested()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (12 - 15)</small></summary>

```php
public static function forNoDriverRequested()
{
	return new static(lang('Encryption.noDriverRequested'));
}
```

</details>


<hr>

#### forNoHandlerAvailable()

```php
public static function forNoHandlerAvailable()
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
public static function forNoHandlerAvailable()
{
	return new static(lang('Encryption.noHandlerAvailable'));
}
```

</details>


<hr>

#### forUnKnownHandler()

```php
public static function forUnKnownHandler(string $driver = null)
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
<td><code>$driver</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (22 - 25)</small></summary>

```php
public static function forUnKnownHandler(string $driver = null)
{
	return new static(lang('Encryption.unKnownHandler', [$driver]));
}
```

</details>


<hr>

#### forNeedsStarterKey()

```php
public static function forNeedsStarterKey()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (27 - 30)</small></summary>

```php
public static function forNeedsStarterKey()
{
	return new static(lang('Encryption.starterKeyNeeded'));
}
```

</details>


<hr>

#### forAuthenticationFailed()

```php
public static function forAuthenticationFailed()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (32 - 35)</small></summary>

```php
public static function forAuthenticationFailed()
{
	return new static(lang('Encryption.authenticationFailed'));
}
```

</details>


<hr>

#### forEncryptionFailed()

```php
public static function forEncryptionFailed()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (36 - 39)</small></summary>

```php
public static function forEncryptionFailed()
{
	return new static(lang('Encryption.encryptionFailed'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Encryption/Exceptions/EncryptionException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Encryption.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/BaseHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>