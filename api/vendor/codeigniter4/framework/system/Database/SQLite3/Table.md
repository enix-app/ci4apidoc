


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/SQLite3/Table.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Result.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Utils.md">next</a></td>
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
<td>framework/system/Database/SQLite3/Table.php
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DataException.md"><strong>CodeIgniter\Database\Exceptions\DataException</strong></a>
</td>
<td>DataException</td>
</tr>
</table>



 
## CodeIgniter\Database\SQLite3\Table

<table style="text-align:left">
<tr><th>Class</th><td>Table</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\SQLite3\Table</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Table
</td></tr>
</table>

<table>
<tr><td>
Provides missing features for altering tables that are common
in other supported databases, but are missing from SQLite.
These are needed in order to support migrations during testing
when another database is used as the primary engine, but
SQLite in memory databases are used for faster test execution.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Database\SQLite3
</td>
</tr>
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
<th><a href="#fields"><strong>fields</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>All of the fields this table represents.</td>
</tr>
<tr>
<th><a href="#keys"><strong>keys</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>All of the unique/primary keys in the table.</td>
</tr>
<tr>
<th><a href="#foreignKeys"><strong>foreignKeys</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>All of the foreign keys in the table.</td>
</tr>
<tr>
<th><a href="#tableName"><strong>tableName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the table we&#039;re working with.</td>
</tr>
<tr>
<th><a href="#prefixedTableName"><strong>prefixedTableName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the table, with database prefix</td>
</tr>
<tr>
<th><a href="#db"><strong>db</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Database connection.</td>
</tr>
<tr>
<th><a href="#forge"><strong>forge</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Handle to our forge.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Table constructor.</td>
</tr>
<tr>
<th><a href="#fromTable"><strong>fromTable</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Reads an existing database table and
collects all of the information needed to
recreate this table.</td>
</tr>
<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Called after `fromTable` and any actions, like `dropColumn`, etc,
to finalize the action. It creates a temp table, creates the new
table with modifications, and copies the data over to the new table.</td>
</tr>
<tr>
<th><a href="#dropColumn"><strong>dropColumn</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Drops columns from the table.</td>
</tr>
<tr>
<th><a href="#modifyColumn"><strong>modifyColumn</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Modifies a field, including changing data type,
renaming, etc.</td>
</tr>
<tr>
<th><a href="#dropForeignKey"><strong>dropForeignKey</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Drops a foreign key from this table so that
it won&#039;t be recreated in the future.</td>
</tr>
<tr>
<th><a href="#createTable"><strong>createTable</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Creates the new table based on our current fields.</td>
</tr>
<tr>
<th><a href="#copyData"><strong>copyData</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Copies data from our old table to the new one,
taking care map data correctly based on any columns
that have been renamed.</td>
</tr>
<tr>
<th><a href="#formatFields"><strong>formatFields</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Converts fields retrieved from the database to
the format needed for creating fields with Forge.</td>
</tr>
<tr>
<th><a href="#formatKeys"><strong>formatKeys</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Converts keys retrieved from the database to
the format needed to create later.</td>
</tr>
<tr>
<th><a href="#dropIndexes"><strong>dropIndexes</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Attempts to drop all indexes and constraints
from the database for this table.</td>
</tr>

</table>





### Properties


<hr>

#### $fields

```php
protected $fields = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
All of the fields this table represents.
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


<hr>

#### $keys

```php
protected $keys = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
All of the unique/primary keys in the table.
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


<hr>

#### $foreignKeys

```php
protected $foreignKeys = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
All of the foreign keys in the table.
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


<hr>

#### $tableName

```php
protected $tableName;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the table we're working with.
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

#### $prefixedTableName

```php
protected $prefixedTableName;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the table, with database prefix
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
Database connection.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Connection
</td>
</tr>
</table>


<hr>

#### $forge

```php
protected $forge;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handle to our forge.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Forge
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(Connection $db, Forge $forge)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Table constructor.
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
<td><em>\Connection
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$forge</code></td>
<td><em>\Forge
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 5 lines (111 - 115)</small></summary>

