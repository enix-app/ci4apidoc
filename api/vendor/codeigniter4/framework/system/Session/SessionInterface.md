


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Session/SessionInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Session.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Test/CIDatabaseTestCase.md">next</a></td>
</tr>
</table>







# CodeIgniter\Session 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Session</td></tr>
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
<td>framework/system/Session/SessionInterface.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Exceptions/SessionException.md">CodeIgniter\Session\Exceptions\SessionException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/ArrayHandler.md">CodeIgniter\Session\Handlers\ArrayHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">CodeIgniter\Session\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/DatabaseHandler.md">CodeIgniter\Session\Handlers\DatabaseHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/FileHandler.md">CodeIgniter\Session\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/MemcachedHandler.md">CodeIgniter\Session\Handlers\MemcachedHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/RedisHandler.md">CodeIgniter\Session\Handlers\RedisHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Session.md">CodeIgniter\Session\Session</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/SessionInterface.md">CodeIgniter\Session\SessionInterface</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Session\SessionInterface

<table style="text-align:left">
<tr><th>Interface</th><td>SessionInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Session\SessionInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Expected behavior of a session container used with CodeIgniter.
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
<th><a href="#regenerate"><strong>regenerate</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Regenerates the session ID.</td>
</tr>
<tr>
<th><a href="#destroy"><strong>destroy</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Destroys the current session.</td>
</tr>
<tr>
<th><a href="#set"><strong>set</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets user data into the session.</td>
</tr>
<tr>
<th><a href="#get"><strong>get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get user data that has been set in the session.</td>
</tr>
<tr>
<th><a href="#has"><strong>has</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns whether an index exists in the session array.</td>
</tr>
<tr>
<th><a href="#remove"><strong>remove</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Remove one or more session properties.</td>
</tr>
<tr>
<th><a href="#setFlashdata"><strong>setFlashdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets data into the session that will only last for a single request.</td>
</tr>
<tr>
<th><a href="#getFlashdata"><strong>getFlashdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve one or more items of flash data from the session.</td>
</tr>
<tr>
<th><a href="#keepFlashdata"><strong>keepFlashdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Keeps a single piece of flash data alive for one more request.</td>
</tr>
<tr>
<th><a href="#markAsFlashdata"><strong>markAsFlashdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Mark a session property or properties as flashdata.</td>
</tr>
<tr>
<th><a href="#unmarkFlashdata"><strong>unmarkFlashdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Unmark data in the session as flashdata.</td>
</tr>
<tr>
<th><a href="#getFlashKeys"><strong>getFlashKeys</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve all of the keys for session data marked as flashdata.</td>
</tr>
<tr>
<th><a href="#setTempdata"><strong>setTempdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets new data into the session, and marks it as temporary data
with a set lifespan.</td>
</tr>
<tr>
<th><a href="#getTempdata"><strong>getTempdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns either a single piece of tempdata, or all temp data currently
in the session.</td>
</tr>
<tr>
<th><a href="#removeTempdata"><strong>removeTempdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Removes a single piece of temporary data from the session.</td>
</tr>
<tr>
<th><a href="#markAsTempdata"><strong>markAsTempdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Mark one of more pieces of data as being temporary, meaning that
it has a set lifespan within the session.</td>
</tr>
<tr>
<th><a href="#unmarkTempdata"><strong>unmarkTempdata</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Unmarks temporary data in the session, effectively removing its
lifespan and allowing it to live as long as the session does.</td>
</tr>
<tr>
<th><a href="#getTempKeys"><strong>getTempKeys</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve the keys of all session data that have been marked as temporary data.</td>
</tr>

</table>






### Methods


<hr>

#### regenerate()

```php
public function regenerate(bool $destroy = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Regenerates the session ID.
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
<td><code>$destroy</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Should old session data be destroyed?</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 53</small></summary>

```php
public function regenerate(bool $destroy = false);
```

</details>


<hr>

#### destroy()

```php
public function destroy()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Destroys the current session.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: line 60</small></summary>

```php
public function destroy();
```

</details>


<hr>

#### set()

