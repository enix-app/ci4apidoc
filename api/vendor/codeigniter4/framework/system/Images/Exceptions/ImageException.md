


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Exceptions/ImageException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/I18n/TimeDifference.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/BaseHandler.md">next</a></td>
</tr>
</table>







# CodeIgniter\Images\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Images\Exceptions</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Exceptions/ImageException.md">CodeIgniter\Images\Exceptions\ImageException</a></td></tr>
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



 
## CodeIgniter\Images\Exceptions\ImageException

<table style="text-align:left">
<tr><th>Class</th><td>ImageException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Images\Exceptions\ImageException</td></tr>
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
<th><a href="#forMissingImage"><strong>forMissingImage</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forFileNotSupported"><strong>forFileNotSupported</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forMissingAngle"><strong>forMissingAngle</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forInvalidDirection"><strong>forInvalidDirection</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forInvalidPath"><strong>forInvalidPath</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forEXIFUnsupported"><strong>forEXIFUnsupported</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forInvalidImageCreate"><strong>forInvalidImageCreate</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forSaveFailed"><strong>forSaveFailed</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forInvalidImageLibraryPath"><strong>forInvalidImageLibraryPath</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#forImageProcessFailed"><strong>forImageProcessFailed</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td></td>
</tr>

</table>






### Methods


<hr>

#### forMissingImage()

```php
public static function forMissingImage()
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
public static function forMissingImage()
{
	return new static(lang('Images.sourceImageRequired'));
}
```

</details>


<hr>

#### forFileNotSupported()

```php
public static function forFileNotSupported()
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
public static function forFileNotSupported()
{
	return new static(lang('Images.fileNotSupported'));
}
```

</details>


<hr>

#### forMissingAngle()

```php
public static function forMissingAngle()
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
public static function forMissingAngle()
{
	return new static(lang('Images.rotationAngleRequired'));
}
```

</details>


<hr>

#### forInvalidDirection()

```php
public static function forInvalidDirection(string $dir = null)
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
<td><code>$dir</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (23 - 26)</small></summary>

```php
public static function forInvalidDirection(string $dir = null)
{
	return new static(lang('Images.invalidDirection', [$dir]));
}
```

</details>


<hr>

#### forInvalidPath()

```php
public static function forInvalidPath()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (28 - 31)</small></summary>

```php
public static function forInvalidPath()
{
	return new static(lang('Images.invalidPath'));
}
```

</details>


<hr>

#### forEXIFUnsupported()

```php
public static function forEXIFUnsupported()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (33 - 36)</small></summary>

```php
public static function forEXIFUnsupported()
{
	return new static(lang('Images.exifNotSupported'));
}
```

</details>


<hr>

#### forInvalidImageCreate()

```php
public static function forInvalidImageCreate(string $extra = null)
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
<td><code>$extra</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (38 - 41)</small></summary>

```php
public static function forInvalidImageCreate(string $extra = null)
{
	return new static(lang('Images.unsupportedImageCreate') . ' ' . $extra);
}
```

</details>


<hr>

#### forSaveFailed()

```php
public static function forSaveFailed()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (43 - 46)</small></summary>

```php
public static function forSaveFailed()
{
	return new static(lang('Images.saveFailed'));
}
```

</details>


<hr>

#### forInvalidImageLibraryPath()

```php
public static function forInvalidImageLibraryPath(string $path = null)
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
<summary><small>Source: 4 lines (48 - 51)</small></summary>

```php
public static function forInvalidImageLibraryPath(string $path = null)
{
	return new static(lang('Images.libPathInvalid', [$path]));
}
```

</details>


<hr>

#### forImageProcessFailed()

```php
public static function forImageProcessFailed()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (53 - 56)</small></summary>

```php
public static function forImageProcessFailed()
{
	return new static(lang('Images.imageProcessFailed'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Exceptions/ImageException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/I18n/TimeDifference.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/BaseHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>