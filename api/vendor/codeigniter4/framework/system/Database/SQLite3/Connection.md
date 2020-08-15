


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/SQLite3/Connection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Builder.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Forge.md">next</a></td>
</tr>
</table>







# CodeIgniter\Database\SQLite3 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Database\SQLite3</td></tr>
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
<td>framework/system/Database/SQLite3/Connection.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Builder.md">CodeIgniter\Database\SQLite3\Builder</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Connection.md">CodeIgniter\Database\SQLite3\Connection</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Forge.md">CodeIgniter\Database\SQLite3\Forge</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/PreparedQuery.md">CodeIgniter\Database\SQLite3\PreparedQuery</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Result.md">CodeIgniter\Database\SQLite3\Result</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Table.md">CodeIgniter\Database\SQLite3\Table</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Utils.md">CodeIgniter\Database\SQLite3\Utils</a></td></tr>
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



 
## CodeIgniter\Database\SQLite3\Connection

<table style="text-align:left">
<tr><th>Class</th><td>Connection</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\SQLite3\Connection</td></tr>
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
Connection for SQLite3
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
<th><a href="#escapeChar"><strong>escapeChar</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Identifier escape character</td>
</tr>
<tr>
<th><a href="#_random_keyword"><strong>_random_keyword</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>ORDER BY random keyword</td>
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
<td>Execute the query</td>
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
<th><a href="#getFieldNames"><strong>getFieldNames</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Fetch Field Names</td>
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
<tr>
<th><a href="#isWriteType"><strong>isWriteType</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines if the statement is a write-type query or not.</td>
</tr>
<tr>
<th><a href="#supportsForeignKeys"><strong>supportsForeignKeys</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if the current install supports Foreign Keys
and has them enabled.</td>
</tr>

</table>





### Properties


<hr>

#### $DBDriver

