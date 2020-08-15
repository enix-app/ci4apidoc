


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/RedisHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/MemcachedHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Session.md">next</a></td>
</tr>
</table>







# CodeIgniter\Session\Handlers 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Session\Handlers</td></tr>
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
<td>framework/system/Session/Handlers/RedisHandler.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/ArrayHandler.md">CodeIgniter\Session\Handlers\ArrayHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">CodeIgniter\Session\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/DatabaseHandler.md">CodeIgniter\Session\Handlers\DatabaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/FileHandler.md">CodeIgniter\Session\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/MemcachedHandler.md">CodeIgniter\Session\Handlers\MemcachedHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/RedisHandler.md">CodeIgniter\Session\Handlers\RedisHandler</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md"><strong>CodeIgniter\Config\BaseConfig</strong></a>
</td>
<td>BaseConfig</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Exceptions/SessionException.md"><strong>CodeIgniter\Session\Exceptions\SessionException</strong></a>
</td>
<td>SessionException</td>
</tr>
</table>



 
## CodeIgniter\Session\Handlers\RedisHandler

<table style="text-align:left">
<tr><th>Class</th><td>RedisHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Session\Handlers\RedisHandler</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">CodeIgniter\Session\Handlers\BaseHandler</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="">CodeIgniter\Session\Handlers\SessionHandlerInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Session handler using Redis for persistence
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
<th><a href="#redis"><strong>redis</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>phpRedis instance</td>
</tr>
<tr>
<th><a href="#keyPrefix"><strong>keyPrefix</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Key prefix</td>
</tr>
<tr>
<th><a href="#lockKey"><strong>lockKey</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Lock key</td>
</tr>
<tr>
<th><a href="#keyExists"><strong>keyExists</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Key exists flag</td>
</tr>
<tr>
<th><a href="#sessionExpiration"><strong>sessionExpiration</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Number of seconds until the session ends.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor</td>
</tr>
<tr>
<th><a href="#open"><strong>open</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Open</td>
</tr>
<tr>
<th><a href="#read"><strong>read</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Read</td>
</tr>
<tr>
<th><a href="#write"><strong>write</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Write</td>
</tr>
<tr>
<th><a href="#close"><strong>close</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Close</td>
</tr>
<tr>
<th><a href="#destroy"><strong>destroy</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Destroy</td>
</tr>
<tr>
<th><a href="#gc"><strong>gc</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Garbage Collector</td>
</tr>
<tr>
<th><a href="#lockSession"><strong>lockSession</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get lock</td>
</tr>
<tr>
<th><a href="#releaseLock"><strong>releaseLock</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Release lock</td>
</tr>

</table>





### Properties


<hr>

#### $redis

```php
protected $redis;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
phpRedis instance
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>resource
</td>
</tr>
</table>


<hr>

#### $keyPrefix

```php
protected $keyPrefix = 'ci_session:';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Key prefix
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

#### $lockKey

```php
protected $lockKey;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Lock key
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

#### $keyExists

```php
protected $keyExists = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Key exists flag
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>bool
</td>
</tr>
</table>


<hr>

#### $sessionExpiration

```php
protected $sessionExpiration = 7200;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Number of seconds until the session ends.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(BaseConfig $config, string $ipAddress)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor
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
<td><em>\BaseConfig
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$ipAddress</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 36 lines (96 - 131)</small></summary>

```php
public function __construct(BaseConfig $config, string $ipAddress)
{
	parent::__construct($config, $ipAddress);

	if (empty($this->savePath))
	{
		throw SessionException::forEmptySavepath();
	}
	elseif (preg_match('#(?:tcp://)?([^:?]+)(?:\:(\d+))?(\?.+)?#', $this->savePath, $matches))
	{
		isset($matches[3]) || $matches[3] = ''; // Just to avoid undefined index notices below

		$this->savePath = [
			'host'     => $matches[1],
			'port'     => empty($matches[2]) ? null : $matches[2],
			'password' => preg_match('#auth=([^\s&]+)#', $matches[3], $match) ? $match[1] : null,
			'database' => preg_match('#database=(\d+)#', $matches[3], $match) ? (int) $match[1] : null,
			'timeout'  => preg_match('#timeout=(\d+\.\d+)#', $matches[3], $match) ? (float) $match[1] : null,
		];

		preg_match('#prefix=([^\s&]+)#', $matches[3], $match) && $this->keyPrefix = $match[1];
	}
	else
	{
		throw SessionException::forInvalidSavePathFormat($this->savePath);
	}

	if ($this->matchIP === true)
	{
		$this->keyPrefix .= $this->ipAddress . ':';
	}

	$this->sessionExpiration = empty($config->sessionExpiration)
		? (int) ini_get('session.gc_maxlifetime')
		: (int) $config->sessionExpiration;
}
```

</details>


<hr>

#### open()

```php
public function open($save_path, $name) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Open
</td></tr>
</table>

