


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Throttle/ThrottlerInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/Throttler.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Typography/Typography.md">next</a></td>
</tr>
</table>







# CodeIgniter\Throttle 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Throttle</td></tr>
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
<td>framework/system/Throttle/ThrottlerInterface.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/Throttler.md">CodeIgniter\Throttle\Throttler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/ThrottlerInterface.md">CodeIgniter\Throttle\ThrottlerInterface</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Throttle\ThrottlerInterface

<table style="text-align:left">
<tr><th>Interface</th><td>ThrottlerInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Throttle\ThrottlerInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Expected behavior of a Throttler
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
<th><a href="#check"><strong>check</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Restricts the number of requests made by a single key within
a set number of seconds.</td>
</tr>
<tr>
<th><a href="#getTokenTime"><strong>getTokenTime</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of seconds until the next available token will
be released for usage.</td>
</tr>

</table>






### Methods


<hr>

#### check()

```php
public function check(string $key, int $capacity, int $seconds, int $cost)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Restricts the number of requests made by a single key within
a set number of seconds.
</td></tr>
</table>

<table>
<tr><td>
Example:

 if (! $throttler->checkIPAddress($request->ipAddress(), 60, MINUTE))
{
     die('You submitted over 60 requests within a minute.');
}
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
<td><code>$key</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The name to use as the "bucket" name.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$capacity</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The number of requests the "bucket" can hold</td>
</tr>

<tr>
<td>3.</td>
<td><code>$seconds</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The time it takes the "bucket" to completely refill</td>
</tr>

<tr>
<td>4.</td>
<td><code>$cost</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The number of tokens this action uses.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: line 65</small></summary>

```php
public function check(string $key, int $capacity, int $seconds, int $cost);
```

</details>


<hr>

#### getTokenTime()

```php
public function getTokenTime() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of seconds until the next available token will
be released for usage.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: line 75</small></summary>

```php
public function getTokenTime(): int;
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Throttle/ThrottlerInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/Throttler.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Typography/Typography.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>