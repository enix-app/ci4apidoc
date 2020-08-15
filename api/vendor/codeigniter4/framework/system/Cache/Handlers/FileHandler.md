


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/Handlers/FileHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/DummyHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/MemcachedHandler.md">next</a></td>
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
<td>framework/system/Cache/Handlers/FileHandler.php
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/CacheException.md"><strong>CodeIgniter\Cache\Exceptions\CacheException</strong></a>
</td>
<td>CacheException</td>
</tr>
</table>



 
## CodeIgniter\Cache\Handlers\FileHandler

<table style="text-align:left">
<tr><th>Class</th><td>FileHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Cache\Handlers\FileHandler</td></tr>
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
File system cache handler
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
<th><a href="#path"><strong>path</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Where to store cached files on the disk.</td>
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
<tr>
<th><a href="#getItem"><strong>getItem</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Does the heavy lifting of actually retrieving the file and
verifying it&#039;s age.</td>
</tr>
<tr>
<th><a href="#writeFile"><strong>writeFile</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Writes a file to disk, or returns false if not successful.</td>
</tr>
<tr>
<th><a href="#deleteFiles"><strong>deleteFiles</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Delete Files</td>
</tr>
<tr>
<th><a href="#getDirFileInfo"><strong>getDirFileInfo</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get Directory File Information</td>
</tr>
<tr>
<th><a href="#getFileInfo"><strong>getFileInfo</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get File Info</td>
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

#### $path

