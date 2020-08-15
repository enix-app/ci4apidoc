


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/FileHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/DatabaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/MemcachedHandler.md">next</a></td>
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
<td>framework/system/Session/Handlers/FileHandler.php
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



 
## CodeIgniter\Session\Handlers\FileHandler

<table style="text-align:left">
<tr><th>Class</th><td>FileHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Session\Handlers\FileHandler</td></tr>
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
Session handler using file system for storage
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
<th><a href="#savePath"><strong>savePath</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Where to save the session files to.</td>
</tr>
<tr>
<th><a href="#fileHandle"><strong>fileHandle</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The file handle</td>
</tr>
<tr>
<th><a href="#filePath"><strong>filePath</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>File Name</td>
</tr>
<tr>
<th><a href="#fileNew"><strong>fileNew</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this is a new file.</td>
</tr>
<tr>
<th><a href="#matchIP"><strong>matchIP</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether IP addresses should be matched.</td>
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
<th><a href="#configureSessionIDRegex"><strong>configureSessionIDRegex</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Configure Session ID regular expression</td>
</tr>

</table>





### Properties


<hr>

#### $savePath

```php
protected $savePath;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Where to save the session files to.
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

#### $fileHandle

```php
protected $fileHandle;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The file handle
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

#### $filePath

```php
protected $filePath;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
File Name
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

#### $fileNew

```php
protected $fileNew;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether this is a new file.
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

#### $matchIP

