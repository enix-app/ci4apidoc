


 



<table>
<tr>
<td style="width:100%"><em>framework/system/I18n/Exceptions/I18nException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Honeypot.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/I18n/Time.md">next</a></td>
</tr>
</table>







# CodeIgniter\I18n\Exceptions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\I18n\Exceptions</td></tr>
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
<td><a href="https://opensource.org/licenses/MIT">https://opensource.org/licenses/MIT</a>    MIT License
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com">https://codeigniter.com</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>filesource</th>
<td>framework/system/I18n/Exceptions/I18nException.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/I18n/Exceptions/I18nException.md">CodeIgniter\I18n\Exceptions\I18nException</a></td></tr>
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



 
## CodeIgniter\I18n\Exceptions\I18nException

<table style="text-align:left">
<tr><th>Class</th><td>I18nException</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\I18n\Exceptions\I18nException</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/FrameworkException.md">CodeIgniter\Exceptions\FrameworkException</a></td></tr>
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
I18nException
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
<th><a href="#forInvalidMonth"><strong>forInvalidMonth</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when the numeric representation of the month falls
outside the range of allowed months.</td>
</tr>
<tr>
<th><a href="#forInvalidDay"><strong>forInvalidDay</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when the supplied day falls outside the range
of allowed days.</td>
</tr>
<tr>
<th><a href="#forInvalidOverDay"><strong>forInvalidOverDay</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when the day provided falls outside the allowed
last day for the given month.</td>
</tr>
<tr>
<th><a href="#forInvalidHour"><strong>forInvalidHour</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when the supplied hour falls outside the
range of allowed hours.</td>
</tr>
<tr>
<th><a href="#forInvalidMinutes"><strong>forInvalidMinutes</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when the supplied minutes falls outside the
range of allowed minutes.</td>
</tr>
<tr>
<th><a href="#forInvalidSeconds"><strong>forInvalidSeconds</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Thrown when the supplied seconds falls outside the
range of allowed seconds.</td>
</tr>

</table>






### Methods


<hr>

#### forInvalidMonth()

```php
public static function forInvalidMonth(string $month)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when the numeric representation of the month falls
outside the range of allowed months.
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
<td><code>$month</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (58 - 61)</small></summary>

```php
public static function forInvalidMonth(string $month)
{
	return new static(lang('Time.invalidMonth', [$month]));
}
```

</details>


<hr>

#### forInvalidDay()

```php
public static function forInvalidDay(string $day)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when the supplied day falls outside the range
of allowed days.
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
<td><code>$day</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (71 - 74)</small></summary>

```php
public static function forInvalidDay(string $day)
{
	return new static(lang('Time.invalidDay', [$day]));
}
```

</details>


<hr>

#### forInvalidOverDay()

```php
public static function forInvalidOverDay(string $lastDay, string $day)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when the day provided falls outside the allowed
last day for the given month.
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
<td><code>$lastDay</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$day</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (85 - 88)</small></summary>

```php
public static function forInvalidOverDay(string $lastDay, string $day)
{
	return new static(lang('Time.invalidOverDay', [$lastDay, $day]));
}
```

</details>


<hr>

#### forInvalidHour()

```php
public static function forInvalidHour(string $hour)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when the supplied hour falls outside the
range of allowed hours.
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
<td><code>$hour</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (98 - 101)</small></summary>

```php
public static function forInvalidHour(string $hour)
{
	return new static(lang('Time.invalidHour', [$hour]));
}
```

</details>


<hr>

#### forInvalidMinutes()

```php
public static function forInvalidMinutes(string $minutes)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when the supplied minutes falls outside the
range of allowed minutes.
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
<td><code>$minutes</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (111 - 114)</small></summary>

```php
public static function forInvalidMinutes(string $minutes)
{
	return new static(lang('Time.invalidMinutes', [$minutes]));
}
```

</details>


<hr>

#### forInvalidSeconds()

```php
public static function forInvalidSeconds(string $seconds)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Thrown when the supplied seconds falls outside the
range of allowed seconds.
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
<td><code>$seconds</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (124 - 127)</small></summary>

```php
public static function forInvalidSeconds(string $seconds)
{
	return new static(lang('Time.invalidSeconds', [$seconds]));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/I18n/Exceptions/I18nException.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Honeypot/Honeypot.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/I18n/Time.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>