```php
public $DBDriver = 'SQLite3';
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

#### $_random_keyword

```php
protected $_random_keyword = [
	'RANDOM()',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
ORDER BY random keyword
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
<summary><small>Source: 22 lines (87 - 108)</small></summary>

```php
public function connect(bool $persistent = false)
{
	if ($persistent && $this->db->DBDebug)
	{
		throw new DatabaseException('SQLite3 doesn\'t support persistent connections.');
	}
	try
	{
		if ($this->database !== ':memory:' && strpos($this->database, DIRECTORY_SEPARATOR) === false)
		{
			$this->database = WRITEPATH . $this->database;
		}

		return (! $this->password)
			? new \SQLite3($this->database)
			: new \SQLite3($this->database, SQLITE3_OPEN_READWRITE | SQLITE3_OPEN_CREATE, $this->password);
	}
	catch (\Exception $e)
	{
		throw new DatabaseException('SQLite3 error: ' . $e->getMessage());
	}
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
<summary><small>Source: 5 lines (118 - 122)</small></summary>

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
<summary><small>Source: 4 lines (131 - 134)</small></summary>

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
<summary><small>Source: 4 lines (145 - 148)</small></summary>

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
<summary><small>Source: 11 lines (157 - 167)</small></summary>

```php
public function getVersion(): string
{
	if (isset($this->dataCache['version']))
	{
		return $this->dataCache['version'];
	}

	$version = \SQLite3::version();

	return $this->dataCache['version'] = $version['versionString'];
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
Execute the query
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
<summary><small>Source: 18 lines (178 - 195)</small></summary>

```php
public function execute(string $sql)
{
	try
	{
		return $this->isWriteType($sql)
			? $this->connID->exec($sql)
			: $this->connID->query($sql);
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
<summary><small>Source: 4 lines (204 - 207)</small></summary>

```php
public function affectedRows(): int
{
	return $this->connID->changes();
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
<summary><small>Source: 4 lines (218 - 221)</small></summary>

```php
protected function _escapeString(string $str): string
{
	return $this->connID->escapeString($str);
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
<summary><small>Source: 9 lines (232 - 240)</small></summary>

```php
protected function _listTables(bool $prefixLimit = false): string
{
	return 'SELECT "NAME" FROM "SQLITE_MASTER" WHERE "TYPE" = \'table\''
		   . ' AND "NAME" NOT LIKE \'sqlite!_%\' ESCAPE \'!\''
		   . (($prefixLimit !== false && $this->DBPrefix !== '')
			? ' AND "NAME" LIKE \'' . $this->escapeLikeString($this->DBPrefix) . '%\' ' . sprintf($this->likeEscapeStr,
				$this->likeEscapeChar)
			: '');
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
<summary><small>Source: 4 lines (251 - 254)</small></summary>

```php
protected function _listColumns(string $table = ''): string
{
	return 'PRAGMA TABLE_INFO(' . $this->protectIdentifiers($table, true, null, false) . ')';
}
```

</details>


<hr>

#### getFieldNames()

```php
public function getFieldNames(string $table)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetch Field Names
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
<td>Table name</td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 55 lines (264 - 318)</small></summary>

```php
public function getFieldNames(string $table)
{
	// Is there a cached result?
	if (isset($this->dataCache['field_names'][$table]))
	{
		return $this->dataCache['field_names'][$table];
	}

	if (empty($this->connID))
	{
		$this->initialize();
	}

	if (false === ($sql = $this->_listColumns($table)))
	{
		if ($this->DBDebug)
		{
			throw new DatabaseException(lang('Database.featureUnavailable'));
		}

		return false;
	}

	$query                                  = $this->query($sql);
	$this->dataCache['field_names'][$table] = [];

	foreach ($query->getResultArray() as $row)
	{
		// Do we know from where to get the column's name?
		if (! isset($key))
		{
			if (isset($row['column_name']))
			{
				$key = 'column_name';
			}
			elseif (isset($row['COLUMN_NAME']))
			{
				$key = 'COLUMN_NAME';
			}
			elseif (isset($row['name']))
			{
				$key = 'name';
			}
			else
			{
				// We have no other choice but to just get the first element's key.
				$key = key($row);
			}
		}

		$this->dataCache['field_names'][$table][] = $row[$key];
	}

	return $this->dataCache['field_names'][$table];
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
<summary><small>Source: 27 lines (329 - 355)</small></summary>

```php
public function _fieldData(string $table): array
{
	if (($query = $this->query('PRAGMA TABLE_INFO(' . $this->protectIdentifiers($table, true, null,
				false) . ')')) === false)
	{
		throw new DatabaseException(lang('Database.failGetFieldData'));
	}
	$query = $query->getResultObject();

	if (empty($query))
	{
		return [];
	}
	$retVal = [];
	for ($i = 0, $c = count($query); $i < $c; $i++)
	{
		$retVal[$i]              = new \stdClass();
		$retVal[$i]->name        = $query[$i]->name;
		$retVal[$i]->type        = $query[$i]->type;
		$retVal[$i]->max_length  = null;
		$retVal[$i]->default     = $query[$i]->dflt_value;
		$retVal[$i]->primary_key = isset($query[$i]->pk) && (bool)$query[$i]->pk;
		$retVal[$i]->nullable    = isset($query[$i]->notnull) && ! (bool)$query[$i]->notnull;
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
<summary><small>Source: 35 lines (366 - 400)</small></summary>

```php
public function _indexData(string $table): array
{
	// Get indexes
	// Don't use PRAGMA index_list, so we can preserve index order
	$sql = "SELECT name FROM sqlite_master WHERE type='index' AND tbl_name=" . $this->escape(strtolower($table));
	if (($query = $this->query($sql)) === false)
	{
		throw new DatabaseException(lang('Database.failGetIndexData'));
	}
	$query = $query->getResultObject();

	$retVal = [];
	foreach ($query as $row)
	{
		$obj       = new \stdClass();
		$obj->name = $row->name;

		// Get fields for index
		$obj->fields = [];
		if (($fields = $this->query('PRAGMA index_info(' . $this->escape(strtolower($row->name)) . ')')) === false)
		{
			throw new DatabaseException(lang('Database.failGetIndexData'));
		}
		$fields = $fields->getResultObject();

		foreach ($fields as $field)
		{
			$obj->fields[] = $field->name;
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





<details>
<summary><small>Source: 34 lines (410 - 443)</small></summary>

```php
public function _foreignKeyData(string $table): array
{
	if ($this->supportsForeignKeys() !== true)
	{
		return [];
	}

	$tables = $this->listTables();

	if (empty($tables))
	{
		return [];
	}

	$retVal = [];

	foreach ($tables as $table)
	{
		$query = $this->query("PRAGMA foreign_key_list({$table})")->getResult();

		foreach ($query as $row)
		{
			$obj                     = new \stdClass();
			$obj->constraint_name    = $row->from . ' to ' . $row->table . '.' . $row->to;
			$obj->table_name         = $table;
			$obj->foreign_table_name = $row->table;
			$obj->sequence           = $row->seq;

			$retVal[] = $obj;
		}
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
<summary><small>Source: 4 lines (452 - 455)</small></summary>

```php
protected function _disableForeignKeyChecks()
{
	return 'PRAGMA foreign_keys = OFF';
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
<summary><small>Source: 4 lines (464 - 467)</small></summary>

```php
protected function _enableForeignKeyChecks()
{
	return 'PRAGMA foreign_keys = ON';
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
<summary><small>Source: 7 lines (480 - 486)</small></summary>

```php
public function error(): array
{
	return [
		'code'    => $this->connID->lastErrorCode(),
		'message' => $this->connID->lastErrorMsg(),
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
<summary><small>Source: 4 lines (495 - 498)</small></summary>

```php
public function insertID(): int
{
	return $this->connID->lastInsertRowID();
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
<summary><small>Source: 4 lines (507 - 510)</small></summary>

```php
protected function _transBegin(): bool
{
	return $this->connID->exec('BEGIN TRANSACTION');
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
<summary><small>Source: 4 lines (519 - 522)</small></summary>

```php
protected function _transCommit(): bool
{
	return $this->connID->exec('END TRANSACTION');
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
<summary><small>Source: 4 lines (531 - 534)</small></summary>

```php
protected function _transRollback(): bool
{
	return $this->connID->exec('ROLLBACK');
}
```

</details>


<hr>

#### isWriteType()

```php
public function isWriteType($sql) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines if the statement is a write-type query or not.
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
<summary><small>Source: 6 lines (543 - 548)</small></summary>

```php
public function isWriteType($sql): bool
{
	return (bool)preg_match(
		'/^\s*"?(SET|INSERT|UPDATE|DELETE|REPLACE|CREATE|DROP|TRUNCATE|LOAD|COPY|ALTER|RENAME|GRANT|REVOKE|LOCK|UNLOCK|REINDEX)\s/i',
		$sql);
}
```

</details>


<hr>

#### supportsForeignKeys()

```php
public function supportsForeignKeys() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if the current install supports Foreign Keys
and has them enabled.
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
<summary><small>Source: 6 lines (558 - 563)</small></summary>

```php
public function supportsForeignKeys(): bool
{
	$result = $this->simpleQuery('PRAGMA foreign_keys');

	return (bool)$result;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/SQLite3/Connection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Builder.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Forge.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>