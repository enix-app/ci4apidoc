


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/SQLite3/Forge.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Connection.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/PreparedQuery.md">next</a></td>
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
<td>framework/system/Database/SQLite3/Forge.php
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



 
## CodeIgniter\Database\SQLite3\Forge

<table style="text-align:left">
<tr><th>Class</th><td>Forge</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\SQLite3\Forge</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Database\SQLite3\CodeIgniter\Database\Forge</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Forge for SQLite3
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
<th><a href="#_unsigned"><strong>_unsigned</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>UNSIGNED support</td>
</tr>
<tr>
<th><a href="#_null"><strong>_null</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>NULL value representation in CREATE/ALTER TABLE statements</td>
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
<th><a href="#createDatabase"><strong>createDatabase</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Create database</td>
</tr>
<tr>
<th><a href="#dropDatabase"><strong>dropDatabase</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Drop database</td>
</tr>
<tr>
<th><a href="#_alterTable"><strong>_alterTable</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>ALTER TABLE</td>
</tr>
<tr>
<th><a href="#_processColumn"><strong>_processColumn</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Process column</td>
</tr>
<tr>
<th><a href="#_processIndexes"><strong>_processIndexes</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Process indexes</td>
</tr>
<tr>
<th><a href="#_attributeType"><strong>_attributeType</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Field attribute TYPE</td>
</tr>
<tr>
<th><a href="#_attributeAutoIncrement"><strong>_attributeAutoIncrement</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Field attribute AUTO_INCREMENT</td>
</tr>
<tr>
<th><a href="#dropForeignKey"><strong>dropForeignKey</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Foreign Key Drop</td>
</tr>

</table>





### Properties


<hr>

#### $_unsigned

```php
protected $_unsigned = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
UNSIGNED support
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>bool<br>array
</td>
</tr>
</table>


<hr>

#### $_null

```php
protected $_null = 'NULL';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
NULL value representation in CREATE/ALTER TABLE statements
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
public function __construct(ConnectionInterface $db)
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
<td><code>$db</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 10 lines (72 - 81)</small></summary>

```php
public function __construct(ConnectionInterface $db)
{
	parent::__construct($db);

	if (version_compare($this->db->getVersion(), '3.3', '<'))
	{
		$this->createTableIfStr = false;
		$this->dropTableIfStr   = false;
	}
}
```

</details>


<hr>

#### createDatabase()

```php
public function createDatabase(string $dbName, bool $ifNotExists = false) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create database
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
<td><code>$dbName</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$ifNotExists</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to add IF NOT EXISTS condition</td>
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
<summary><small>Source: 6 lines (93 - 98)</small></summary>

```php
public function createDatabase(string $dbName, bool $ifNotExists = false): bool
{
	// In SQLite, a database is created when you connect to the database.
	// We'll return TRUE so that an error isn't generated.
	return true;
}
```

</details>


<hr>

#### dropDatabase()

```php
public function dropDatabase(string $dbName) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Drop database
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
<td><code>$dbName</code></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Database\Exceptions\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 36 lines (110 - 145)</small></summary>

```php
public function dropDatabase(string $dbName): bool
{
	// In SQLite, a database is dropped when we delete a file
	if (! is_file($dbName))
	{
		if ($this->db->DBDebug)
		{
			throw new DatabaseException('Unable to drop the specified database.');
		}

		return false;
	}

	// We need to close the pseudo-connection first
	$this->db->close();
	if (! @unlink($dbName))
	{
		if ($this->db->DBDebug)
		{
			throw new DatabaseException('Unable to drop the specified database.');
		}

		return false;
	}

	if (! empty($this->db->dataCache['db_names']))
	{
		$key = array_search(strtolower($dbName), array_map('strtolower', $this->db->dataCache['db_names']), true);
		if ($key !== false)
		{
			unset($this->db->dataCache['db_names'][$key]);
		}
	}

	return true;
}
```

</details>


<hr>

#### _alterTable()

```php
protected function _alterTable(string $alter_type, string $table, $field)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
ALTER TABLE
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
<td><code>$alter_type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>ALTER type</td>
</tr>

<tr>
<td>2.</td>
<td><code>$table</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Table name</td>
</tr>

<tr>
<td>3.</td>
<td><code>$field</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Column definition</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 24 lines (158 - 181)</small></summary>

```php
protected function _alterTable(string $alter_type, string $table, $field)
{
	switch ($alter_type)
	{
		case 'DROP':
			$sqlTable = new Table($this->db, $this);

			$sqlTable->fromTable($table)
				->dropColumn($field)
				->run();

			return '';
		case 'CHANGE':
			$sqlTable = new Table($this->db, $this);

			$sqlTable->fromTable($table)
					 ->modifyColumn($field)
					 ->run();

			return null;
		default:
			return parent::_alterTable($alter_type, $table, $field);
	}
}
```

</details>


<hr>

#### _processColumn()

```php
protected function _processColumn(array $field) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Process column
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
<td><code>$field</code></td>
<td><em>array
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
<summary><small>Source: 15 lines (192 - 206)</small></summary>

