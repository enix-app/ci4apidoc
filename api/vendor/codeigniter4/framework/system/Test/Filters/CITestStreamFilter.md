


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Filters/CITestStreamFilter.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/FeatureTestTrait.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Interfaces/FabricatorModel.md">next</a></td>
</tr>
</table>







# CodeIgniter\Test\Filters 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Test\Filters</td></tr>
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
<td>framework/system/Test/Filters/CITestStreamFilter.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Filters/CITestStreamFilter.md">CodeIgniter\Test\Filters\CITestStreamFilter</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Test\Filters\CITestStreamFilter

<table style="text-align:left">
<tr><th>Class</th><td>CITestStreamFilter</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Test\Filters\CITestStreamFilter</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Test\Filters\php_user_filter</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class to extract an output snapshot.
</td></tr>
</table>

<table>
<tr><td>
Used to capture output during unit testing, so that it can
be used in assertions.
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
<th><a href="#buffer"><strong>buffer</strong></a></th>
<td>prop</td>
<td>
public<br>static

</td>
<td>Buffer to capture stream content.</td>
</tr>

<tr>
<th><a href="#filter"><strong>filter</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Output filtering - catch it all.</td>
</tr>

</table>





### Properties


<hr>

#### $buffer

```php
public static $buffer = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Buffer to capture stream content.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>string
</td>
</tr>
</table>







### Methods


<hr>

#### filter()

```php
public function filter($in, $out, &$consumed, $closing)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Output filtering - catch it all.
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
<td><code>$in</code></td>
<td><em>resource
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$out</code></td>
<td><em>resource
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$consumed</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$closing</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (67 - 75)</small></summary>

```php
public function filter($in, $out, &$consumed, $closing)
{
	while ($bucket = stream_bucket_make_writeable($in))
	{
		static::$buffer .= $bucket->data;
		$consumed       += $bucket->datalen;
	}
	return PSFS_PASS_ON;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Filters/CITestStreamFilter.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/FeatureTestTrait.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Interfaces/FabricatorModel.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>