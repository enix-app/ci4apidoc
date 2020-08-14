


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Session.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/RedisHandler.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/SessionInterface.md">next</a></td>
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
<td>framework/system/Session/Session.php
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



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerAwareTrait.md"><strong>Psr\Log\LoggerAwareTrait</strong></a>
</td>
<td>LoggerAwareTrait</td>
</tr>
</table>



 
## CodeIgniter\Session\Session

<table style="text-align:left">
<tr><th>Class</th><td>Session</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Session\Session</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/SessionInterface.md">CodeIgniter\Session\SessionInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Implementation of CodeIgniter session container.
</td></tr>
</table>

<table>
<tr><td>
Session configuration is done through session variables and cookie related
variables in app/config/App.php
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
<th><a href="#driver"><strong>driver</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Instance of the driver to use.</td>
</tr>
<tr>
<th><a href="#sessionDriverName"><strong>sessionDriverName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The storage driver to use: files, database, redis, memcached</td>
</tr>
<tr>
<th><a href="#sessionCookieName"><strong>sessionCookieName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The session cookie name, must contain only [0-9a-z_-] characters.</td>
</tr>
<tr>
<th><a href="#sessionExpiration"><strong>sessionExpiration</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The number of SECONDS you want the session to last.</td>
</tr>
<tr>
<th><a href="#sessionSavePath"><strong>sessionSavePath</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The location to save sessions to, driver dependent..

For the &#039;files&#039; driver, it&#039;s a path to a writable directory.</td>
</tr>
<tr>
<th><a href="#sessionMatchIP"><strong>sessionMatchIP</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether to match the user&#039;s IP address when reading the session data.</td>
</tr>
<tr>
<th><a href="#sessionTimeToUpdate"><strong>sessionTimeToUpdate</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>How many seconds between CI regenerating the session ID.</td>
</tr>
<tr>
<th><a href="#sessionRegenerateDestroy"><strong>sessionRegenerateDestroy</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether to destroy session data associated with the old session ID
when auto-regenerating the session ID. When set to FALSE, the data
will be later deleted by the garbage collector.</td>
</tr>
<tr>
<th><a href="#cookieDomain"><strong>cookieDomain</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The domain name to use for cookies.</td>
</tr>
<tr>
<th><a href="#cookiePath"><strong>cookiePath</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Path used for storing cookies.</td>
</tr>
<tr>
<th><a href="#cookieSecure"><strong>cookieSecure</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cookie will only be set if a secure HTTPS connection exists.</td>
</tr>
<tr>
<th><a href="#sidRegexp"><strong>sidRegexp</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>sid regex expression</td>
</tr>
<tr>
<th><a href="#logger"><strong>logger</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Logger instance to record error messages and warnings.</td>
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
<th><a href="#start"><strong>start</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Initialize the session container and starts up the session.</td>
</tr>
<tr>
<th><a href="#stop"><strong>stop</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Does a full stop of the session:</td>
</tr>
<tr>
<th><a href="#configure"><strong>configure</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Configuration.</td>
</tr>
<tr>
<th><a href="#configureSidLength"><strong>configureSidLength</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Configure session ID length</td>
</tr>
<tr>
<th><a href="#initVars"><strong>initVars</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Handle temporary variables</td>
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
<th><a href="#push"><strong>push</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Push new value onto session value that is array.</td>
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
<th><a href="#__set"><strong>__set</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Magic method to set variables in the session by simply calling
 $session-&gt;foo = bar;</td>
</tr>
<tr>
<th><a href="#__get"><strong>__get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Magic method to get session variables by simply calling
 $foo = $session-&gt;foo;</td>
</tr>
<tr>
<th><a href="#__isset"><strong>__isset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Magic method to check for session variables.</td>
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
<tr>
<th><a href="#setSaveHandler"><strong>setSaveHandler</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Sets the driver as the session handler in PHP.</td>
</tr>
<tr>
<th><a href="#startSession"><strong>startSession</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Starts the session.</td>
</tr>
<tr>
<th><a href="#setCookie"><strong>setCookie</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Takes care of setting the cookie on the client side.</td>
</tr>

</table>





### Properties


<hr>

#### $driver

```php
protected $driver;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instance of the driver to use.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Log\Handlers\HandlerInterface
</td>
</tr>
</table>


<hr>

#### $sessionDriverName

```php
protected $sessionDriverName;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The storage driver to use: files, database, redis, memcached
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