```php
public function __construct(Connection $db, Forge $forge)
{
	$this->db    = $db;
	$this->forge = $forge;
}
```

</details>


<hr>

#### fromTable()

```php
public function fromTable(string $table)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reads an existing database table and
collects all of the information needed to
recreate this table.
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
<td>\CodeIgniter\Database\SQLite3\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 30 lines (126 - 155)</small></summary>

```php
public function fromTable(string $table)
{
	$this->prefixedTableName = $table;

	// Remove the prefix, if any, since it's
	// already been added by the time we get here...
	$prefix = $this->db->DBPrefix;
	if (! empty($prefix))
	{
		if (strpos($table, $prefix) === 0)
		{
			$table = substr($table, strlen($prefix));
		}
	}

	if (! $this->db->tableExists($this->prefixedTableName))
	{
		throw DataException::forTableNotFound($this->prefixedTableName);
	}

	$this->tableName = $table;

	$this->fields = $this->formatFields($this->db->getFieldData($table));

	$this->keys = array_merge($this->keys, $this->formatKeys($this->db->getIndexData($table)));

	$this->foreignKeys = $this->db->getForeignKeyData($table);

	return $this;
}
```

</details>


<hr>

#### run()

```php
public function run() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Called after `fromTable` and any actions, like `dropColumn`, etc,
to finalize the action. It creates a temp table, creates the new
table with modifications, and copies the data over to the new table.
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
<summary><small>Source: 22 lines (164 - 185)</small></summary>

```php
public function run(): bool
{
	$this->db->query('PRAGMA foreign_keys = OFF');

	$this->db->transStart();

	$this->forge->renameTable($this->tableName, "temp_{$this->tableName}");

	$this->forge->reset();

	$this->createTable();

	$this->copyData();

	$this->forge->dropTable("temp_{$this->tableName}");

	$success = $this->db->transComplete();

	$this->db->query('PRAGMA foreign_keys = ON');

	return $success;
}
```

</details>


<hr>

#### dropColumn()

```php
public function dropColumn($columns)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Drops columns from the table.
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
<td><code>$columns</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Database\SQLite3\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 20 lines (194 - 213)</small></summary>

```php
public function dropColumn($columns)
{
	//unset($this->fields[$column]);

	if (is_string($columns))
	{
		$columns = explode(',', $columns);
	}

	foreach ($columns as $column)
	{
		$column = trim($column);
		if (isset($this->fields[$column]))
		{
			unset($this->fields[$column]);
		}
	}

	return $this;
}
```

</details>


<hr>

#### modifyColumn()

```php
public function modifyColumn(array $field)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Modifies a field, including changing data type,
renaming, etc.
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
<td>\CodeIgniter\Database\SQLite3\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (223 - 233)</small></summary>

```php
public function modifyColumn(array $field)
{
	$field = $field[0];

	$oldName = $field['name'];
	unset($field['name']);

	$this->fields[$oldName] = $field;

	return $this;
}
```

</details>


<hr>

#### dropForeignKey()

```php
public function dropForeignKey(string $column)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Drops a foreign key from this table so that
it won't be recreated in the future.
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
<td><code>$column</code></td>
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
<td>\CodeIgniter\Database\SQLite3\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 25 lines (243 - 267)</small></summary>

```php
public function dropForeignKey(string $column)
{
	if (empty($this->foreignKeys))
	{
		return $this;
	}

	for ($i = 0; $i < count($this->foreignKeys); $i++)
	{
		if ($this->foreignKeys[$i]->table_name !== $this->tableName)
		{
			continue;
		}

		// The column name should be the first thing in the constraint name
		if (strpos($this->foreignKeys[$i]->constraint_name, $column) !== 0)
		{
			continue;
		}

		unset($this->foreignKeys[$i]);
	}

	return $this;
}
```

</details>


<hr>

#### createTable()

```php
protected function createTable()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Creates the new table based on our current fields.
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
<summary><small>Source: 44 lines (274 - 317)</small></summary>

