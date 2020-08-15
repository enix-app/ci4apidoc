


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/MySQLi/Connection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Builder.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Forge.md">next</a></td>
</tr>
</table>







# CodeIgniter\Database\MySQLi 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Database\MySQLi</td></tr>
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
<td>framework/system/Database/MySQLi/Connection.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Builder.md">CodeIgniter\Database\MySQLi\Builder</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Connection.md">CodeIgniter\Database\MySQLi\Connection</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Forge.md">CodeIgniter\Database\MySQLi\Forge</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/PreparedQuery.md">CodeIgniter\Database\MySQLi\PreparedQuery</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Result.md">CodeIgniter\Database\MySQLi\Result</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Utils.md">CodeIgniter\Database\MySQLi\Utils</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseConnection.md"><strong>CodeIgniter\Database\BaseConnection</strong></a>
</td>
<td>BaseConnection</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/ConnectionInterface.md"><strong>CodeIgniter\Database\ConnectionInterface</strong></a>
</td>
<td>ConnectionInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DatabaseException.md"><strong>CodeIgniter\Database\Exceptions\DatabaseException</strong></a>
</td>
<td>DatabaseException</td>
</tr>
</table>



 
## CodeIgniter\Database\MySQLi\Connection

<table style="text-align:left">
<tr><th>Class</th><td>Connection</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\MySQLi\Connection</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseConnection.md">CodeIgniter\Database\BaseConnection</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/ConnectionInterface.md">CodeIgniter\Database\ConnectionInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Connection for MySQLi
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
<th><a href="#DBDriver"><strong>DBDriver</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Database driver</td>
</tr>
<tr>
<th><a href="#deleteHack"><strong>deleteHack</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>DELETE hack flag</td>
</tr>
<tr>
<th><a href="#escapeChar"><strong>escapeChar</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Identifier escape character</td>
</tr>
<tr>
<th><a href="#mysqli"><strong>mysqli</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>MySQLi object</td>
</tr>

<tr>
<th><a href="#connect"><strong>connect</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Connect to the database.</td>
</tr>
<tr>
<th><a href="#reconnect"><strong>reconnect</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Keep or establish the connection if no queries have been sent for
a length of time exceeding the server&#039;s idle timeout.</td>
</tr>
<tr>
<th><a href="#_close"><strong>_close</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Close the database connection.</td>
</tr>
<tr>
<th><a href="#setDatabase"><strong>setDatabase</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Select a specific database table to use.</td>
</tr>
<tr>
<th><a href="#getVersion"><strong>getVersion</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a string containing the version of the database being used.</td>
</tr>
<tr>
<th><a href="#execute"><strong>execute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Executes the query against the database.</td>
</tr>
<tr>
<th><a href="#prepQuery"><strong>prepQuery</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Prep the query</td>
</tr>
<tr>
<th><a href="#affectedRows"><strong>affectedRows</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the total number of rows affected by this query.</td>
</tr>
<tr>
<th><a href="#_escapeString"><strong>_escapeString</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Platform-dependant string escape</td>
</tr>
<tr>
<th><a href="#escapeLikeStringDirect"><strong>escapeLikeStringDirect</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Escape Like String Direct
There are a few instances where MySQLi queries cannot take the
additional &quot;ESCAPE x&quot; parameter for specifying the escape character
in &quot;LIKE&quot; strings, and this handles those directly with a backslash.</td>
</tr>
<tr>
<th><a href="#_listTables"><strong>_listTables</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Generates the SQL for listing tables in a platform-dependent manner.</td>
</tr>
<tr>
<th><a href="#_listColumns"><strong>_listColumns</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Generates a platform-specific query string so that the column names can be fetched.</td>
</tr>
<tr>
<th><a href="#_fieldData"><strong>_fieldData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an array of objects with field data</td>
</tr>
<tr>
<th><a href="#_indexData"><strong>_indexData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an array of objects with index data</td>
</tr>
<tr>
<th><a href="#_foreignKeyData"><strong>_foreignKeyData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an array of objects with Foreign key data</td>
</tr>
<tr>
<th><a href="#_disableForeignKeyChecks"><strong>_disableForeignKeyChecks</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Returns platform-specific SQL to disable foreign key checks.</td>
</tr>
<tr>
<th><a href="#_enableForeignKeyChecks"><strong>_enableForeignKeyChecks</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Returns platform-specific SQL to enable foreign key checks.</td>
</tr>
<tr>
<th><a href="#error"><strong>error</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the last error code and message.</td>
</tr>
<tr>
<th><a href="#insertID"><strong>insertID</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Insert ID</td>
</tr>
<tr>
<th><a href="#_transBegin"><strong>_transBegin</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Begin Transaction</td>
</tr>
<tr>
<th><a href="#_transCommit"><strong>_transCommit</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Commit Transaction</td>
</tr>
<tr>
<th><a href="#_transRollback"><strong>_transRollback</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Rollback Transaction</td>
</tr>