#### $sessionCookieName

```php
protected $sessionCookieName = 'ci_session';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The session cookie name, must contain only [0-9a-z_-] characters.
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

#### $sessionExpiration

```php
protected $sessionExpiration = 7200;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The number of SECONDS you want the session to last.
</td></tr>
</table>

<table>
<tr><td>
Setting it to 0 (zero) means expire when the browser is closed.
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


<hr>

#### $sessionSavePath

```php
protected $sessionSavePath;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The location to save sessions to, driver dependent..

For the 'files' driver, it's a path to a writable directory.
</td></tr>
</table>

<table>
<tr><td>
WARNING: Only absolute paths are supported!

For the 'database' driver, it's a table name.

TODO: address memcache & redis needs

IMPORTANT: You are REQUIRED to set a valid save path!
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

#### $sessionMatchIP

```php
protected $sessionMatchIP = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to match the user's IP address when reading the session data.
</td></tr>
</table>

<table>
<tr><td>
WARNING: If you're using the database driver, don't forget to update
your session table's PRIMARY KEY when changing this setting.
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

#### $sessionTimeToUpdate

```php
protected $sessionTimeToUpdate = 300;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
How many seconds between CI regenerating the session ID.
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


<hr>

#### $sessionRegenerateDestroy

```php
protected $sessionRegenerateDestroy = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to destroy session data associated with the old session ID
when auto-regenerating the session ID. When set to FALSE, the data
will be later deleted by the garbage collector.
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

#### $cookieDomain

```php
protected $cookieDomain = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The domain name to use for cookies.
</td></tr>
</table>

<table>
<tr><td>
Set to .your-domain.com for site-wide cookies.
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

#### $cookiePath

```php
protected $cookiePath = '/';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Path used for storing cookies.
</td></tr>
</table>

<table>
<tr><td>
Typically will be a forward slash.
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

#### $cookieSecure

```php
protected $cookieSecure = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cookie will only be set if a secure HTTPS connection exists.
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

#### $sidRegexp

```php
protected $sidRegexp;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
sid regex expression
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

#### $logger

```php
protected $logger;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Logger instance to record error messages and warnings.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\PSR\Log\LoggerInterface
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(\SessionHandlerInterface $driver, $config)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor.
</td></tr>
</table>

<table>
<tr><td>
Extract configuration settings and save them here.
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
<td><code>$driver</code></td>
<td><em>\SessionHandlerInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$config</code></td>
<td><em>\Config\App
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 18 lines (172 - 189)</small></summary>

```php
public function __construct(\SessionHandlerInterface $driver, $config)
{
	$this->driver = $driver;

	$this->sessionDriverName        = $config->sessionDriver;
	$this->sessionCookieName        = $config->sessionCookieName;
	$this->sessionExpiration        = $config->sessionExpiration;
	$this->sessionSavePath          = $config->sessionSavePath;
	$this->sessionMatchIP           = $config->sessionMatchIP;
	$this->sessionTimeToUpdate      = $config->sessionTimeToUpdate;
	$this->sessionRegenerateDestroy = $config->sessionRegenerateDestroy;

	$this->cookieDomain = $config->cookieDomain;
	$this->cookiePath   = $config->cookiePath;
	$this->cookieSecure = $config->cookieSecure;

	helper('array');
}
```

</details>


<hr>

#### start()

```php
public function start()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Initialize the session container and starts up the session.
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
<summary><small>Source: 71 lines (198 - 268)</small></summary>