```php
protected function _processColumn(array $field): string
{
	if ($field['type'] === 'TEXT' && strpos($field['length'], "('") === 0)
	{
		$field['type'] .= ' CHECK(' . $this->db->escapeIdentifiers($field['name'])
			. ' IN ' . $field['length'] . ')';
	}

	return $this->db->escapeIdentifiers($field['name'])
		   . ' ' . $field['type']
		   . $field['auto_increment']
		   . $field['null']
		   . $field['unique']
		   . $field['default'];
}
```

</details>


<hr>

#### _processIndexes()

```php
protected function _processIndexes(string $table) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Process indexes
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 35 lines (217 - 251)</small></summary>

```php
protected function _processIndexes(string $table): array
{
	$sqls = [];

	for ($i = 0, $c = count($this->keys); $i < $c; $i++)
	{
		$this->keys[$i] = (array)$this->keys[$i];

		for ($i2 = 0, $c2 = count($this->keys[$i]); $i2 < $c2; $i2++)
		{
			if (! isset($this->fields[$this->keys[$i][$i2]]))
			{
				unset($this->keys[$i][$i2]);
			}
		}
		if (count($this->keys[$i]) <= 0)
		{
			continue;
		}

		if (in_array($i, $this->uniqueKeys))
		{
			$sqls[] = 'CREATE UNIQUE INDEX ' . $this->db->escapeIdentifiers($table . '_' . implode('_', $this->keys[$i]))
					  . ' ON ' . $this->db->escapeIdentifiers($table)
					  . ' (' . implode(', ', $this->db->escapeIdentifiers($this->keys[$i])) . ');';
			continue;
		}

		$sqls[] = 'CREATE INDEX ' . $this->db->escapeIdentifiers($table . '_' . implode('_', $this->keys[$i]))
				  . ' ON ' . $this->db->escapeIdentifiers($table)
				  . ' (' . implode(', ', $this->db->escapeIdentifiers($this->keys[$i])) . ');';
	}

	return $sqls;
}
```

</details>


<hr>

#### _attributeType()

```php
protected function _attributeType(array &$attributes)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Field attribute TYPE
</td></tr>
</table>

<table>
<tr><td>
Performs a data type mapping between different databases.
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
<td><code>$</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>&$attributes</td>
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
<summary><small>Source: 12 lines (263 - 274)</small></summary>

```php
protected function _attributeType(array &$attributes)
{
	switch (strtoupper($attributes['TYPE']))
	{
		case 'ENUM':
		case 'SET':
			$attributes['TYPE'] = 'TEXT';
			break;
		default:
			break;
	}
}
```

</details>


<hr>

#### _attributeAutoIncrement()

```php
protected function _attributeAutoIncrement(array &$attributes, array &$field)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Field attribute AUTO_INCREMENT
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
<td><code>$</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>&$attributes</td>
</tr>

<tr>
<td>2.</td>
<td><code>$</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>&$field</td>
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
<summary><small>Source: 14 lines (286 - 299)</small></summary>

```php
protected function _attributeAutoIncrement(array &$attributes, array &$field)
{
	if (! empty($attributes['AUTO_INCREMENT']) && $attributes['AUTO_INCREMENT'] === true
		&& stripos($field['type'], 'int') !== false)
	{
		$field['type']           = 'INTEGER PRIMARY KEY';
		$field['default']        = '';
		$field['null']           = '';
		$field['unique']         = '';
		$field['auto_increment'] = ' AUTOINCREMENT';

		$this->primaryKeys = [];
	}
}
```

</details>


<hr>

#### dropForeignKey()

```php
public function dropForeignKey(string $table, string $foreignName) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Foreign Key Drop
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

<tr>
<td>2.</td>
<td><code>$foreignName</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Foreign name</td>
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
<td>\CodeIgniter\Database\Exceptions\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 16 lines (312 - 327)</small></summary>

```php
public function dropForeignKey(string $table, string $foreignName): bool
{
	// If this version of SQLite doesn't support it, we're done here
	if ($this->db->supportsForeignKeys() !== true)
	{
		return true;
	}

	// Otherwise we have to copy the table and recreate
	// without the foreign key being involved now
	$sqlTable = new Table($this->db, $this);

	return $sqlTable->fromTable($this->db->DBPrefix . $table)
		->dropForeignKey($foreignName)
		->run();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/SQLite3/Forge.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Connection.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/PreparedQuery.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>