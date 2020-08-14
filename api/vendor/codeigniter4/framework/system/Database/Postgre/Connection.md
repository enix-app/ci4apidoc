


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/Connection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Builder.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Forge.md">next</a></td>
</tr>
</table>







# CodeIgniter\Database\Postgre 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Database\Postgre</td></tr>
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
<td>framework/system/Database/Postgre/Connection.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Builder.md">CodeIgniter\Database\Postgre\Builder</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Connection.md">CodeIgniter\Database\Postgre\Connection</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Forge.md">CodeIgniter\Database\Postgre\Forge</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/PreparedQuery.md">CodeIgniter\Database\Postgre\PreparedQuery</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Result.md">CodeIgniter\Database\Postgre\Result</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Utils.md">CodeIgniter\Database\Postgre\Utils</a></td></tr>
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



 
## CodeIgniter\Database\Postgre\Connection

<table style="text-align:left">
<tr><th>Class</th><td>Connection</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\Postgre\Connection</td></tr>
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
Connection for Postgre
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
<th><a href="#schema"><strong>schema</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Database schema</td>
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
<th><a href="#affectedRows"><strong>affectedRows</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the total number of rows affected by this query.</td>
</tr>
<tr>
<th><a href="#escape"><strong>escape</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>&quot;Smart&quot; Escape String</td>
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
<th><a href="#buildDSN"><strong>buildDSN</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Build a DSN from the provided parameters</td>
</tr>
<tr>
<th><a href="#setClientEncoding"><strong>setClientEncoding</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Set client encoding</td>
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
public $DBDriver = 'postgre';
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

#### $schema

```php
public $schema = 'public';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Database schema
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

#### $escapeChar

```php
public $escapeChar = '"';
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





<details>
<summary><small>Source: 36 lines (82 - 117)</small></summary>