```php
public function set($data, $value = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets user data into the session.
</td></tr>
</table>

<table>
<tr><td>
If $data is a string, then it is interpreted as a session property
key, and  $value is expected to be non-null.

If $data is an array, it is expected to be an array of key/value pairs
to be set as session properties.
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
<td><code>$data</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Property name or associative array of properties</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Property value if single key provided</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 76</small></summary>

```php
public function set($data, $value = null);
```

</details>


<hr>

#### get()

```php
public function get(string $key = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get user data that has been set in the session.
</td></tr>
</table>

<table>
<tr><td>
If the property exists as "normal", returns it.
Otherwise, returns an array of any temp or flash data values with the
property key.

Replaces the legacy method $session->userdata();
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
<td>Identifier of the session property to retrieve</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: line 93</small></summary>

```php
public function get(string $key = null);
```

</details>


<hr>

#### has()

```php
public function has(string $key) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns whether an index exists in the session array.
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
<td>Identifier of the session property we are interested in.</td>
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
<summary><small>Source: line 104</small></summary>

```php
public function has(string $key): bool;
```

</details>


<hr>

#### remove()

```php
public function remove($key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Remove one or more session properties.
</td></tr>
</table>

<table>
<tr><td>
If $key is an array, it is interpreted as an array of string property
identifiers to remove. Otherwise, it is interpreted as the identifier
of a specific session property to remove.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Identifier of the session property or properties to remove.</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 117</small></summary>

```php
public function remove($key);
```

</details>


<hr>

#### setFlashdata()

```php
public function setFlashdata($data, $value = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets data into the session that will only last for a single request.
</td></tr>
</table>

<table>
<tr><td>
Perfect for use with single-use status update messages.

If $data is an array, it is interpreted as an associative array of
key/value pairs for flashdata properties.
Otherwise, it is interpreted as the identifier of a specific
flashdata property, with $value containing the property value.
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
<td><code>$data</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Property identifier or associative array of properties</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Property value if $data is a scalar</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 133</small></summary>

```php
public function setFlashdata($data, $value = null);
```

</details>


<hr>

#### getFlashdata()

```php
public function getFlashdata(string $key = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve one or more items of flash data from the session.
</td></tr>
</table>

<table>
<tr><td>
If the item key is null, return all flashdata.
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
<td>Property identifier</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: line 146</small></summary>

```php
public function getFlashdata(string $key = null);
```

</details>


<hr>

#### keepFlashdata()

```php
public function keepFlashdata($key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Keeps a single piece of flash data alive for one more request.
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
<td><em>array<br>string
</em></td>
<td>false</td>
<td>Property identifier or array of them</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 155</small></summary>

```php
public function keepFlashdata($key);
```

</details>


<hr>

#### markAsFlashdata()

```php
public function markAsFlashdata($key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Mark a session property or properties as flashdata.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Property identifier or array of them</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>false
</td>
</tr>
</table>





<details>
<summary><small>Source: line 166</small></summary>

```php
public function markAsFlashdata($key);
```

</details>


<hr>

#### unmarkFlashdata()

```php
public function unmarkFlashdata($key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Unmark data in the session as flashdata.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Property identifier or array of them</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 175</small></summary>

```php
public function unmarkFlashdata($key);
```

</details>


<hr>

#### getFlashKeys()

```php
public function getFlashKeys() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve all of the keys for session data marked as flashdata.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: line 184</small></summary>

```php
public function getFlashKeys(): array;
```

</details>


<hr>

#### setTempdata()

```php
public function setTempdata($data, $value = null, int $ttl = 300)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets new data into the session, and marks it as temporary data
with a set lifespan.
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
<td><code>$data</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Session data key or associative array of items</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Value to store</td>
</tr>

<tr>
<td>3.</td>
<td><code>$ttl</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Time-to-live in seconds</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 196</small></summary>

```php
public function setTempdata($data, $value = null, int $ttl = 300);
```

</details>


<hr>

#### getTempdata()

```php
public function getTempdata(string $key = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns either a single piece of tempdata, or all temp data currently
in the session.
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
<td>Session data key</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: line 207</small></summary>

```php
public function getTempdata(string $key = null);
```

</details>


<hr>

#### removeTempdata()

```php
public function removeTempdata(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes a single piece of temporary data from the session.
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
<td>Session data key</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 216</small></summary>

```php
public function removeTempdata(string $key);
```

</details>


<hr>

#### markAsTempdata()

```php
public function markAsTempdata($key, int $ttl = 300)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Mark one of more pieces of data as being temporary, meaning that
it has a set lifespan within the session.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Property identifier or array of them</td>
</tr>

<tr>
<td>2.</td>
<td><code>$ttl</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Time to live, in seconds</td>
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
<summary><small>Source: line 229</small></summary>

```php
public function markAsTempdata($key, int $ttl = 300);
```

</details>


<hr>

#### unmarkTempdata()

```php
public function unmarkTempdata($key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Unmarks temporary data in the session, effectively removing its
lifespan and allowing it to live as long as the session does.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Property identifier or array of them</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 239</small></summary>

```php
public function unmarkTempdata($key);
```

</details>


<hr>

#### getTempKeys()

```php
public function getTempKeys() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve the keys of all session data that have been marked as temporary data.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: line 248</small></summary>

```php
public function getTempKeys(): array;
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Session/SessionInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Session.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Test/CIDatabaseTestCase.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>