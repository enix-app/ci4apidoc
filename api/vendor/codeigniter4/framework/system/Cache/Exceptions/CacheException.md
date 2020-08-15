


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/Exceptions/CacheException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/ExceptionInterface.md">next</a></td>
</tr>
</table>







# CodeIgniter\Cache\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Cache\Exceptions</td></tr>
</table>

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CodeIgniter
</td></tr>
</table>

<table>
<tr><td>
An open source application development framework for PHP

This content is released under the MIT License (MIT)

Copyright (c) 2014-2019 British Columbia Institute of Technology
Copyright (c) 2019-2020 CodeIgniter Foundation

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter
</td>
</tr>
<tr style="vertical-align:top;">
<th>author</th>
<td>CodeIgniter Dev Team
</td>
</tr>
<tr style="vertical-align:top;">
<th>copyright</th>
<td>2019-2020 CodeIgniter Foundation
</td>
</tr>
<tr style="vertical-align:top;">
<th>license</th>
<td><a href="https://opensource.org/licenses/MIT">https://opensource.org/licenses/MIT</a>	MIT License
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com">https://codeigniter.com</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>filesource</th>
<td>framework/system/Cache/Exceptions/CacheException.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/CacheException.md">CodeIgniter\Cache\Exceptions\CacheException</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/ExceptionInterface.md">CodeIgniter\Cache\Exceptions\ExceptionInterface</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Cache\Exceptions\CacheException

<table style="text-align:left">
<tr><th>Class</th><td>CacheException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Cache\Exceptions\CacheException</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Cache\Exceptions\RuntimeException</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/ExceptionInterface.md">CodeIgniter\Cache\Exceptions\ExceptionInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CacheException
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
<th><a href="#forUnableToWrite"><strong>forUnableToWrite</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when handler has no permission to write cache.</td>
</tr>
<tr>
<th><a href="#forInvalidHandlers"><strong>forInvalidHandlers</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when an unrecognized handler is used.</td>
</tr>
<tr>
<th><a href="#forNoBackup"><strong>forNoBackup</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when no backup handler is setup in config.</td>
</tr>
<tr>
<th><a href="#forHandlerNotFound"><strong>forHandlerNotFound</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when specified handler was not found.</td>
</tr>

</table>






### Methods


<hr>

#### forUnableToWrite()

```php
public static function forUnableToWrite(string $path)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when handler has no permission to write cache.
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
<td><code>$path</code></td>
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
<td>\CodeIgniter\Cache\Exceptions\CacheException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (53 - 56)</small></summary>

```php
public static function forUnableToWrite(string $path)
{
	return new static(lang('Cache.unableToWrite', [$path]));
}
```

</details>


<hr>

#### forInvalidHandlers()

```php
public static function forInvalidHandlers()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when an unrecognized handler is used.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Cache\Exceptions\CacheException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (63 - 66)</small></summary>

```php
public static function forInvalidHandlers()
{
	return new static(lang('Cache.invalidHandlers'));
}
```

</details>


<hr>

#### forNoBackup()

```php
public static function forNoBackup()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when no backup handler is setup in config.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Cache\Exceptions\CacheException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (73 - 76)</small></summary>

```php
public static function forNoBackup()
{
	return new static(lang('Cache.noBackup'));
}
```

</details>


<hr>

#### forHandlerNotFound()

```php
public static function forHandlerNotFound()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when specified handler was not found.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Cache\Exceptions\CacheException
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (83 - 86)</small></summary>

```php
public static function forHandlerNotFound()
{
	return new static(lang('Cache.handlerNotFound'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/Exceptions/CacheException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/ExceptionInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:09**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>