</table>





### Properties


<hr>

#### $DBDriver

```php
public $DBDriver = 'MySQLi';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Database driver
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

#### $deleteHack

```php
public $deleteHack = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
DELETE hack flag
</td></tr>
</table>

<table>
<tr><td>
Whether to use the MySQL "delete hack" which allows the number
of affected rows to be shown. Uses a preg_replace when enabled,
adding a bit more processing to all queries.
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

#### $escapeChar

```php
public $escapeChar = '`';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Identifier escape character
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

#### $mysqli

```php
public $mysqli;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
MySQLi object
</td></tr>
</table>

<table>
<tr><td>
Has to be preserved without being assigned to $conn_id.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\MySQLi
</td>
</tr>
</table>







### Methods


<hr>

#### connect()

```php
public function connect(bool $persistent = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Connect to the database.
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
<td><code>$persistent</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Database\Exceptions\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 137 lines (93 - 229)</small></summary>

```php
public function connect(bool $persistent = false)
{
	// Do we have a socket path?
	if ($this->hostname[0] === '/')
	{
		$hostname = null;
		$port     = null;
		$socket   = $this->hostname;
	}
	else
	{
		$hostname = ($persistent === true) ? 'p:' . $this->hostname : $this->hostname;
		$port     = empty($this->port) ? null : $this->port;
		$socket   = '';
	}

	$client_flags = ($this->compress === true) ? MYSQLI_CLIENT_COMPRESS : 0;
	$this->mysqli = mysqli_init();

	mysqli_report(MYSQLI_REPORT_ALL & ~MYSQLI_REPORT_INDEX);

	$this->mysqli->options(MYSQLI_OPT_CONNECT_TIMEOUT, 10);

	if (isset($this->strictOn))
	{
		if ($this->strictOn)
		{
			$this->mysqli->options(MYSQLI_INIT_COMMAND,
				'SET SESSION sql_mode = CONCAT(@@sql_mode, ",", "STRICT_ALL_TABLES")');
		}
		else
		{
			$this->mysqli->options(MYSQLI_INIT_COMMAND, 'SET SESSION sql_mode =
					REPLACE(REPLACE(REPLACE(REPLACE(REPLACE(REPLACE(
											@@sql_mode,
											"STRICT_ALL_TABLES,", ""),
										",STRICT_ALL_TABLES", ""),
									"STRICT_ALL_TABLES", ""),
								"STRICT_TRANS_TABLES,", ""),
							",STRICT_TRANS_TABLES", ""),
						"STRICT_TRANS_TABLES", "")'
			);
		}
	}

	if (is_array($this->encrypt))
	{
		$ssl                                                  = [];
		empty($this->encrypt['ssl_key']) || $ssl['key']       = $this->encrypt['ssl_key'];
		empty($this->encrypt['ssl_cert']) || $ssl['cert']     = $this->encrypt['ssl_cert'];
		empty($this->encrypt['ssl_ca']) || $ssl['ca']         = $this->encrypt['ssl_ca'];
		empty($this->encrypt['ssl_capath']) || $ssl['capath'] = $this->encrypt['ssl_capath'];
		empty($this->encrypt['ssl_cipher']) || $ssl['cipher'] = $this->encrypt['ssl_cipher'];

		if (! empty($ssl))
		{
			if (isset($this->encrypt['ssl_verify']))
			{
				if ($this->encrypt['ssl_verify'])
				{
					defined('MYSQLI_OPT_SSL_VERIFY_SERVER_CERT') &&
					$this->mysqli->options(MYSQLI_OPT_SSL_VERIFY_SERVER_CERT, true);
				}
				// Apparently (when it exists), setting MYSQLI_OPT_SSL_VERIFY_SERVER_CERT
				// to FALSE didn't do anything, so PHP 5.6.16 introduced yet another
				// constant ...
				//
				// https://secure.php.net/ChangeLog-5.php#5.6.16
				// https://bugs.php.net/bug.php?id=68344
				elseif (defined('MYSQLI_CLIENT_SSL_DONT_VERIFY_SERVER_CERT') && version_compare($this->mysqli->client_info, '5.6', '>='))
				{
					$client_flags += MYSQLI_CLIENT_SSL_DONT_VERIFY_SERVER_CERT;
				}
			}

			$client_flags += MYSQLI_CLIENT_SSL;
			$this->mysqli->ssl_set(
				$ssl['key'] ?? null, $ssl['cert'] ?? null, $ssl['ca'] ?? null,
				$ssl['capath'] ?? null, $ssl['cipher'] ?? null
			);
		}
	}

	try
	{
		if ($this->mysqli->real_connect($hostname, $this->username, $this->password,
			$this->database, $port, $socket, $client_flags)
		)
		{
			// Prior to version 5.7.3, MySQL silently downgrades to an unencrypted connection if SSL setup fails
			if (($client_flags & MYSQLI_CLIENT_SSL) && version_compare($this->mysqli->client_info, '5.7.3', '<=')
				&& empty($this->mysqli->query("SHOW STATUS LIKE 'ssl_cipher'")
									  ->fetch_object()->Value)
			)
			{
				$this->mysqli->close();
				$message = 'MySQLi was configured for an SSL connection, but got an unencrypted connection instead!';
				log_message('error', $message);

				if ($this->DBDebug)
				{
					throw new DatabaseException($message);
				}

				return false;
			}

			if (! $this->mysqli->set_charset($this->charset))
			{
				log_message('error',
					"Database: Unable to set the configured connection charset ('{$this->charset}').");
				$this->mysqli->close();

				if ($this->DBDebug)
				{
					throw new DatabaseException('Unable to set client connection character set: ' . $this->charset);
				}

				return false;
			}

			return $this->mysqli;
		}
	}
	catch (\Throwable $e)
	{
		// Clean sensitive information from errors.
		$msg = $e->getMessage();

		$msg = str_replace($this->username, '****', $msg);
		$msg = str_replace($this->password, '****', $msg);

		throw new DatabaseException($msg, $e->getCode(), $e);
	}

	return false;
}
```

</details>


<hr>

#### reconnect()

```php
public function reconnect()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Keep or establish the connection if no queries have been sent for
a length of time exceeding the server's idle timeout.
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
<summary><small>Source: 5 lines (239 - 243)</small></summary>

```php
public function reconnect()
{
	$this->close();
	$this->initialize();
}
```

</details>


<hr>

#### _close()

```php
protected function _close()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Close the database connection.
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
<summary><small>Source: 4 lines (252 - 255)</small></summary>

```php
protected function _close()
{
	$this->connID->close();
}
```

</details>


<hr>

#### setDatabase()

```php
public function setDatabase(string $databaseName) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Select a specific database table to use.
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
<td><code>$databaseName</code></td>
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
<summary><small>Source: 21 lines (266 - 286)</small></summary>

```php
public function setDatabase(string $databaseName): bool
{
	if ($databaseName === '')
	{
		$databaseName = $this->database;
	}

	if (empty($this->connID))
	{
		$this->initialize();
	}

	if ($this->connID->select_db($databaseName))
	{
		$this->database = $databaseName;

		return true;
	}

	return false;
}
```

</details>


<hr>

#### getVersion()

```php
public function getVersion() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a string containing the version of the database being used.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (295 - 308)</small></summary>

```php
public function getVersion(): string
{
	if (isset($this->dataCache['version']))
	{
		return $this->dataCache['version'];
	}

	if (empty($this->mysqli))
	{
		$this->initialize();
	}

	return $this->dataCache['version'] = $this->mysqli->server_info;
}
```

</details>


<hr>

#### execute()

```php
public function execute(string $sql)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Executes the query against the database.
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
<td><code>$sql</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 24 lines (319 - 342)</small></summary>

```php
public function execute(string $sql)
{
	while ($this->connID->more_results())
	{
		$this->connID->next_result();
		if ($res = $this->connID->store_result())
		{
			$res->free();
		}
	}
	try
	{
		return $this->connID->query($this->prepQuery($sql));
	}
	catch (\mysqli_sql_exception $e)
	{
		log_message('error', $e);
		if ($this->DBDebug)
		{
			throw $e;
		}
	}
	return false;
}
```

</details>


<hr>

#### prepQuery()

```php
protected function prepQuery(string $sql) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prep the query
</td></tr>
</table>

<table>
<tr><td>
If needed, each database adapter can prep the query string
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
<td><code>$sql</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>an SQL query</td>
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
<summary><small>Source: 11 lines (355 - 365)</small></summary>

```php
protected function prepQuery(string $sql): string
{
	// mysqli_affected_rows() returns 0 for "DELETE FROM TABLE" queries. This hack
	// modifies the query so that it a proper number of affected rows is returned.
	if ($this->deleteHack === true && preg_match('/^\s*DELETE\s+FROM\s+(\S+)\s*$/i', $sql))
	{
		return trim($sql) . ' WHERE 1=1';
	}

	return $sql;
}
```

</details>


<hr>

#### affectedRows()

```php
public function affectedRows() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the total number of rows affected by this query.
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
<summary><small>Source: 4 lines (374 - 377)</small></summary>

```php
public function affectedRows(): int
{
	return $this->connID->affected_rows ?? 0;
}
```

</details>


<hr>

#### _escapeString()

```php
protected function _escapeString(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Platform-dependant string escape
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
<td><code>$str</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (387 - 400)</small></summary>

```php
protected function _escapeString(string $str): string
{
	if (is_bool($str))
	{
		return $str;
	}

	if (! $this->connID)
	{
		$this->initialize();
	}

	return $this->connID->real_escape_string($str);
}
```

</details>


<hr>

#### escapeLikeStringDirect()

```php
public function escapeLikeStringDirect($str)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Escape Like String Direct
There are a few instances where MySQLi queries cannot take the
additional "ESCAPE x" parameter for specifying the escape character
in "LIKE" strings, and this handles those directly with a backslash.
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
<td><code>$str</code></td>
<td><em>string<br>string[]
</em></td>
<td>false</td>
<td>Input string</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>string[]
</td>
</tr>
</table>





<details>
<summary><small>Source: 26 lines (413 - 438)</small></summary>

```php
public function escapeLikeStringDirect($str)
{
	if (is_array($str))
	{
		foreach ($str as $key => $val)
		{
			$str[$key] = $this->escapeLikeStringDirect($val);
		}

		return $str;
	}

	$str = $this->_escapeString($str);

	// Escape LIKE condition wildcards
	return str_replace([
		$this->likeEscapeChar,
		'%',
		'_',
	], [
		'\\' . $this->likeEscapeChar,
		'\\' . '%',
		'\\' . '_',
	], $str
	);
}
```

</details>


<hr>

#### _listTables()

```php
protected function _listTables(bool $prefixLimit = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates the SQL for listing tables in a platform-dependent manner.
</td></tr>
</table>

<table>
<tr><td>
Uses escapeLikeStringDirect().
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
<td><code>$prefixLimit</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
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
<summary><small>Source: 11 lines (450 - 460)</small></summary>

```php
protected function _listTables(bool $prefixLimit = false): string
{
	$sql = 'SHOW TABLES FROM ' . $this->escapeIdentifiers($this->database);

	if ($prefixLimit !== false && $this->DBPrefix !== '')
	{
		return $sql . " LIKE '" . $this->escapeLikeStringDirect($this->DBPrefix) . "%'";
	}

	return $sql;
}
```

</details>


<hr>

#### _listColumns()

```php
protected function _listColumns(string $table = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates a platform-specific query string so that the column names can be fetched.
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
<td><code>$table</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (471 - 474)</small></summary>

```php
protected function _listColumns(string $table = ''): string
{
	return 'SHOW COLUMNS FROM ' . $this->protectIdentifiers($table, true, null, false);
}
```

</details>


<hr>

#### _fieldData()

```php
public function _fieldData(string $table) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array of objects with field data
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
<td><code>$table</code></td>
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
<td>\stdClass[]
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 25 lines (485 - 509)</small></summary>

```php
public function _fieldData(string $table): array
{
	$table = $this->protectIdentifiers($table, true, null, false);

	if (($query = $this->query('SHOW COLUMNS FROM ' . $table)) === false)
	{
		throw new DatabaseException(lang('Database.failGetFieldData'));
	}
	$query = $query->getResultObject();

	$retVal = [];
	for ($i = 0, $c = count($query); $i < $c; $i++)
	{
		$retVal[$i]       = new \stdClass();
		$retVal[$i]->name = $query[$i]->Field;

		sscanf($query[$i]->Type, '%[a-z](%d)', $retVal[$i]->type, $retVal[$i]->max_length);

		$retVal[$i]->nullable    = $query[$i]->Null === 'YES';
		$retVal[$i]->default     = $query[$i]->Default;
		$retVal[$i]->primary_key = (int)($query[$i]->Key === 'PRI');
	}

	return $retVal;
}
```

</details>


<hr>

#### _indexData()

```php
public function _indexData(string $table) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array of objects with index data
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
<td><code>$table</code></td>
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
<td>\stdClass[]
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\DatabaseException
</td>
</tr>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\LogicException
</td>
</tr>
</table>



<details>
<summary><small>Source: 55 lines (521 - 575)</small></summary>

```php
public function _indexData(string $table): array
{
	$table = $this->protectIdentifiers($table, true, null, false);

	if (($query = $this->query('SHOW INDEX FROM ' . $table)) === false)
	{
		throw new DatabaseException(lang('Database.failGetIndexData'));
	}

	if (! $indexes = $query->getResultArray())
	{
		return [];
	}

	$keys = [];

	foreach ($indexes as $index)
	{
		if (empty($keys[$index['Key_name']]))
		{
			$keys[$index['Key_name']]       = new \stdClass();
			$keys[$index['Key_name']]->name = $index['Key_name'];

			if ($index['Key_name'] === 'PRIMARY')
			{
				$type = 'PRIMARY';
			}
			elseif ($index['Index_type'] === 'FULLTEXT')
			{
				$type = 'FULLTEXT';
			}
			elseif ($index['Non_unique'])
			{
				if ($index['Index_type'] === 'SPATIAL')
				{
					$type = 'SPATIAL';
				}
				else
				{
					$type = 'INDEX';
				}
			}
			else
			{
				$type = 'UNIQUE';
			}

			$keys[$index['Key_name']]->type = $type;
		}

		$keys[$index['Key_name']]->fields[] = $index['Column_name'];
	}

	return $keys;
}
```

</details>


<hr>

#### _foreignKeyData()

```php
public function _foreignKeyData(string $table) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array of objects with Foreign key data
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
<td><code>$table</code></td>
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
<td>\stdClass[]
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 40 lines (586 - 625)</small></summary>

```php
public function _foreignKeyData(string $table): array
{
	$sql = '
                   SELECT
                       tc.CONSTRAINT_NAME,
                       tc.TABLE_NAME,
                       kcu.COLUMN_NAME,
                       rc.REFERENCED_TABLE_NAME,
                       kcu.REFERENCED_COLUMN_NAME
                   FROM information_schema.TABLE_CONSTRAINTS AS tc
                   INNER JOIN information_schema.REFERENTIAL_CONSTRAINTS AS rc
                       ON tc.CONSTRAINT_NAME = rc.CONSTRAINT_NAME
                   INNER JOIN information_schema.KEY_COLUMN_USAGE AS kcu
                       ON tc.CONSTRAINT_NAME = kcu.CONSTRAINT_NAME
                   WHERE
                       tc.CONSTRAINT_TYPE = ' . $this->escape('FOREIGN KEY') . ' AND
                       tc.TABLE_SCHEMA = ' . $this->escape($this->database) . ' AND
                       tc.TABLE_NAME = ' . $this->escape($table);

	if (($query = $this->query($sql)) === false)
	{
		throw new DatabaseException(lang('Database.failGetForeignKeyData'));
	}
	$query = $query->getResultObject();

	$retVal = [];
	foreach ($query as $row)
	{
		$obj                      = new \stdClass();
		$obj->constraint_name     = $row->CONSTRAINT_NAME;
		$obj->table_name          = $row->TABLE_NAME;
		$obj->column_name         = $row->COLUMN_NAME;
		$obj->foreign_table_name  = $row->REFERENCED_TABLE_NAME;
		$obj->foreign_column_name = $row->REFERENCED_COLUMN_NAME;

		$retVal[] = $obj;
	}

	return $retVal;
}
```

</details>


<hr>

#### _disableForeignKeyChecks()

```php
protected function _disableForeignKeyChecks()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns platform-specific SQL to disable foreign key checks.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (634 - 637)</small></summary>

```php
protected function _disableForeignKeyChecks()
{
	return 'SET FOREIGN_KEY_CHECKS=0';
}
```

</details>


<hr>

#### _enableForeignKeyChecks()

```php
protected function _enableForeignKeyChecks()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns platform-specific SQL to enable foreign key checks.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (646 - 649)</small></summary>

```php
protected function _enableForeignKeyChecks()
{
	return 'SET FOREIGN_KEY_CHECKS=1';
}
```

</details>


<hr>

#### error()

```php
public function error() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the last error code and message.
</td></tr>
</table>

<table>
<tr><td>
Must return an array with keys 'code' and 'message':

return ['code' => null, 'message' => null);
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
<summary><small>Source: 15 lines (662 - 676)</small></summary>

```php
public function error(): array
{
	if (! empty($this->mysqli->connect_errno))
	{
		return [
			'code'    => $this->mysqli->connect_errno,
			'message' => $this->mysqli->connect_error,
		];
	}

	return [
		'code'    => $this->connID->errno,
		'message' => $this->connID->error,
	];
}
```

</details>


<hr>

#### insertID()

```php
public function insertID() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Insert ID
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
<summary><small>Source: 4 lines (685 - 688)</small></summary>

```php
public function insertID(): int
{
	return $this->connID->insert_id;
}
```

</details>


<hr>

#### _transBegin()

```php
protected function _transBegin() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Begin Transaction
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
<summary><small>Source: 6 lines (697 - 702)</small></summary>

```php
protected function _transBegin(): bool
{
	$this->connID->autocommit(false);

	return $this->connID->begin_transaction();
}
```

</details>


<hr>

#### _transCommit()

```php
protected function _transCommit() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Commit Transaction
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
<summary><small>Source: 11 lines (711 - 721)</small></summary>

```php
protected function _transCommit(): bool
{
	if ($this->connID->commit())
	{
		$this->connID->autocommit(true);

		return true;
	}

	return false;
}
```

</details>


<hr>

#### _transRollback()

```php
protected function _transRollback() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Rollback Transaction
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
<summary><small>Source: 11 lines (730 - 740)</small></summary>

```php
protected function _transRollback(): bool
{
	if ($this->connID->rollback())
	{
		$this->connID->autocommit(true);

		return true;
	}

	return false;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/MySQLi/Connection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Builder.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Forge.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>