<table>
<tr><td>
Sanitizes save_path and initializes connection.
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
<td><code>$save_path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Server path</td>
</tr>

<tr>
<td>2.</td>
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Session cookie name, unused</td>
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
<summary><small>Source: 29 lines (144 - 172)</small></summary>

```php
public function open($save_path, $name): bool
{
	if (empty($this->savePath))
	{
		return false;
	}

	$redis = new \Redis();

	if (! $redis->connect($this->savePath['host'], $this->savePath['port'], $this->savePath['timeout']))
	{
		$this->logger->error('Session: Unable to connect to Redis with the configured settings.');
	}
	elseif (isset($this->savePath['password']) && ! $redis->auth($this->savePath['password']))
	{
		$this->logger->error('Session: Unable to authenticate to Redis instance.');
	}
	elseif (isset($this->savePath['database']) && ! $redis->select($this->savePath['database']))
	{
		$this->logger->error('Session: Unable to select Redis database with index ' . $this->savePath['database']);
	}
	else
	{
		$this->redis = $redis;
		return true;
	}

	return false;
}
```

</details>


<hr>

#### read()

```php
public function read($sessionID) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Read
</td></tr>
</table>

<table>
<tr><td>
Reads session data and acquires a lock
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
<td><code>$sessionID</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Session ID</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 20 lines (185 - 204)</small></summary>

```php
public function read($sessionID): string
{
	if (isset($this->redis) && $this->lockSession($sessionID))
	{
		// Needed by write() to detect session_regenerate_id() calls
		if (is_null($this->sessionID))
		{
			$this->sessionID = $sessionID;
		}

		$session_data                               = $this->redis->get($this->keyPrefix . $sessionID);
		is_string($session_data) ? $this->keyExists = true : $session_data = '';

		$this->fingerprint = md5($session_data);

		return $session_data;
	}

	return '';
}
```

</details>


<hr>

#### write()

```php
public function write($sessionID, $sessionData) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Write
</td></tr>
</table>

<table>
<tr><td>
Writes (create / update) session data
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
<td><code>$sessionID</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Session ID</td>
</tr>

<tr>
<td>2.</td>
<td><code>$sessionData</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Serialized session data</td>
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
<summary><small>Source: 39 lines (218 - 256)</small></summary>

```php
public function write($sessionID, $sessionData): bool
{
	if (! isset($this->redis))
	{
		return false;
	}
	// Was the ID regenerated?
	elseif ($sessionID !== $this->sessionID)
	{
		if (! $this->releaseLock() || ! $this->lockSession($sessionID))
		{
			return false;
		}

		$this->keyExists = false;
		$this->sessionID = $sessionID;
	}

	if (isset($this->lockKey))
	{
		$this->redis->expire($this->lockKey, 300);

		if ($this->fingerprint !== ($fingerprint = md5($sessionData)) || $this->keyExists === false)
		{
			if ($this->redis->set($this->keyPrefix . $sessionID, $sessionData, $this->sessionExpiration))
			{
				$this->fingerprint = $fingerprint;
				$this->keyExists   = true;
				return true;
			}

			return false;
		}

		return $this->redis->expire($this->keyPrefix . $sessionID, $this->sessionExpiration);
	}

	return false;
}
```

</details>


<hr>

#### close()

