


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/DatabaseHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/FileHandler.md">next</a></td>
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
<td>framework/system/Session/Handlers/DatabaseHandler.php
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseConnection.md"><strong>CodeIgniter\Database\BaseConnection</strong></a>
</td>
<td>BaseConnection</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Exceptions/SessionException.md"><strong>CodeIgniter\Session\Exceptions\SessionException</strong></a>
</td>
<td>SessionException</td>
</tr>
<tr>
<td>
<strong>Config\Database</strong>
</td>
<td>Database</td>
</tr>
</table>



 
## CodeIgniter\Session\Handlers\DatabaseHandler

<table style="text-align:left">
<tr><th>Class</th><td>DatabaseHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Session\Handlers\DatabaseHandler</td></tr>
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
Session handler using current Database for storage
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
<th><a href="#DBGroup"><strong>DBGroup</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The database group to use for storage.</td>
</tr>
<tr>
<th><a href="#table"><strong>table</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the table to store session info.</td>
</tr>
<tr>
<th><a href="#db"><strong>db</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The DB Connection instance.</td>
</tr>
<tr>
<th><a href="#platform"><strong>platform</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The database type, for locking purposes.</td>
</tr>
<tr>
<th><a href="#rowExists"><strong>rowExists</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Row exists flag</td>
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
<td>Lock the session.</td>
</tr>
<tr>
<th><a href="#releaseLock"><strong>releaseLock</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Releases the lock, if any.</td>
</tr>

</table>





### Properties


<hr>

#### $DBGroup

```php
protected $DBGroup;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The database group to use for storage.
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

#### $table

```php
protected $table;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the table to store session info.
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

#### $db

```php
protected $db;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The DB Connection instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\BaseConnection
</td>
</tr>
</table>


<hr>

#### $platform

```php
protected $platform;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The database type, for locking purposes.
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

#### $rowExists

```php
protected $rowExists = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Row exists flag
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








<details>
<summary><small>Source: 28 lines (96 - 123)</small></summary>

```php
public function __construct(BaseConfig $config, string $ipAddress)
{
	parent::__construct($config, $ipAddress);

	// Determine Table
	$this->table = $config->sessionSavePath;

	if (empty($this->table))
	{
		throw SessionException::forMissingDatabaseTable();
	}

	// Get DB Connection
	$this->DBGroup = $config->sessionDBGroup ?? config(Database::class)->defaultGroup;

	$this->db = Database::connect($this->DBGroup);

	// Determine Database type
	$driver = strtolower(get_class($this->db));
	if (strpos($driver, 'mysql') !== false)
	{
		$this->platform = 'mysql';
	}
	elseif (strpos($driver, 'postgre') !== false)
	{
		$this->platform = 'postgre';
	}
}
```

</details>


<hr>

#### open()

```php
public function open($savePath, $name) : bool
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
Ensures we have an initialized database connection.
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
<td><code>$savePath</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Path to session files' directory</td>
</tr>

<tr>
<td>2.</td>
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Session cookie name</td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 9 lines (138 - 146)</small></summary>

