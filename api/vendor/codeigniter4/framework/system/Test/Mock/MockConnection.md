


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockConnection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCodeIgniter.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockEmail.md">next</a></td>
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/CodeIgniter.md"><strong>CodeIgniter\CodeIgniter</strong></a>
</td>
<td>CodeIgniter</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseConnection.md"><strong>CodeIgniter\Database\BaseConnection</strong></a>
</td>
<td>BaseConnection</td>
</tr>
</table>



 
## CodeIgniter\Test\Mock\MockConnection

<table style="text-align:left">
<tr><th>Class</th><td>MockConnection</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Test\Mock\MockConnection</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseConnection.md">CodeIgniter\Database\BaseConnection</a></td></tr>
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
<th><a href="#returnValues"><strong>returnValues</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#database"><strong>database</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#lastQuery"><strong>lastQuery</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td></td>
</tr>

<tr>
<th><a href="#shouldReturn"><strong>shouldReturn</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#query"><strong>query</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Orchestrates a query against the database. Queries must use
Database\Statement objects to store the query and build it.</td>
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
protected

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
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#_indexData"><strong>_indexData</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#_foreignKeyData"><strong>_foreignKeyData</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#_close"><strong>_close</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Close the connection.</td>
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

#### $returnValues

```php
protected $returnValues = [];
```






<hr>

#### $database

```php
public $database;
```






<hr>

#### $lastQuery

```php
public $lastQuery;
```











### Methods


<hr>

#### shouldReturn()

```php
public function shouldReturn(string $method, $return)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td><code>$method</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$return</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 6 lines (16 - 21)</small></summary>

```php
public function shouldReturn(string $method, $return)
{
	$this->returnValues[$method] = $return;

	return $this;
}
```

</details>


<hr>

#### query()

```php
public function query(string $sql, $binds = null, bool $setEscapeFlags = true, string $queryClass = 'CodeIgniter\\Database\\Query')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Orchestrates a query against the database. Queries must use
Database\Statement objects to store the query and build it.
</td></tr>
</table>

<table>
<tr><td>
This method works with the cache.

Should automatically handle different connections for read/write
queries if needed.
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

<tr>
<td>2.</td>
<td><code>$binds</code></td>
<td><em>mixed
</em></td>
<td>true</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$setEscapeFlags</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$queryClass</code></td>
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
<td>\CodeIgniter\Database\BaseResult<br>\CodeIgniter\Database\Query<br>false
</td>
</tr>
</table>





<details>
<summary><small>Source: 33 lines (41 - 73)</small></summary>

```php
public function query(string $sql, $binds = null, bool $setEscapeFlags = true, string $queryClass = 'CodeIgniter\\Database\\Query')
{
	$queryClass = str_replace('Connection', 'Query', get_class($this));

	$query = new $queryClass($this);

	$query->setQuery($sql, $binds, $setEscapeFlags);

	if (! empty($this->swapPre) && ! empty($this->DBPrefix))
	{
		$query->swapPrefix($this->DBPrefix, $this->swapPre);
	}

	$startTime = microtime(true);

	$this->lastQuery = $query;

	// Run the query
	if (false === ($this->resultID = $this->simpleQuery($query->getQuery())))
	{
		$query->setDuration($startTime, $startTime);

		// @todo deal with errors

		return false;
	}

	$query->setDuration($startTime);

	$resultClass = str_replace('Connection', 'Result', get_class($this));

	return new $resultClass($this->connID, $this->resultID);
}
```

</details>


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
<summary><small>Source: 13 lines (84 - 96)</small></summary>

```php
public function connect(bool $persistent = false)
{
	$return = $this->returnValues['connect'] ?? true;

	if (is_array($return))
	{
		// By removing the top item here, we can
		// get a different value for, say, testing failover connections.
		$return = array_shift($this->returnValues['connect']);
	}

	return $return;
}
```

</details>


<hr>

#### reconnect()

```php
public function reconnect() : bool
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (106 - 109)</small></summary>

```php
public function reconnect(): bool
{
	return true;
}
```

</details>


<hr>

#### setDatabase()

```php
public function setDatabase(string $databaseName)
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (120 - 125)</small></summary>

```php
public function setDatabase(string $databaseName)
{
	$this->database = $databaseName;

	return $this;
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
<summary><small>Source: 4 lines (134 - 137)</small></summary>

```php
public function getVersion(): string
{
	return CodeIgniter::CI_VERSION;
}
```

</details>


<hr>

#### execute()

```php
protected function execute(string $sql)
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
<summary><small>Source: 4 lines (148 - 151)</small></summary>

```php
protected function execute(string $sql)
{
	return $this->returnValues['execute'];
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
<summary><small>Source: 4 lines (160 - 163)</small></summary>

```php
public function affectedRows(): int
{
	return 1;
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
<summary><small>Source: 7 lines (176 - 182)</small></summary>

```php
public function error(): array
{
	return [
		'code'    => null,
		'message' => null,
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
<summary><small>Source: 4 lines (191 - 194)</small></summary>

```php
public function insertID(): int
{
	return $this->connID->insert_id;
}
```

</details>


<hr>

#### _listTables()

```php
protected function _listTables(bool $constrainByPrefix = false) : string
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
<td><code>$constrainByPrefix</code></td>
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
<summary><small>Source: 4 lines (205 - 208)</small></summary>

```php
protected function _listTables(bool $constrainByPrefix = false): string
{
	return '';
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
<summary><small>Source: 4 lines (219 - 222)</small></summary>

```php
protected function _listColumns(string $table = ''): string
{
	return '';
}
```

</details>


<hr>

#### _fieldData()

```php
protected function _fieldData(string $table) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (228 - 231)</small></summary>

```php
protected function _fieldData(string $table): array
{
	return [];
}
```

</details>


<hr>

#### _indexData()

```php
protected function _indexData(string $table) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (237 - 240)</small></summary>

```php
protected function _indexData(string $table): array
{
	return [];
}
```

</details>


<hr>

#### _foreignKeyData()

```php
protected function _foreignKeyData(string $table) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (246 - 249)</small></summary>

```php
protected function _foreignKeyData(string $table): array
{
	return [];
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
Close the connection.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 3 lines (256 - 258)</small></summary>

```php
protected function _close()
{
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
<summary><small>Source: 4 lines (267 - 270)</small></summary>

```php
protected function _transBegin(): bool
{
	return true;
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
<summary><small>Source: 4 lines (279 - 282)</small></summary>

```php
protected function _transCommit(): bool
{
	return true;
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
<summary><small>Source: 4 lines (291 - 294)</small></summary>

```php
protected function _transRollback(): bool
{
	return true;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockConnection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCodeIgniter.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockEmail.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>