```php
public function close() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Close
</td></tr>
</table>

<table>
<tr><td>
Releases locks and closes connection.
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
<summary><small>Source: 29 lines (267 - 295)</small></summary>

```php
public function close(): bool
{
	if (isset($this->redis))
	{
		try
		{
			$ping_reply = $this->redis->ping();
			if (($ping_reply === true) || ($ping_reply === '+PONG'))
			{
				isset($this->lockKey) && $this->redis->del($this->lockKey);

				if (! $this->redis->close())
				{
					return false;
				}
			}
		}
		catch (\RedisException $e)
		{
			$this->logger->error('Session: Got RedisException on close(): ' . $e->getMessage());
		}

		$this->redis = null;

		return true;
	}

	return true;
}
```

</details>


<hr>

#### destroy()

```php
public function destroy($sessionID) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Destroy
</td></tr>
</table>

<table>
<tr><td>
Destroys the current session.
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
<td><code>$sessionID</code></td>
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
<summary><small>Source: 14 lines (308 - 321)</small></summary>

```php
public function destroy($sessionID): bool
{
	if (isset($this->redis, $this->lockKey))
	{
		if (($result = $this->redis->del($this->keyPrefix . $sessionID)) !== 1)
		{
			$this->logger->debug('Session: Redis::del() expected to return 1, got ' . var_export($result, true) . ' instead.');
		}

		return $this->destroyCookie();
	}

	return false;
}
```

</details>


<hr>

#### gc()

```php
public function gc($maxlifetime) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Garbage Collector
</td></tr>
</table>

<table>
<tr><td>
Deletes expired sessions
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
<td><code>$maxlifetime</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Maximum lifetime of sessions</td>
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
<summary><small>Source: 5 lines (333 - 337)</small></summary>

```php
public function gc($maxlifetime): bool
{
	// Not necessary, Redis takes care of that.
	return true;
}
```

</details>


<hr>

#### lockSession()

```php
protected function lockSession(string $sessionID) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get lock
</td></tr>
</table>

<table>
<tr><td>
Acquires an (emulated) lock.
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
<td><code>$sessionID</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Session ID</td>
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
<summary><small>Source: 46 lines (350 - 395)</small></summary>

```php
protected function lockSession(string $sessionID): bool
{
	// PHP 7 reuses the SessionHandler object on regeneration,
	// so we need to check here if the lock key is for the
	// correct session ID.
	if ($this->lockKey === $this->keyPrefix . $sessionID . ':lock')
	{
		return $this->redis->expire($this->lockKey, 300);
	}

	// 30 attempts to obtain a lock, in case another request already has it
	$lock_key = $this->keyPrefix . $sessionID . ':lock';
	$attempt  = 0;

	do
	{
		if (($ttl = $this->redis->ttl($lock_key)) > 0)
		{
			sleep(1);
			continue;
		}

		if (! $this->redis->setex($lock_key, 300, time()))
		{
			$this->logger->error('Session: Error while trying to obtain lock for ' . $this->keyPrefix . $sessionID);
			return false;
		}

		$this->lockKey = $lock_key;
		break;
	}
	while (++ $attempt < 30);

	if ($attempt === 30)
	{
		log_message('error', 'Session: Unable to obtain lock for ' . $this->keyPrefix . $sessionID . ' after 30 attempts, aborting.');
		return false;
	}
	elseif ($ttl === -1)
	{
		log_message('debug', 'Session: Lock for ' . $this->keyPrefix . $sessionID . ' had no TTL, overriding.');
	}

	$this->lock = true;
	return true;
}
```

</details>


<hr>

#### releaseLock()

```php
protected function releaseLock() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Release lock
</td></tr>
</table>

<table>
<tr><td>
Releases a previously acquired lock
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
<summary><small>Source: 16 lines (406 - 421)</small></summary>

```php
protected function releaseLock(): bool
{
	if (isset($this->redis, $this->lockKey) && $this->lock)
	{
		if (! $this->redis->del($this->lockKey))
		{
			$this->logger->error('Session: Error while trying to free lock for ' . $this->lockKey);
			return false;
		}

		$this->lockKey = null;
		$this->lock    = false;
	}

	return true;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/RedisHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/MemcachedHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Session.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>