```php
protected function createTable()
{
	$this->dropIndexes();
	$this->db->resetDataCache();

	// Handle any modified columns.
	$fields = [];
	foreach ($this->fields as $name => $field)
	{
		if (isset($field['new_name']))
		{
			$fields[$field['new_name']] = $field;
			continue;
		}

		$fields[$name] = $field;
	}

	$this->forge->addField($fields);

	// Unique/Index keys
	if (is_array($this->keys))
	{
		foreach ($this->keys as $key)
		{
			switch ($key['type'])
			{
				case 'primary':
					$this->forge->addPrimaryKey($key['fields']);
					break;
				case 'unique':
					$this->forge->addUniqueKey($key['fields']);
					break;
				case 'index':
					$this->forge->addKey($key['fields']);
					break;
			}
		}
	}

	// Foreign Keys

	return $this->forge->createTable($this->tableName);
}
```

</details>


<hr>

#### copyData()

```php
protected function copyData()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Copies data from our old table to the new one,
taking care map data correctly based on any columns
that have been renamed.
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
<summary><small>Source: 25 lines (326 - 350)</small></summary>

```php
protected function copyData()
{
	$exFields  = [];
	$newFields = [];

	foreach ($this->fields as $name => $details)
	{
		// Are we modifying the column?
		if (isset($details['new_name']))
		{
			$newFields[] = $details['new_name'];
		}
		else
		{
			$newFields[] = $name;
		}

		$exFields[] = $name;
	}

	$exFields  = implode(', ', $exFields);
	$newFields = implode(', ', $newFields);

	$this->db->query("INSERT INTO {$this->prefixedTableName}({$newFields}) SELECT {$exFields} FROM {$this->db->DBPrefix}temp_{$this->tableName}");
}
```

</details>


<hr>

#### formatFields()

```php
protected function formatFields($fields)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts fields retrieved from the database to
the format needed for creating fields with Forge.
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
<td><code>$fields</code></td>
<td><em>array<br>bool
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
<summary><small>Source: 28 lines (360 - 387)</small></summary>

```php
protected function formatFields($fields)
{
	if (! is_array($fields))
	{
		return $fields;
	}

	$return = [];

	foreach ($fields as $field)
	{
		$return[$field->name] = [
			'type'     => $field->type,
			'default'  => $field->default,
			'nullable' => $field->nullable,
		];

		if ($field->primary_key)
		{
			$this->keys[$field->name] = [
				'fields' => [$field->name],
				'type'   => 'primary',
			];
		}
	}

	return $return;
}
```

</details>


<hr>

#### formatKeys()

```php
protected function formatKeys($keys)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts keys retrieved from the database to
the format needed to create later.
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
<td><code>$keys</code></td>
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
<summary><small>Source: 19 lines (397 - 415)</small></summary>

```php
protected function formatKeys($keys)
{
	if (! is_array($keys))
	{
		return $keys;
	}

	$return = [];

	foreach ($keys as $name => $key)
	{
		$return[$name] = [
			'fields' => $key->fields,
			'type'   => 'index',
		];
	}

	return $return;
}
```

</details>


<hr>

#### dropIndexes()

```php
protected function dropIndexes()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to drop all indexes and constraints
from the database for this table.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>null<br>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 17 lines (423 - 439)</small></summary>

```php
protected function dropIndexes()
{
	if (! is_array($this->keys) || ! count($this->keys))
	{
		return;
	}

	foreach ($this->keys as $name => $key)
	{
		if ($key['type'] === 'primary' || $key['type'] === 'unique')
		{
			continue;
		}

		$this->db->query("DROP INDEX IF EXISTS '{$name}'");
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/SQLite3/Table.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Result.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Utils.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>