```php
public function start()
{
	if (is_cli() && ENVIRONMENT !== 'testing')
	{
		// @codeCoverageIgnoreStart
		$this->logger->debug('Session: Initialization under CLI aborted.');

		return;
		// @codeCoverageIgnoreEnd
	}
	elseif ((bool) ini_get('session.auto_start'))
	{
		$this->logger->error('Session: session.auto_start is enabled in php.ini. Aborting.');

		return;
	}
	elseif (session_status() === PHP_SESSION_ACTIVE)
	{
		$this->logger->warning('Session: Sessions is enabled, and one exists.Please don\'t $session->start();');

		return;
	}

	if (! $this->driver instanceof \SessionHandlerInterface)
	{
		$this->logger->error("Session: Handler '" . $this->driver .
				"' doesn't implement SessionHandlerInterface. Aborting.");
	}

	$this->configure();

	$this->setSaveHandler();

	// Sanitize the cookie, because apparently PHP doesn't do that for userspace handlers
	if (isset($_COOKIE[$this->sessionCookieName]) && (
			! is_string($_COOKIE[$this->sessionCookieName]) || ! preg_match('#\A' . $this->sidRegexp . '\z#', $_COOKIE[$this->sessionCookieName])
			)
	)
	{
		unset($_COOKIE[$this->sessionCookieName]);
	}

	$this->startSession();

	// Is session ID auto-regeneration configured? (ignoring ajax requests)
	if ((empty($_SERVER['HTTP_X_REQUESTED_WITH']) ||
			strtolower($_SERVER['HTTP_X_REQUESTED_WITH']) !== 'xmlhttprequest') && ($regenerate_time = $this->sessionTimeToUpdate) > 0
	)
	{
		if (! isset($_SESSION['__ci_last_regenerate']))
		{
			$_SESSION['__ci_last_regenerate'] = time();
		}
		elseif ($_SESSION['__ci_last_regenerate'] < (time() - $regenerate_time))
		{
			$this->regenerate((bool) $this->sessionRegenerateDestroy);
		}
	}
	// Another work-around ... PHP doesn't seem to send the session cookie
	// unless it is being currently created or regenerated
	elseif (isset($_COOKIE[$this->sessionCookieName]) && $_COOKIE[$this->sessionCookieName] === session_id())
	{
		$this->setCookie();
	}

	$this->initVars();

	$this->logger->info("Session: Class initialized using '" . $this->sessionDriverName . "' driver.");

	return $this;
}
```

</details>


<hr>

#### stop()

```php
public function stop()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does a full stop of the session:
</td></tr>
</table>

<table>
<tr><td>
- destroys the session
- unsets the session id
- destroys the session cookie
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 8 lines (279 - 286)</small></summary>

```php
public function stop()
{
	setcookie(
			$this->sessionCookieName, session_id(), 1, $this->cookiePath, $this->cookieDomain, $this->cookieSecure, true
	);

	session_regenerate_id(true);
}
```

</details>


<hr>

#### configure()

```php
protected function configure()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Configuration.
</td></tr>
</table>

<table>
<tr><td>
Handle input binds and configuration defaults.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 38 lines (295 - 332)</small></summary>

```php
protected function configure()
{
	if (empty($this->sessionCookieName))
	{
		$this->sessionCookieName = ini_get('session.name');
	}
	else
	{
		ini_set('session.name', $this->sessionCookieName);
	}

	session_set_cookie_params(
			$this->sessionExpiration, $this->cookiePath, $this->cookieDomain, $this->cookieSecure, true // HTTP only; Yes, this is intentional and not configurable for security reasons.
	);

	//if (empty($this->sessionExpiration))
	if (! isset($this->sessionExpiration))
	{
		$this->sessionExpiration = (int) ini_get('session.gc_maxlifetime');
	}
	else
	{
		ini_set('session.gc_maxlifetime', (int) $this->sessionExpiration);
	}

	if (! empty($this->sessionSavePath))
	{
		ini_set('session.save_path', $this->sessionSavePath);
	}

	// Security is king
	ini_set('session.use_trans_sid', 0);
	ini_set('session.use_strict_mode', 1);
	ini_set('session.use_cookies', 1);
	ini_set('session.use_only_cookies', 1);

	$this->configureSidLength();
}
```

</details>


<hr>

#### configureSidLength()

```php
protected function configureSidLength()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Configure session ID length
</td></tr>
</table>

<table>
<tr><td>
To make life easier, we used to force SHA-1 and 4 bits per
character on everyone. And of course, someone was unhappy.

Then PHP 7.1 broke backwards-compatibility because ext/session
is such a mess that nobody wants to touch it with a pole stick,
and the one guy who does, nobody has the energy to argue with.

So we were forced to make changes, and OF COURSE something was
going to break and now we have this pile of shit. -- Narf
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 32 lines (351 - 382)</small></summary>

```php
protected function configureSidLength()
{
	$bits_per_character = (int) (ini_get('session.sid_bits_per_character') !== false
		? ini_get('session.sid_bits_per_character')
		: 4);
	$sid_length         = (int) (ini_get('session.sid_length') !== false
		? ini_get('session.sid_length')
		: 40);
	if (($sid_length * $bits_per_character) < 160)
	{
		$bits = ($sid_length * $bits_per_character);
		// Add as many more characters as necessary to reach at least 160 bits
		$sid_length += (int) ceil((160 % $bits) / $bits_per_character);
		ini_set('session.sid_length', $sid_length);
	}

	// Yes, 4,5,6 are the only known possible values as of 2016-10-27
	switch ($bits_per_character)
	{
		case 4:
			$this->sidRegexp = '[0-9a-f]';
			break;
		case 5:
			$this->sidRegexp = '[0-9a-v]';
			break;
		case 6:
			$this->sidRegexp = '[0-9a-zA-Z,-]';
			break;
	}

	$this->sidRegexp .= '{' . $sid_length . '}';
}
```

</details>


<hr>

#### initVars()

```php
protected function initVars()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handle temporary variables
</td></tr>
</table>