```php
public function open($savePath, $name): bool
{
	if (empty($this->db->connID))
	{
		$this->db->initialize();
	}

	return true;
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 53 lines (159 - 211)</small></summary>

```php
public function read($sessionID): string
{
	if ($this->lockSession($sessionID) === false)
	{
		$this->fingerprint = md5('');
		return '';
	}

	// Needed by write() to detect session_regenerate_id() calls
	if (is_null($this->sessionID))
	{
		$this->sessionID = $sessionID;
	}

	$builder = $this->db->table($this->table)
			->select('data')
			->where('id', $sessionID);

	if ($this->matchIP)
	{
		$builder = $builder->where('ip_address', $this->ipAddress);
	}

	$result = $builder->get()->getRow();

	if ($result === null)
	{
		// PHP7 will reuse the same SessionHandler object after
		// ID regeneration, so we need to explicitly set this to
		// FALSE instead of relying on the default ...
		$this->rowExists   = false;
		$this->fingerprint = md5('');

		return '';
	}

	// PostgreSQL's variant of a BLOB datatype is Bytea, which is a
	// PITA to work with, so we use base64-encoded data in a TEXT
	// field instead.
	if (is_bool($result))
	{
		$result = '';
	}
	else
	{
		$result = ($this->platform === 'postgre') ? base64_decode(rtrim($result->data)) : $result->data;
	}

	$this->fingerprint = md5($result);
	$this->rowExists   = true;

	return $result;
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
<summary><small>Source: 59 lines (225 - 283)</small></summary>

```php
public function write($sessionID, $sessionData): bool
{
	if ($this->lock === false)
	{
		return $this->fail();
	}

	// Was the ID regenerated?
	elseif ($sessionID !== $this->sessionID)
	{
		$this->rowExists = false;
		$this->sessionID = $sessionID;
	}

	if ($this->rowExists === false)
	{
		$insertData = [
			'id'         => $sessionID,
			'ip_address' => $this->ipAddress,
			'timestamp'  => time(),
			'data'       => $this->platform === 'postgre' ? base64_encode($sessionData) : $sessionData,
		];

		if (! $this->db->table($this->table)->insert($insertData))
		{
			return $this->fail();
		}

		$this->fingerprint = md5($sessionData);
		$this->rowExists   = true;

		return true;
	}

	$builder = $this->db->table($this->table)->where('id', $sessionID);

	if ($this->matchIP)
	{
		$builder = $builder->where('ip_address', $this->ipAddress);
	}

	$updateData = [
		'timestamp' => time(),
	];

	if ($this->fingerprint !== md5($sessionData))
	{
		$updateData['data'] = ($this->platform === 'postgre') ? base64_encode($sessionData) : $sessionData;
	}

	if (! $builder->update($updateData))
	{
		return $this->fail();
	}

	$this->fingerprint = md5($sessionData);

	return true;
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
Releases locks and closes file descriptor.
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
<summary><small>Source: 4 lines (294 - 297)</small></summary>

```php
public function close(): bool
{
	return ($this->lock && ! $this->releaseLock()) ? $this->fail() : true;
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
<summary><small>Source: 26 lines (310 - 335)</small></summary>

```php
public function destroy($sessionID): bool
{
	if ($this->lock)
	{
		$builder = $this->db->table($this->table)->where('id', $sessionID);

		if ($this->matchIP)
		{
			$builder = $builder->where('ip_address', $this->ipAddress);
		}

		if (! $builder->delete())
		{
			return $this->fail();
		}
	}

	if ($this->close())
	{
		$this->destroyCookie();

		return true;
	}

	return $this->fail();
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
<summary><small>Source: 4 lines (348 - 351)</small></summary>

```php
public function gc($maxlifetime): bool
{
	return ($this->db->table($this->table)->delete('timestamp < ' . (time() - $maxlifetime))) ? true : $this->fail();
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
Lock the session.
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
<summary><small>Source: 28 lines (361 - 388)</small></summary>

```php
protected function lockSession(string $sessionID): bool
{
	if ($this->platform === 'mysql')
	{
		$arg = md5($sessionID . ($this->matchIP ? '_' . $this->ipAddress : ''));
		if ($this->db->query("SELECT GET_LOCK('{$arg}', 300) AS ci_session_lock")->getRow()->ci_session_lock)
		{
			$this->lock = $arg;
			return true;
		}

		return $this->fail();
	}
	elseif ($this->platform === 'postgre')
	{
		$arg = "hashtext('{$sessionID}')" . ($this->matchIP ? ", hashtext('{$this->ipAddress}')" : '');
		if ($this->db->simpleQuery("SELECT pg_advisory_lock({$arg})"))
		{
			$this->lock = $arg;
			return true;
		}

		return $this->fail();
	}

	// Unsupported DB? Let the parent handle the simplified version.
	return parent::lockSession($sessionID);
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
Releases the lock, if any.
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
<summary><small>Source: 31 lines (397 - 427)</small></summary>

```php
protected function releaseLock(): bool
{
	if (! $this->lock)
	{
		return true;
	}

	if ($this->platform === 'mysql')
	{
		if ($this->db->query("SELECT RELEASE_LOCK('{$this->lock}') AS ci_session_lock")->getRow()->ci_session_lock)
		{
			$this->lock = false;
			return true;
		}

		return $this->fail();
	}
	elseif ($this->platform === 'postgre')
	{
		if ($this->db->simpleQuery("SELECT pg_advisory_unlock({$this->lock})"))
		{
			$this->lock = false;
			return true;
		}

		return $this->fail();
	}

	// Unsupported DB? Let the parent handle the simple version.
	return parent::releaseLock();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/DatabaseHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/FileHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>