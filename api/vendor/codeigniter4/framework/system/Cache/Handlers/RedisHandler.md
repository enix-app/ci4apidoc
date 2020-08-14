


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/Handlers/RedisHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/PredisHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/WincacheHandler.md">next</a></td>
</tr>
</table>







# CodeIgniter\Cache\Handlers 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Cache\Handlers</td></tr>
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
<td>framework/system/Cache/Handlers/RedisHandler.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/DummyHandler.md">CodeIgniter\Cache\Handlers\DummyHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/FileHandler.md">CodeIgniter\Cache\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/MemcachedHandler.md">CodeIgniter\Cache\Handlers\MemcachedHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/PredisHandler.md">CodeIgniter\Cache\Handlers\PredisHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/RedisHandler.md">CodeIgniter\Cache\Handlers\RedisHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/WincacheHandler.md">CodeIgniter\Cache\Handlers\WincacheHandler</a></td></tr>
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
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md"><strong>CodeIgniter\Exceptions\CriticalError</strong></a>
</td>
<td>CriticalError</td>
</tr>
</table>



 
## CodeIgniter\Cache\Handlers\RedisHandler

<table style="text-align:left">
<tr><th>Class</th><td>RedisHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Cache\Handlers\RedisHandler</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md">CodeIgniter\Cache\CacheInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Redis cache handler
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
<th><a href="#prefix"><strong>prefix</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Prefixed to all cache names.</td>
</tr>
<tr>
<th><a href="#config"><strong>config</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Default config</td>
</tr>
<tr>
<th><a href="#redis"><strong>redis</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Redis connection</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor.</td>
</tr>
<tr>
<th><a href="#__destruct"><strong>__destruct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Class destructor</td>
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

#### $config

```php
protected $config = [
	'host'     => '127.0.0.1',
	'password' => null,
	'port'     => 6379,
	'timeout'  => 0,
	'database' => 0,
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Default config
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


<hr>

#### $redis

```php
protected $redis;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Redis connection
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Redis
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct($config)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor.
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
<td><code>$config</code></td>
<td><em>\Config\Cache
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (85 - 93)</small></summary>

```php
public function __construct($config)
{
	$this->prefix = $config->prefix ?: '';

	if (! empty($config))
	{
		$this->config = array_merge($this->config, $config->redis);
	}
}
```

</details>


<hr>

#### __destruct()

```php
public function __destruct()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class destructor
</td></tr>
</table>

<table>
<tr><td>
Closes the connection to Redis if present.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 7 lines (100 - 106)</small></summary>

```php
public function __destruct()
{
	if ($this->redis)
	{
		$this->redis->close();
	}
}
```

</details>


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
<summary><small>Source: 39 lines (113 - 151)</small></summary>

```php
public function initialize()
{
	$config = $this->config;

	$this->redis = new \Redis();

	// Try to connect to Redis, if an issue occurs throw a CriticalError exception,
	// so that the CacheFactory can attempt to initiate the next cache handler.
	try
	{
		// Note:: If Redis is your primary cache choice, and it is "offline", every page load will end up been delayed by the timeout duration.
		// I feel like some sort of temporary flag should be set, to indicate that we think Redis is "offline", allowing us to bypass the timeout for a set period of time.

		if (! $this->redis->connect($config['host'], ($config['host'][0] === '/' ? 0 : $config['port']), $config['timeout']))
		{
			// Note:: I'm unsure if log_message() is necessary, however I'm not 100% comfortable removing it.
			log_message('error', 'Cache: Redis connection failed. Check your configuration.');
			throw new CriticalError('Cache: Redis connection failed. Check your configuration.');
		}

		if (isset($config['password']) && ! $this->redis->auth($config['password']))
		{
			log_message('error', 'Cache: Redis authentication failed.');
			throw new CriticalError('Cache: Redis authentication failed.');
		}

		if (isset($config['database']) && ! $this->redis->select($config['database']))
		{
			log_message('error', 'Cache: Redis select database failed.');
			throw new CriticalError('Cache: Redis select database failed.');
		}
	}
	catch (\RedisException $e)
	{
		// $this->redis->connect() can sometimes throw a RedisException.
		// We need to convert the exception into a CriticalError exception and throw it.
		throw new CriticalError('Cache: RedisException occurred with message (' . $e->getMessage() . ').');
	}
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
<summary><small>Source: 27 lines (162 - 188)</small></summary>

```php
public function get(string $key)
{
	$key = $this->prefix . $key;

	$data = $this->redis->hMGet($key, ['__ci_type', '__ci_value']);

	if (! isset($data['__ci_type'], $data['__ci_value']) || $data['__ci_value'] === false)
	{
		return null;
	}

	switch ($data['__ci_type'])
	{
		case 'array':
		case 'object':
			return unserialize($data['__ci_value']);
		case 'boolean':
		case 'integer':
		case 'double': // Yes, 'double' is returned and NOT 'float'
		case 'string':
		case 'NULL':
			return settype($data['__ci_value'], $data['__ci_type']) ? $data['__ci_value'] : null;
		case 'resource':
		default:
			return null;
	}
}
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
<summary><small>Source: 32 lines (201 - 232)</small></summary>

```php
public function save(string $key, $value, int $ttl = 60)
{
	$key = $this->prefix . $key;

	switch ($data_type = gettype($value))
	{
		case 'array':
		case 'object':
			$value = serialize($value);
			break;
		case 'boolean':
		case 'integer':
		case 'double': // Yes, 'double' is returned and NOT 'float'
		case 'string':
		case 'NULL':
			break;
		case 'resource':
		default:
			return false;
	}

	if (! $this->redis->hMSet($key, ['__ci_type' => $data_type, '__ci_value' => $value]))
	{
		return false;
	}
	elseif ($ttl)
	{
		$this->redis->expireAt($key, time() + $ttl);
	}

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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (243 - 248)</small></summary>

```php
public function delete(string $key)
{
	$key = $this->prefix . $key;

	return ($this->redis->del($key) === 1);
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
<summary><small>Source: 6 lines (260 - 265)</small></summary>

```php
public function increment(string $key, int $offset = 1)
{
	$key = $this->prefix . $key;

	return $this->redis->hIncrBy($key, 'data', $offset);
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
<summary><small>Source: 6 lines (277 - 282)</small></summary>

```php
public function decrement(string $key, int $offset = 1)
{
	$key = $this->prefix . $key;

	return $this->redis->hIncrBy($key, 'data', -$offset);
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (291 - 294)</small></summary>

```php
public function clean()
{
	return $this->redis->flushDB();
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
<summary><small>Source: 4 lines (306 - 309)</small></summary>

```php
public function getCacheInfo()
{
	return $this->redis->info();
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
<summary><small>Source: 18 lines (320 - 337)</small></summary>

```php
public function getMetaData(string $key)
{
	$key = $this->prefix . $key;

	$value = $this->get($key);

	if ($value !== null)
	{
		$time = time();
		return [
			'expire' => $time + $this->redis->ttl($key),
			'mtime'  => $time,
			'data'   => $value,
		];
	}

	return null;
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
<summary><small>Source: 4 lines (346 - 349)</small></summary>

```php
public function isSupported(): bool
{
	return extension_loaded('redis');
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/Handlers/RedisHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/PredisHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/WincacheHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>