```php
protected $matchIP = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether IP addresses should be matched.
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
public function __construct($config, string $ipAddress)
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
<summary><small>Source: 25 lines (94 - 118)</small></summary>

```php
public function __construct($config, string $ipAddress)
{
	parent::__construct($config, $ipAddress);

	if (! empty($config->sessionSavePath))
	{
		$this->savePath = rtrim($config->sessionSavePath, '/\\');
		ini_set('session.save_path', $config->sessionSavePath);
	}
	else
	{
		$sessionPath = rtrim(ini_get('session.save_path'), '/\\');

		if (! $sessionPath)
		{
			$sessionPath = WRITEPATH . 'session';
		}

		$this->savePath = $sessionPath;
	}

	$this->matchIP = $config->sessionMatchIP;

	$this->configureSessionIDRegex();
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
Sanitizes the save_path directory.
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
<summary><small>Source: 21 lines (133 - 153)</small></summary>

```php
public function open($savePath, $name): bool
{
	if (! is_dir($savePath))
	{
		if (! mkdir($savePath, 0700, true))
		{
			throw SessionException::forInvalidSavePath($this->savePath);
		}
	}
	elseif (! is_writable($savePath))
	{
		throw SessionException::forWriteProtectedSavePath($this->savePath);
	}

	$this->savePath = $savePath;
	$this->filePath = $this->savePath . '/'
					  . $name // we'll use the session cookie name as a prefix to avoid collisions
					  . ($this->matchIP ? md5($this->ipAddress) : '');

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
<summary><small>Source: 59 lines (166 - 224)</small></summary>

```php
public function read($sessionID): string
{
	// This might seem weird, but PHP 5.6 introduced session_reset(),
	// which re-reads session data
	if ($this->fileHandle === null)
	{
		$this->fileNew = ! is_file($this->filePath . $sessionID);

		if (($this->fileHandle = fopen($this->filePath . $sessionID, 'c+b')) === false)
		{
			$this->logger->error("Session: Unable to open file '" . $this->filePath . $sessionID . "'.");

			return false;
		}

		if (flock($this->fileHandle, LOCK_EX) === false)
		{
			$this->logger->error("Session: Unable to obtain lock for file '" . $this->filePath . $sessionID . "'.");
			fclose($this->fileHandle);
			$this->fileHandle = null;

			return false;
		}

		// Needed by write() to detect session_regenerate_id() calls
		if (is_null($this->sessionID))
		{
			$this->sessionID = $sessionID;
		}

		if ($this->fileNew)
		{
			chmod($this->filePath . $sessionID, 0600);
			$this->fingerprint = md5('');

			return '';
		}
	}
	else
	{
		rewind($this->fileHandle);
	}

	$session_data = '';
	clearstatcache();    // Address https://github.com/codeigniter4/CodeIgniter4/issues/2056
	for ($read = 0, $length = filesize($this->filePath . $sessionID); $read < $length; $read += strlen($buffer))
	{
		if (($buffer = fread($this->fileHandle, $length - $read)) === false)
		{
			break;
		}

		$session_data .= $buffer;
	}

	$this->fingerprint = md5($session_data);

	return $session_data;
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
<summary><small>Source: 46 lines (238 - 283)</small></summary>

```php
public function write($sessionID, $sessionData): bool
{
	// If the two IDs don't match, we have a session_regenerate_id() call
	if ($sessionID !== $this->sessionID)
	{
		$this->sessionID = $sessionID;
	}

	if (! is_resource($this->fileHandle))
	{
		return false;
	}
	elseif ($this->fingerprint === md5($sessionData))
	{
		return ($this->fileNew) ? true : touch($this->filePath . $sessionID);
	}

	if (! $this->fileNew)
	{
		ftruncate($this->fileHandle, 0);
		rewind($this->fileHandle);
	}

	if (($length = strlen($sessionData)) > 0)
	{
		for ($written = 0; $written < $length; $written += $result)
		{
			if (($result = fwrite($this->fileHandle, substr($sessionData, $written))) === false)
			{
				break;
			}
		}

		if (! is_int($result))
		{
			$this->fingerprint = md5(substr($sessionData, 0, $written));
			$this->logger->error('Session: Unable to write data.');

			return false;
		}
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
<summary><small>Source: 14 lines (294 - 307)</small></summary>

```php
public function close(): bool
{
	if (is_resource($this->fileHandle))
	{
		flock($this->fileHandle, LOCK_UN);
		fclose($this->fileHandle);

		$this->fileHandle = $this->fileNew = null;

		return true;
	}

	return true;
}
```

</details>


<hr>

#### destroy()

```php
public function destroy($session_id) : bool
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
<td><code>$session_id</code></td>
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
<summary><small>Source: 17 lines (320 - 336)</small></summary>

```php
public function destroy($session_id): bool
{
	if ($this->close())
	{
		return is_file($this->filePath . $session_id)
			? (unlink($this->filePath . $session_id) && $this->destroyCookie()) : true;
	}
	elseif ($this->filePath !== null)
	{
		clearstatcache();

		return is_file($this->filePath . $session_id)
			? (unlink($this->filePath . $session_id) && $this->destroyCookie()) : true;
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
<summary><small>Source: 39 lines (349 - 387)</small></summary>

```php
public function gc($maxlifetime): bool
{
	if (! is_dir($this->savePath) || ($directory = opendir($this->savePath)) === false)
	{
		$this->logger->debug("Session: Garbage collector couldn't list files under directory '" . $this->savePath . "'.");

		return false;
	}

	$ts = time() - $maxlifetime;

	$pattern = $this->matchIP === true
		? '[0-9a-f]{32}'
		: '';

	$pattern = sprintf(
		'#\A%s' . $pattern . $this->sessionIDRegex . '\z#',
		preg_quote($this->cookieName)
	);

	while (($file = readdir($directory)) !== false)
	{
		// If the filename doesn't match this pattern, it's either not a session file or is not ours
		if (! preg_match($pattern, $file)
			|| ! is_file($this->savePath . DIRECTORY_SEPARATOR . $file)
			|| ($mtime = filemtime($this->savePath . DIRECTORY_SEPARATOR . $file)) === false
			|| $mtime > $ts
		)
		{
			continue;
		}

		unlink($this->savePath . DIRECTORY_SEPARATOR . $file);
	}

	closedir($directory);

	return true;
}
```

</details>


<hr>

#### configureSessionIDRegex()

```php
protected function configureSessionIDRegex()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Configure Session ID regular expression
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 28 lines (394 - 421)</small></summary>

```php
protected function configureSessionIDRegex()
{
	$bitsPerCharacter = (int)ini_get('session.sid_bits_per_character');
	$SIDLength        = (int)ini_get('session.sid_length');

	if (($bits = $SIDLength * $bitsPerCharacter) < 160)
	{
		// Add as many more characters as necessary to reach at least 160 bits
		$SIDLength += (int)ceil((160 % $bits) / $bitsPerCharacter);
		ini_set('session.sid_length', $SIDLength);
	}

	// Yes, 4,5,6 are the only known possible values as of 2016-10-27
	switch ($bitsPerCharacter)
	{
		case 4:
			$this->sessionIDRegex = '[0-9a-f]';
			break;
		case 5:
			$this->sessionIDRegex = '[0-9a-v]';
			break;
		case 6:
			$this->sessionIDRegex = '[0-9a-zA-Z,-]';
			break;
	}

	$this->sessionIDRegex .= '{' . $SIDLength . '}';
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/FileHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/DatabaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/MemcachedHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:18**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>