```php
public function connect(bool $persistent = false)
{
	if (empty($this->DSN))
	{
		$this->buildDSN();
	}

	// Strip pgsql if exists
	if (mb_strpos($this->DSN, 'pgsql:') === 0)
	{
		$this->DSN = mb_substr($this->DSN, 6);
	}

	// Convert semicolons to spaces.
	$this->DSN = str_replace(';', ' ', $this->DSN);

	$this->connID = $persistent === true ? pg_pconnect($this->DSN) : pg_connect($this->DSN);

	if ($this->connID !== false)
	{
		if ($persistent === true && pg_connection_status($this->connID) === PGSQL_CONNECTION_BAD && pg_ping($this->connID) === false
		)
		{
			return false;
		}

		empty($this->schema) || $this->simpleQuery("SET search_path TO {$this->schema},public");

		if ($this->setClientEncoding($this->charset) === false)
		{
			return false;
		}
	}

	return $this->connID;
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
<summary><small>Source: 7 lines (127 - 133)</small></summary>

```php
public function reconnect()
{
	if (pg_ping($this->connID) === false)
	{
		$this->connID = false;
	}
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
<summary><small>Source: 4 lines (142 - 145)</small></summary>

```php
protected function _close()
{
	pg_close($this->connID);
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
<summary><small>Source: 4 lines (156 - 159)</small></summary>

```php
public function setDatabase(string $databaseName): bool
{
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
<summary><small>Source: 14 lines (168 - 181)</small></summary>

```php
public function getVersion(): string
{
	if (isset($this->dataCache['version']))
	{
		return $this->dataCache['version'];
	}

	if (! $this->connID || ( $pgVersion = pg_version($this->connID)) === false)
	{
		$this->initialize();
	}

	return isset($pgVersion['server']) ? $this->dataCache['version'] = $pgVersion['server'] : false;
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
<summary><small>Source: 16 lines (192 - 207)</small></summary>

```php
public function execute(string $sql)
{
	try
	{
		return pg_query($this->connID, $sql);
	}
	catch (\ErrorException $e)
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
<summary><small>Source: 4 lines (216 - 219)</small></summary>

```php
public function affectedRows(): int
{
	return pg_affected_rows($this->resultID);
}
```

</details>


<hr>

#### escape()

```php
public function escape($str)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
"Smart" Escape String
</td></tr>
</table>

<table>
<tr><td>
Escapes data based on type
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
<td><em>mixed
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
<summary><small>Source: 18 lines (231 - 248)</small></summary>

```php
public function escape($str)
{
	if (! $this->connID)
	{
		$this->initialize();
	}

	if (is_string($str) || ( is_object($str) && method_exists($str, '__toString')))
	{
		return pg_escape_literal($this->connID, $str);
	}
	elseif (is_bool($str))
	{
		return $str ? 'TRUE' : 'FALSE';
	}

	return parent::escape($str);
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
<summary><small>Source: 9 lines (258 - 266)</small></summary>

```php
protected function _escapeString(string $str): string
{
	if (! $this->connID)
	{
		$this->initialize();
	}

	return pg_escape_string($this->connID, $str);
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
<summary><small>Source: 13 lines (277 - 289)</small></summary>

```php
protected function _listTables(bool $prefixLimit = false): string
{
	$sql = 'SELECT "table_name" FROM "information_schema"."tables" WHERE "table_schema" = \'' . $this->schema . "'";

	if ($prefixLimit !== false && $this->DBPrefix !== '')
	{
		return $sql . ' AND "table_name" LIKE \''
				. $this->escapeLikeString($this->DBPrefix) . "%' "
				. sprintf($this->likeEscapeStr, $this->likeEscapeChar);
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
<summary><small>Source: 7 lines (300 - 306)</small></summary>

```php
protected function _listColumns(string $table = ''): string
{
	return 'SELECT "column_name"
		FROM "information_schema"."columns"
		WHERE LOWER("table_name") = '
			. $this->escape($this->DBPrefix . strtolower($table));
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
<summary><small>Source: 25 lines (317 - 341)</small></summary>

```php
public function _fieldData(string $table): array
{
	$sql = 'SELECT "column_name", "data_type", "character_maximum_length", "numeric_precision", "column_default"
		FROM "information_schema"."columns"
		WHERE LOWER("table_name") = '
			. $this->escape(strtolower($table));

	if (($query = $this->query($sql)) === false)
	{
		throw new DatabaseException(lang('Database.failGetFieldData'));
	}
	$query = $query->getResultObject();

	$retVal = [];
	for ($i = 0, $c = count($query); $i < $c; $i ++)
	{
		$retVal[$i]             = new \stdClass();
		$retVal[$i]->name       = $query[$i]->column_name;
		$retVal[$i]->type       = $query[$i]->data_type;
		$retVal[$i]->default    = $query[$i]->column_default;
		$retVal[$i]->max_length = $query[$i]->character_maximum_length > 0 ? $query[$i]->character_maximum_length : $query[$i]->numeric_precision;
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
</table>



<details>
<summary><small>Source: 37 lines (352 - 388)</small></summary>

```php
public function _indexData(string $table): array
{
	$sql = 'SELECT "indexname", "indexdef"
		FROM "pg_indexes"
		WHERE LOWER("tablename") = ' . $this->escape(strtolower($table)) . '
		AND "schemaname" = ' . $this->escape('public');

	if (($query = $this->query($sql)) === false)
	{
		throw new DatabaseException(lang('Database.failGetIndexData'));
	}
	$query = $query->getResultObject();

	$retVal = [];
	foreach ($query as $row)
	{
		$obj         = new \stdClass();
		$obj->name   = $row->indexname;
		$_fields     = explode(',', preg_replace('/^.*\((.+?)\)$/', '$1', trim($row->indexdef)));
		$obj->fields = array_map(function ($v) {
			return trim($v);
		}, $_fields);

		if (strpos($row->indexdef, 'CREATE UNIQUE INDEX pk') === 0)
		{
			$obj->type = 'PRIMARY';
		}
		else
		{
			$obj->type = (strpos($row->indexdef, 'CREATE UNIQUE') === 0) ? 'UNIQUE' : 'INDEX';
		}

		$retVal[$obj->name] = $obj;
	}

	return $retVal;
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
<summary><small>Source: 34 lines (399 - 432)</small></summary>

```php
public function _foreignKeyData(string $table): array
{
	$sql = 'SELECT
                           tc.constraint_name, tc.table_name, kcu.column_name,
                           ccu.table_name AS foreign_table_name,
                           ccu.column_name AS foreign_column_name
                       FROM information_schema.table_constraints AS tc
                       JOIN information_schema.key_column_usage AS kcu
                           ON tc.constraint_name = kcu.constraint_name
                       JOIN information_schema.constraint_column_usage AS ccu
                           ON ccu.constraint_name = tc.constraint_name
                       WHERE constraint_type = ' . $this->escape('FOREIGN KEY') . ' AND
                           tc.table_name = ' . $this->escape($table);

	if (($query = $this->query($sql)) === false)
	{
		throw new DatabaseException(lang('Database.failGetForeignKeyData'));
	}
	$query = $query->getResultObject();

	$retVal = [];
	foreach ($query as $row)
	{
		$obj                      = new \stdClass();
		$obj->constraint_name     = $row->constraint_name;
		$obj->table_name          = $row->table_name;
		$obj->column_name         = $row->column_name;
		$obj->foreign_table_name  = $row->foreign_table_name;
		$obj->foreign_column_name = $row->foreign_column_name;
		$retVal[]                 = $obj;
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
<summary><small>Source: 4 lines (441 - 444)</small></summary>

```php
protected function _disableForeignKeyChecks()
{
	return 'SET CONSTRAINTS ALL DEFERRED';
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
<summary><small>Source: 4 lines (453 - 456)</small></summary>

```php
protected function _enableForeignKeyChecks()
{
	return 'SET CONSTRAINTS ALL IMMEDIATE;';
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
<summary><small>Source: 7 lines (469 - 475)</small></summary>

```php
public function error(): array
{
	return [
		'code'    => '',
		'message' => pg_last_error($this->connID),
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
<summary><small>Source: 39 lines (484 - 522)</small></summary>

```php
public function insertID(): int
{
	$v = pg_version($this->connID);
	// 'server' key is only available since PostgreSQL 7.4
	$v = explode(' ', $v['server'])[0] ?? 0;

	$table  = func_num_args() > 0 ? func_get_arg(0) : null;
	$column = func_num_args() > 1 ? func_get_arg(1) : null;

	if ($table === null && $v >= '8.1')
	{
		$sql = 'SELECT LASTVAL() AS ins_id';
	}
	elseif ($table !== null)
	{
		if ($column !== null && $v >= '8.0')
		{
			$sql   = "SELECT pg_get_serial_sequence('{$table}', '{$column}') AS seq";
			$query = $this->query($sql);
			$query = $query->getRow();
			$seq   = $query->seq;
		}
		else
		{
			// seq_name passed in table parameter
			$seq = $table;
		}

		$sql = "SELECT CURRVAL('{$seq}') AS ins_id";
	}
	else
	{
		return pg_last_oid($this->resultID);
	}

	$query = $this->query($sql);
	$query = $query->getRow();
	return (int) $query->ins_id;
}
```

</details>


<hr>

#### buildDSN()

```php
protected function buildDSN()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Build a DSN from the provided parameters
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
<summary><small>Source: 44 lines (531 - 574)</small></summary>

```php
protected function buildDSN()
{
	$this->DSN === '' || $this->DSN = '';

	// If UNIX sockets are used, we shouldn't set a port
	if (strpos($this->hostname, '/') !== false)
	{
		$this->port = '';
	}

	$this->hostname === '' || $this->DSN = "host={$this->hostname} ";

	if (! empty($this->port) && ctype_digit($this->port))
	{
		$this->DSN .= "port={$this->port} ";
	}

	if ($this->username !== '')
	{
		$this->DSN .= "user={$this->username} ";

		// An empty password is valid!
		// password must be set to null to ignore it.

		$this->password === null || $this->DSN .= "password='{$this->password}' ";
	}

	$this->database === '' || $this->DSN .= "dbname={$this->database} ";

	// We don't have these options as elements in our standard configuration
	// array, but they might be set by parse_url() if the configuration was
	// provided via string> Example:
	//
	// postgre://username:password@localhost:5432/database?connect_timeout=5&sslmode=1
	foreach (['connect_timeout', 'options', 'sslmode', 'service'] as $key)
	{
		if (isset($this->{$key}) && is_string($this->{$key}) && $this->{$key} !== '')
		{
			$this->DSN .= "{$key}='{$this->{$key}}' ";
		}
	}

	$this->DSN = rtrim($this->DSN);
}
```

</details>


<hr>

#### setClientEncoding()

```php
protected function setClientEncoding(string $charset) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set client encoding
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
<td><code>$charset</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The client encoding to which the data will be converted.</td>
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
<summary><small>Source: 4 lines (584 - 587)</small></summary>

```php
protected function setClientEncoding(string $charset): bool
{
	return pg_set_client_encoding($this->connID, $charset) === 0;
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
<summary><small>Source: 4 lines (596 - 599)</small></summary>

```php
protected function _transBegin(): bool
{
	return (bool) pg_query($this->connID, 'BEGIN');
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
<summary><small>Source: 4 lines (608 - 611)</small></summary>

```php
protected function _transCommit(): bool
{
	return (bool) pg_query($this->connID, 'COMMIT');
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
<summary><small>Source: 4 lines (620 - 623)</small></summary>

```php
protected function _transRollback(): bool
{
	return (bool) pg_query($this->connID, 'ROLLBACK');
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/Connection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Builder.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Forge.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>