```php
protected $path;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Where to store cached files on the disk.
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





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CacheException
</td>
</tr>
</table>



<details>
<summary><small>Source: 11 lines (73 - 83)</small></summary>

```php
public function __construct($config)
{
	$path = ! empty($config->storePath) ? $config->storePath : WRITEPATH . 'cache';
	if (! is_really_writable($path))
	{
		throw CacheException::forUnableToWrite($path);
	}

	$this->prefix = $config->prefix ?: '';
	$this->path   = rtrim($path, '/') . '/';
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
<summary><small>Source: 4 lines (90 - 93)</small></summary>

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
<summary><small>Source: 8 lines (104 - 111)</small></summary>

```php
public function get(string $key)
{
	$key = $this->prefix . $key;

	$data = $this->getItem($key);

	return is_array($data) ? $data['data'] : null;
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
<summary><small>Source: 19 lines (124 - 142)</small></summary>

```php
public function save(string $key, $value, int $ttl = 60)
{
	$key = $this->prefix . $key;

	$contents = [
		'time' => time(),
		'ttl'  => $ttl,
		'data' => $value,
	];

	if ($this->writeFile($this->path . $key, serialize($contents)))
	{
		chmod($this->path . $key, 0640);

		return true;
	}

	return false;
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
<summary><small>Source: 6 lines (153 - 158)</small></summary>

```php
public function delete(string $key)
{
	$key = $this->prefix . $key;

	return is_file($this->path . $key) && unlink($this->path . $key);
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
<summary><small>Source: 22 lines (170 - 191)</small></summary>

```php
public function increment(string $key, int $offset = 1)
{
	$key = $this->prefix . $key;

	$data = $this->getItem($key);

	if ($data === false)
	{
		$data = [
			'data' => 0,
			'ttl'  => 60,
		];
	}
	elseif (! is_int($data['data']))
	{
		return false;
	}

	$new_value = $data['data'] + $offset;

	return $this->save($key, $new_value, $data['ttl']) ? $new_value : false;
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
<summary><small>Source: 22 lines (203 - 224)</small></summary>

```php
public function decrement(string $key, int $offset = 1)
{
	$key = $this->prefix . $key;

	$data = $this->getItem($key);

	if ($data === false)
	{
		$data = [
			'data' => 0,
			'ttl'  => 60,
		];
	}
	elseif (! is_int($data['data']))
	{
		return false;
	}

	$new_value = $data['data'] - $offset;

	return $this->save($key, $new_value, $data['ttl']) ? $new_value : false;
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
<summary><small>Source: 4 lines (233 - 236)</small></summary>

```php
public function clean()
{
	return $this->deleteFiles($this->path, false, true);
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
<summary><small>Source: 4 lines (248 - 251)</small></summary>

```php
public function getCacheInfo()
{
	return $this->getDirFileInfo($this->path);
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
<summary><small>Source: 29 lines (262 - 290)</small></summary>

```php
public function getMetaData(string $key)
{
	$key = $this->prefix . $key;

	if (! is_file($this->path . $key))
	{
		return false;
	}

	$data = @unserialize(file_get_contents($this->path . $key));

	if (is_array($data))
	{
		$mtime = filemtime($this->path . $key);

		if (! isset($data['ttl']))
		{
			return false;
		}

		return [
			'expire' => $mtime + $data['ttl'],
			'mtime'  => $mtime,
			'data'   => $data['data'],
		];
	}

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
<summary><small>Source: 4 lines (299 - 302)</small></summary>

```php
public function isSupported(): bool
{
	return is_writable($this->path);
}
```

</details>


<hr>

#### getItem()

```php
protected function getItem(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does the heavy lifting of actually retrieving the file and
verifying it's age.
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
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool<br>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 22 lines (314 - 335)</small></summary>

```php
protected function getItem(string $key)
{
	if (! is_file($this->path . $key))
	{
		return false;
	}

	$data = unserialize(file_get_contents($this->path . $key));

	if ($data['ttl'] > 0 && time() > $data['time'] + $data['ttl'])
	{
		// If the file is still there then remove it
		if (is_file($this->path . $key))
		{
			unlink($this->path . $key);
		}

		return false;
	}

	return $data;
}
```

</details>


<hr>

#### writeFile()

```php
protected function writeFile($path, $data, $mode = 'wb')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Writes a file to disk, or returns false if not successful.
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

<tr>
<td>2.</td>
<td><code>$data</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$mode</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 22 lines (351 - 372)</small></summary>

```php
protected function writeFile($path, $data, $mode = 'wb')
{
	if (($fp = @fopen($path, $mode)) === false)
	{
		return false;
	}

	flock($fp, LOCK_EX);

	for ($result = $written = 0, $length = strlen($data); $written < $length; $written += $result)
	{
		if (($result = fwrite($fp, substr($data, $written))) === false)
		{
			break;
		}
	}

	flock($fp, LOCK_UN);
	fclose($fp);

	return is_int($result);
}
```

</details>


<hr>

#### deleteFiles()

```php
protected function deleteFiles(string $path, bool $del_dir = false, bool $htdocs = false, int $_level = 0) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Delete Files
</td></tr>
</table>

<table>
<tr><td>
Deletes all files contained in the supplied directory path.
Files must be writable or owned by the system in order to be deleted.
If the second parameter is set to TRUE, any directories contained
within the supplied base directory will be nuked as well.
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
<td>File path</td>
</tr>

<tr>
<td>2.</td>
<td><code>$del_dir</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to delete any directories found in the path</td>
</tr>

<tr>
<td>3.</td>
<td><code>$htdocs</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to skip deleting .htaccess and index page files</td>
</tr>

<tr>
<td>4.</td>
<td><code>$_level</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Current directory depth level (default: 0; internal use only)</td>
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
<summary><small>Source: 29 lines (391 - 419)</small></summary>

```php
protected function deleteFiles(string $path, bool $del_dir = false, bool $htdocs = false, int $_level = 0): bool
{
	// Trim the trailing slash
	$path = rtrim($path, '/\\');

	if (! $current_dir = @opendir($path))
	{
		return false;
	}

	while (false !== ($filename = @readdir($current_dir)))
	{
		if ($filename !== '.' && $filename !== '..')
		{
			if (is_dir($path . DIRECTORY_SEPARATOR . $filename) && $filename[0] !== '.')
			{
				$this->deleteFiles($path . DIRECTORY_SEPARATOR . $filename, $del_dir, $htdocs, $_level + 1);
			}
			elseif ($htdocs !== true || ! preg_match('/^(\.htaccess|index\.(html|htm|php)|web\.config)$/i', $filename))
			{
				@unlink($path . DIRECTORY_SEPARATOR . $filename);
			}
		}
	}

	closedir($current_dir);

	return ($del_dir === true && $_level > 0) ? @rmdir($path) : true;
}
```

</details>


<hr>

#### getDirFileInfo()

```php
protected function getDirFileInfo(string $source_dir, bool $top_level_only = true, bool $_recursion = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get Directory File Information
</td></tr>
</table>

<table>
<tr><td>
Reads the specified directory and builds an array containing the filenames,
filesize, dates, and permissions

Any sub-folders contained within the specified path are read as well.
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
<td><code>$source_dir</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Path to source</td>
</tr>

<tr>
<td>2.</td>
<td><code>$top_level_only</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Look only at the top level directory specified?</td>
</tr>

<tr>
<td>3.</td>
<td><code>$_recursion</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Internal variable to determine recursion status - do not use in calls</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 35 lines (437 - 471)</small></summary>

```php
protected function getDirFileInfo(string $source_dir, bool $top_level_only = true, bool $_recursion = false)
{
	static $_filedata = [];
	$relative_path    = $source_dir;

	if ($fp = @opendir($source_dir))
	{
		// reset the array and make sure $source_dir has a trailing slash on the initial call
		if ($_recursion === false)
		{
			$_filedata  = [];
			$source_dir = rtrim(realpath($source_dir), DIRECTORY_SEPARATOR) . DIRECTORY_SEPARATOR;
		}

		// Used to be foreach (scandir($source_dir, 1) as $file), but scandir() is simply not as fast
		while (false !== ($file = readdir($fp)))
		{
			if (is_dir($source_dir . $file) && $file[0] !== '.' && $top_level_only === false)
			{
				$this->getDirFileInfo($source_dir . $file . DIRECTORY_SEPARATOR, $top_level_only, true);
			}
			elseif ($file[0] !== '.')
			{
				$_filedata[$file]                  = $this->getFileInfo($source_dir . $file);
				$_filedata[$file]['relative_path'] = $relative_path;
			}
		}

		closedir($fp);

		return $_filedata;
	}

	return false;
}
```

</details>


<hr>

#### getFileInfo()

```php
protected function getFileInfo(string $file, $returned_values = array('name', 'server_path', 'size', 'date'))
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get File Info
</td></tr>
</table>

<table>
<tr><td>
Given a file and path, returns the name, path, size, date modified
Second parameter allows you to explicitly declare what information you want returned
Options are: name, server_path, size, date, readable, writable, executable, fileperms
Returns FALSE if the file cannot be found.
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
<td><code>$file</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Path to file</td>
</tr>

<tr>
<td>2.</td>
<td><code>$returned_values</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Array or comma separated string of information returned</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 45 lines (488 - 532)</small></summary>

```php
protected function getFileInfo(string $file, $returned_values = ['name', 'server_path', 'size', 'date'])
{
	if (! is_file($file))
	{
		return false;
	}

	if (is_string($returned_values))
	{
		$returned_values = explode(',', $returned_values);
	}

	foreach ($returned_values as $key)
	{
		switch ($key)
		{
			case 'name':
				$fileInfo['name'] = basename($file);
				break;
			case 'server_path':
				$fileInfo['server_path'] = $file;
				break;
			case 'size':
				$fileInfo['size'] = filesize($file);
				break;
			case 'date':
				$fileInfo['date'] = filemtime($file);
				break;
			case 'readable':
				$fileInfo['readable'] = is_readable($file);
				break;
			case 'writable':
				$fileInfo['writable'] = is_writable($file);
				break;
			case 'executable':
				$fileInfo['executable'] = is_executable($file);
				break;
			case 'fileperms':
				$fileInfo['fileperms'] = fileperms($file);
				break;
		}
	}

	return $fileInfo;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/Handlers/FileHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/DummyHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/MemcachedHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:09**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>