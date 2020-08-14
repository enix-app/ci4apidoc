


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/CacheInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheFactory.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/CacheException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Cache 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Cache</td></tr>
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
<td>framework/system/Cache/CacheInterface.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheFactory.md">CodeIgniter\Cache\CacheFactory</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md">CodeIgniter\Cache\CacheInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/CacheException.md">CodeIgniter\Cache\Exceptions\CacheException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/ExceptionInterface.md">CodeIgniter\Cache\Exceptions\ExceptionInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/DummyHandler.md">CodeIgniter\Cache\Handlers\DummyHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/FileHandler.md">CodeIgniter\Cache\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/MemcachedHandler.md">CodeIgniter\Cache\Handlers\MemcachedHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/PredisHandler.md">CodeIgniter\Cache\Handlers\PredisHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/RedisHandler.md">CodeIgniter\Cache\Handlers\RedisHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/WincacheHandler.md">CodeIgniter\Cache\Handlers\WincacheHandler</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Cache\CacheInterface

<table style="text-align:left">
<tr><th>Interface</th><td>CacheInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Cache\CacheInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cache interface
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
<th><a href="#initialize"><strong>initialize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Takes care of any handler-specific setup that must be done.</td>
</tr>
<tr>
<th><a href="#get"><strong>get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attempts to fetch an item from the cache store.</td>
</tr>
<tr>
<th><a href="#save"><strong>save</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Saves an item to the cache store.</td>
</tr>
<tr>
<th><a href="#delete"><strong>delete</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Deletes a specific item from the cache store.</td>
</tr>
<tr>
<th><a href="#increment"><strong>increment</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Performs atomic incrementation of a raw stored value.</td>
</tr>
<tr>
<th><a href="#decrement"><strong>decrement</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Performs atomic decrementation of a raw stored value.</td>
</tr>
<tr>
<th><a href="#clean"><strong>clean</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Will delete all items in the entire cache.</td>
</tr>
<tr>
<th><a href="#getCacheInfo"><strong>getCacheInfo</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns information on the entire cache.</td>
</tr>
<tr>
<th><a href="#getMetaData"><strong>getMetaData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns detailed information about the specific item in the cache.</td>
</tr>
<tr>
<th><a href="#isSupported"><strong>isSupported</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines if the driver is supported on this system.</td>
</tr>

</table>






### Methods


<hr>

#### initialize()

```php
public function initialize()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes care of any handler-specific setup that must be done.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: line 51</small></summary>

```php
public function initialize();
```

</details>


<hr>

#### get()

```php
public function get(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to fetch an item from the cache store.
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
<td>Cache item name</td>
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
<summary><small>Source: line 62</small></summary>

```php
public function get(string $key);
```

</details>


<hr>

#### save()

```php
public function save(string $key, $value, int $ttl = 60)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Saves an item to the cache store.
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
<td>Cache item name</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>The data to save</td>
</tr>

<tr>
<td>3.</td>
<td><code>$ttl</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Time To Live, in seconds (default 60)</td>
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
<summary><small>Source: line 75</small></summary>

```php
public function save(string $key, $value, int $ttl = 60);
```

</details>


<hr>

#### delete()

```php
public function delete(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Deletes a specific item from the cache store.
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
<td>Cache item name</td>
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
<summary><small>Source: line 86</small></summary>

```php
public function delete(string $key);
```

</details>


<hr>

#### increment()

```php
public function increment(string $key, int $offset = 1)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Performs atomic incrementation of a raw stored value.
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
<td>Cache ID</td>
</tr>

<tr>
<td>2.</td>
<td><code>$offset</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Step/value to increase by</td>
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
<summary><small>Source: line 98</small></summary>

```php
public function increment(string $key, int $offset = 1);
```

</details>


<hr>

#### decrement()

```php
public function decrement(string $key, int $offset = 1)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Performs atomic decrementation of a raw stored value.
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
<td>Cache ID</td>
</tr>

<tr>
<td>2.</td>
<td><code>$offset</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Step/value to increase by</td>
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
<summary><small>Source: line 110</small></summary>

```php
public function decrement(string $key, int $offset = 1);
```

</details>


<hr>

#### clean()

```php
public function clean()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Will delete all items in the entire cache.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: line 119</small></summary>

```php
public function clean();
```

</details>


<hr>

#### getCacheInfo()

```php
public function getCacheInfo()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns information on the entire cache.
</td></tr>
</table>

<table>
<tr><td>
The information returned and the structure of the data
varies depending on the handler.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: line 131</small></summary>

```php
public function getCacheInfo();
```

</details>


<hr>

#### getMetaData()

```php
public function getMetaData(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns detailed information about the specific item in the cache.
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
<td>Cache item name.</td>
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
<summary><small>Source: line 142</small></summary>

```php
public function getMetaData(string $key);
```

</details>


<hr>

#### isSupported()

```php
public function isSupported() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines if the driver is supported on this system.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: line 151</small></summary>

```php
public function isSupported(): bool;
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/CacheInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheFactory.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/CacheException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:07**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>