<table>
<tr><td>
Clears old "flash" data, marks the new one for deletion and handles
"temp" data deletion.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 28 lines (392 - 419)</small></summary>

```php
protected function initVars()
{
	if (empty($_SESSION['__ci_vars']))
	{
		return;
	}

	$current_time = time();

	foreach ($_SESSION['__ci_vars'] as $key => &$value)
	{
		if ($value === 'new')
		{
			$_SESSION['__ci_vars'][$key] = 'old';
		}
		// Hacky, but 'old' will (implicitly) always be less than time() ;)
		// DO NOT move this above the 'new' check!
		elseif ($value < $current_time)
		{
			unset($_SESSION[$key], $_SESSION['__ci_vars'][$key]);
		}
	}

	if (empty($_SESSION['__ci_vars']))
	{
		unset($_SESSION['__ci_vars']);
	}
}
```

</details>


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
<summary><small>Source: 5 lines (431 - 435)</small></summary>

```php
public function regenerate(bool $destroy = false)
{
	$_SESSION['__ci_last_regenerate'] = time();
	session_regenerate_id($destroy);
}
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
<summary><small>Source: 4 lines (442 - 445)</small></summary>

```php
public function destroy()
{
	session_destroy();
}
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
<summary><small>Source: 21 lines (464 - 484)</small></summary>

```php
public function set($data, $value = null)
{
	if (is_array($data))
	{
		foreach ($data as $key => &$value)
		{
			if (is_int($key))
			{
				$_SESSION[$value] = null;
			}
			else
			{
				$_SESSION[$key] = $value;
			}
		}

		return;
	}

	$_SESSION[$data] = $value;
}
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
<summary><small>Source: 32 lines (500 - 531)</small></summary>

```php
public function get(string $key = null)
{
	if (! empty($key) && (! is_null($value = isset($_SESSION[$key]) ? $_SESSION[$key] : null) || ! is_null($value = dot_array_search($key, $_SESSION ?? []))))
	{
		return $value;
	}
	elseif (empty($_SESSION))
	{
		return $key === null ? [] : null;
	}

	if (! empty($key))
	{
		return null;
	}

	$userdata = [];
	$_exclude = array_merge(
		['__ci_vars'], $this->getFlashKeys(), $this->getTempKeys()
	);

	$keys = array_keys($_SESSION);
	foreach ($keys as $key)
	{
		if (! in_array($key, $_exclude, true))
		{
			$userdata[$key] = $_SESSION[$key];
		}
	}

	return $userdata;
}
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
<summary><small>Source: 4 lines (542 - 545)</small></summary>

```php
public function has(string $key): bool
{
	return isset($_SESSION[$key]);
}
```

</details>


<hr>

#### push()

```php
public function push(string $key, array $data)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Push new value onto session value that is array.
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

<tr>
<td>2.</td>
<td><code>$data</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>value to be pushed to existing session key.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 7 lines (557 - 563)</small></summary>

```php
public function push(string $key, array $data)
{
	if ($this->has($key) && is_array($value = $this->get($key)))
	{
		$this->set($key, array_merge($value, $data));
	}
}
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
<summary><small>Source: 14 lines (576 - 589)</small></summary>

```php
public function remove($key)
{
	if (is_array($key))
	{
		foreach ($key as $k)
		{
			unset($_SESSION[$k]);
		}

		return;
	}

	unset($_SESSION[$key]);
}
```

</details>


<hr>

#### __set()

