


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockCache.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCURLRequest.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCodeIgniter.md">next</a></td>
</tr>
</table>







# CodeIgniter\Test\Mock 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Test\Mock</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockAppConfig.md">CodeIgniter\Test\Mock\MockAppConfig</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockAutoload.md">CodeIgniter\Test\Mock\MockAutoload</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockBuilder.md">CodeIgniter\Test\Mock\MockBuilder</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCLIConfig.md">CodeIgniter\Test\Mock\MockCLIConfig</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCURLRequest.md">CodeIgniter\Test\Mock\MockCURLRequest</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCache.md">CodeIgniter\Test\Mock\MockCache</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCodeIgniter.md">CodeIgniter\Test\Mock\MockCodeIgniter</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockConnection.md">CodeIgniter\Test\Mock\MockConnection</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockEmail.md">CodeIgniter\Test\Mock\MockEmail</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockEvents.md">CodeIgniter\Test\Mock\MockEvents</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockFileLogger.md">CodeIgniter\Test\Mock\MockFileLogger</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockIncomingRequest.md">CodeIgniter\Test\Mock\MockIncomingRequest</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockLanguage.md">CodeIgniter\Test\Mock\MockLanguage</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockLogger.md">CodeIgniter\Test\Mock\MockLogger</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockQuery.md">CodeIgniter\Test\Mock\MockQuery</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockResourceController.md">CodeIgniter\Test\Mock\MockResourceController</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockResourcePresenter.md">CodeIgniter\Test\Mock\MockResourcePresenter</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockResponse.md">CodeIgniter\Test\Mock\MockResponse</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockResult.md">CodeIgniter\Test\Mock\MockResult</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockSecurity.md">CodeIgniter\Test\Mock\MockSecurity</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockServices.md">CodeIgniter\Test\Mock\MockServices</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockSession.md">CodeIgniter\Test\Mock\MockSession</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockTable.md">CodeIgniter\Test\Mock\MockTable</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md"><strong>CodeIgniter\Cache\CacheInterface</strong></a>
</td>
<td>CacheInterface</td>
</tr>
</table>



 
## CodeIgniter\Test\Mock\MockCache

<table style="text-align:left">
<tr><th>Class</th><td>MockCache</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Test\Mock\MockCache</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md">CodeIgniter\Cache\CacheInterface</a><br>
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
<th><a href="#prefix"><strong>prefix</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Prefixed to all cache names.</td>
</tr>
<tr>
<th><a href="#cache"><strong>cache</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Mock cache storage.</td>
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





### Properties


<hr>

#### $prefix

```php
protected $prefix;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prefixed to all cache names.
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


<hr>

#### $cache

```php
protected $cache = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Mock cache storage.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
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
<summary><small>Source: 4 lines (26 - 29)</small></summary>

```php
public function initialize()
{
	// Not to see here...
}
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
<summary><small>Source: 8 lines (40 - 47)</small></summary>

```php
public function get(string $key)
{
	$key = $this->prefix . $key;

	return array_key_exists($key, $this->cache)
		? $this->cache[$key]
		: null;
}
```

</details>


<hr>

#### save()

```php
public function save(string $key, $value, int $ttl = 60, bool $raw = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Saves an item to the cache store.
</td></tr>
</table>

<table>
<tr><td>
The $raw parameter is only utilized by Mamcache in order to
allow usage of increment() and decrement().
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
<td><em>
</em></td>
<td>false</td>
<td> data to save</td>
</tr>

<tr>
<td>3.</td>
<td><code>$ttl</code></td>
<td><em>null
</em></td>
<td>false</td>
<td>Time To Live, in seconds (default 60)</td>
</tr>

<tr>
<td>4.</td>
<td><code>$raw</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to store the raw value.</td>
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
<summary><small>Source: 8 lines (64 - 71)</small></summary>

```php
public function save(string $key, $value, int $ttl = 60, bool $raw = false)
{
	$key = $this->prefix . $key;

	$this->cache[$key] = $value;

	return true;
}
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
<summary><small>Source: 4 lines (82 - 85)</small></summary>

```php
public function delete(string $key)
{
	unset($this->cache[$key]);
}
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
<summary><small>Source: 17 lines (97 - 113)</small></summary>

```php
public function increment(string $key, int $offset = 1)
{
	$key = $this->prefix . $key;

	$data = $this->cache[$key] ?: null;

	if (empty($data))
	{
		$data = 0;
	}
	elseif (! is_int($data))
	{
		return false;
	}

	return $this->save($key, $data + $offset);
}
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
<summary><small>Source: 17 lines (125 - 141)</small></summary>

```php
public function decrement(string $key, int $offset = 1)
{
	$key = $this->prefix . $key;

	$data = $this->cache[$key] ?: null;

	if (empty($data))
	{
		$data = 0;
	}
	elseif (! is_int($data))
	{
		return false;
	}

	return $this->save($key, $data - $offset);
}
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
<summary><small>Source: 4 lines (150 - 153)</small></summary>

```php
public function clean()
{
	$this->cache = [];
}
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
<summary><small>Source: 4 lines (165 - 168)</small></summary>

```php
public function getCacheInfo()
{
	return [];
}
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
<summary><small>Source: 4 lines (179 - 182)</small></summary>

```php
public function getMetaData(string $key)
{
	return false;
}
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
<summary><small>Source: 4 lines (191 - 194)</small></summary>

```php
public function isSupported(): bool
{
	return true;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockCache.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCURLRequest.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCodeIgniter.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>