```php
public function __set(string $key, $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Magic method to set variables in the session by simply calling
 $session->foo = bar;
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
<td>Identifier of the session property to set.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (600 - 603)</small></summary>

```php
public function __set(string $key, $value)
{
	$_SESSION[$key] = $value;
}
```

</details>


<hr>

#### __get()

```php
public function __get(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Magic method to get session variables by simply calling
 $foo = $session->foo;
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
<td>Identifier of the session property to remove.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>null<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (615 - 629)</small></summary>

```php
public function __get(string $key)
{
	// Note: Keep this order the same, just in case somebody wants to
	//       use 'session_id' as a session data key, for whatever reason
	if (isset($_SESSION[$key]))
	{
		return $_SESSION[$key];
	}
	elseif ($key === 'session_id')
	{
		return session_id();
	}

	return null;
}
```

</details>


<hr>

#### __isset()

```php
public function __isset(string $key) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Magic method to check for session variables.
</td></tr>
</table>

<table>
<tr><td>
Different from has() in that it will validate 'session_id' as well.
Mostly used by internal PHP functions, users should stick to has()
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
<td>Identifier of the session property to remove.</td>
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
<summary><small>Source: 4 lines (642 - 645)</small></summary>

```php
public function __isset(string $key): bool
{
	return isset($_SESSION[$key]) || ($key === 'session_id');
}
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
<td><em>array<br>string
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
<summary><small>Source: 5 lines (664 - 668)</small></summary>

```php
public function setFlashdata($data, $value = null)
{
	$this->set($data, $value);
	$this->markAsFlashdata(is_array($data) ? array_keys($data) : $data);
}
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
<summary><small>Source: 20 lines (680 - 699)</small></summary>

```php
public function getFlashdata(string $key = null)
{
	if (isset($key))
	{
		return (isset($_SESSION['__ci_vars'], $_SESSION['__ci_vars'][$key], $_SESSION[$key]) &&
				! is_int($_SESSION['__ci_vars'][$key])) ? $_SESSION[$key] : null;
	}

	$flashdata = [];

	if (! empty($_SESSION['__ci_vars']))
	{
		foreach ($_SESSION['__ci_vars'] as $key => &$value)
		{
			is_int($value) || $flashdata[$key] = $_SESSION[$key];
		}
	}

	return $flashdata;
}
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
<summary><small>Source: 4 lines (708 - 711)</small></summary>

```php
public function keepFlashdata($key)
{
	$this->markAsFlashdata($key);
}
```

</details>


<hr>

#### markAsFlashdata()

```php
public function markAsFlashdata($key) : bool
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
<td><em>array<br>string
</em></td>
<td>false</td>
<td>Property identifier or array of them</td>
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
<summary><small>Source: 28 lines (722 - 749)</small></summary>

```php
public function markAsFlashdata($key): bool
{
	if (is_array($key))
	{
		foreach ($key as $sessionKey)
		{
			if (! isset($_SESSION[$sessionKey]))
			{
				return false;
			}
		}

		$new = array_fill_keys($key, 'new');

		$_SESSION['__ci_vars'] = isset($_SESSION['__ci_vars']) ? array_merge($_SESSION['__ci_vars'], $new) : $new;

		return true;
	}

	if (! isset($_SESSION[$key]))
	{
		return false;
	}

	$_SESSION['__ci_vars'][$key] = 'new';

	return true;
}
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
<td><em>mixed
</em></td>
<td>false</td>
<td>Property identifier or array of them</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 22 lines (758 - 779)</small></summary>

```php
public function unmarkFlashdata($key)
{
	if (empty($_SESSION['__ci_vars']))
	{
		return;
	}

	is_array($key) || $key = [$key];

	foreach ($key as $k)
	{
		if (isset($_SESSION['__ci_vars'][$k]) && ! is_int($_SESSION['__ci_vars'][$k]))
		{
			unset($_SESSION['__ci_vars'][$k]);
		}
	}

	if (empty($_SESSION['__ci_vars']))
	{
		unset($_SESSION['__ci_vars']);
	}
}
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
<summary><small>Source: 15 lines (788 - 802)</small></summary>

```php
public function getFlashKeys(): array
{
	if (! isset($_SESSION['__ci_vars']))
	{
		return [];
	}

	$keys = [];
	foreach (array_keys($_SESSION['__ci_vars']) as $key)
	{
		is_int($_SESSION['__ci_vars'][$key]) || $keys[] = $key;
	}

	return $keys;
}
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
<td><em>null
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
<summary><small>Source: 5 lines (817 - 821)</small></summary>

```php
public function setTempdata($data, $value = null, int $ttl = 300)
{
	$this->set($data, $value);
	$this->markAsTempdata($data, $ttl);
}
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
<summary><small>Source: 20 lines (832 - 851)</small></summary>

```php
public function getTempdata(string $key = null)
{
	if (isset($key))
	{
		return (isset($_SESSION['__ci_vars'], $_SESSION['__ci_vars'][$key], $_SESSION[$key]) &&
				is_int($_SESSION['__ci_vars'][$key])) ? $_SESSION[$key] : null;
	}

	$tempdata = [];

	if (! empty($_SESSION['__ci_vars']))
	{
		foreach ($_SESSION['__ci_vars'] as $key => &$value)
		{
			is_int($value) && $tempdata[$key] = $_SESSION[$key];
		}
	}

	return $tempdata;
}
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
<summary><small>Source: 5 lines (860 - 864)</small></summary>

```php
public function removeTempdata(string $key)
{
	$this->unmarkTempdata($key);
	unset($_SESSION[$key]);
}
```

</details>


<hr>

#### markAsTempdata()

```php
public function markAsTempdata($key, int $ttl = 300) : bool
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
<summary><small>Source: 47 lines (877 - 923)</small></summary>

```php
public function markAsTempdata($key, int $ttl = 300): bool
{
	$ttl += time();

	if (is_array($key))
	{
		$temp = [];

		foreach ($key as $k => $v)
		{
			// Do we have a key => ttl pair, or just a key?
			if (is_int($k))
			{
				$k = $v;
				$v = $ttl;
			}
			elseif (is_string($v))
			{
				$v = time() + $ttl;
			}
			else
			{
				$v += time();
			}

			if (! array_key_exists($k, $_SESSION))
			{
				return false;
			}

			$temp[$k] = $v;
		}

		$_SESSION['__ci_vars'] = isset($_SESSION['__ci_vars']) ? array_merge($_SESSION['__ci_vars'], $temp) : $temp;

		return true;
	}

	if (! isset($_SESSION[$key]))
	{
		return false;
	}

	$_SESSION['__ci_vars'][$key] = $ttl;

	return true;
}
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
<summary><small>Source: 22 lines (933 - 954)</small></summary>

```php
public function unmarkTempdata($key)
{
	if (empty($_SESSION['__ci_vars']))
	{
		return;
	}

	is_array($key) || $key = [$key];

	foreach ($key as $k)
	{
		if (isset($_SESSION['__ci_vars'][$k]) && is_int($_SESSION['__ci_vars'][$k]))
		{
			unset($_SESSION['__ci_vars'][$k]);
		}
	}

	if (empty($_SESSION['__ci_vars']))
	{
		unset($_SESSION['__ci_vars']);
	}
}
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
<summary><small>Source: 15 lines (963 - 977)</small></summary>

```php
public function getTempKeys(): array
{
	if (! isset($_SESSION['__ci_vars']))
	{
		return [];
	}

	$keys = [];
	foreach (array_keys($_SESSION['__ci_vars']) as $key)
	{
		is_int($_SESSION['__ci_vars'][$key]) && $keys[] = $key;
	}

	return $keys;
}
```

</details>


<hr>

#### setSaveHandler()

```php
protected function setSaveHandler()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the driver as the session handler in PHP.
</td></tr>
</table>

<table>
<tr><td>
Extracted for easier testing.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (985 - 988)</small></summary>

```php
protected function setSaveHandler()
{
	session_set_save_handler($this->driver, true);
}
```

</details>


<hr>

#### startSession()

```php
protected function startSession()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Starts the session.
</td></tr>
</table>

<table>
<tr><td>
Extracted for testing reasons.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 12 lines (996 - 1007)</small></summary>

```php
protected function startSession()
{
	if (ENVIRONMENT === 'testing')
	{
		$_SESSION = [];
		return;
	}

	// @codeCoverageIgnoreStart
	session_start();
	// @codeCoverageIgnoreEnd
}
```

</details>


<hr>

#### setCookie()

```php
protected function setCookie()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes care of setting the cookie on the client side.
</td></tr>
</table>

<table>
<tr><td>
Extracted for testing reasons.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 6 lines (1015 - 1020)</small></summary>

```php
protected function setCookie()
{
	setcookie(
			$this->sessionCookieName, session_id(), (empty($this->sessionExpiration) ? 0 : time() + $this->sessionExpiration), $this->cookiePath, $this->cookieDomain, $this->cookieSecure, true
	);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Session.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/RedisHandler.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Session/SessionInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>