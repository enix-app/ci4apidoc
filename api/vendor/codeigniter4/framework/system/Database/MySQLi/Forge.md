


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/MySQLi/Forge.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Connection.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/PreparedQuery.md">next</a></td>
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
<td>framework/system/Database/MySQLi/Forge.php
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



 

 
## CodeIgniter\Database\MySQLi\Forge

<table style="text-align:left">
<tr><th>Class</th><td>Forge</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\MySQLi\Forge</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Database\MySQLi\CodeIgniter\Database\Forge</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Forge for MySQLi
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
<th><a href="#createDatabaseStr"><strong>createDatabaseStr</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CREATE DATABASE statement</td>
</tr>
<tr>
<th><a href="#createDatabaseIfStr"><strong>createDatabaseIfStr</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CREATE DATABASE IF statement</td>
</tr>
<tr>
<th><a href="#dropConstraintStr"><strong>dropConstraintStr</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>DROP CONSTRAINT statement</td>
</tr>
<tr>
<th><a href="#createTableKeys"><strong>createTableKeys</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CREATE TABLE keys flag</td>
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
<th><a href="#_quoted_table_options"><strong>_quoted_table_options</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Table Options list which required to be quoted</td>
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
<th><a href="#_createTableAttributes"><strong>_createTableAttributes</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>CREATE TABLE attributes</td>
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

</table>





### Properties


<hr>

#### $createDatabaseStr

```php
protected $createDatabaseStr = 'CREATE DATABASE %s CHARACTER SET %s COLLATE %s';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CREATE DATABASE statement
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

#### $createDatabaseIfStr

```php
protected $createDatabaseIfStr = 'CREATE DATABASE IF NOT EXISTS %s CHARACTER SET %s COLLATE %s';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CREATE DATABASE IF statement
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

#### $dropConstraintStr

```php
protected $dropConstraintStr = 'ALTER TABLE %s DROP FOREIGN KEY %s';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
DROP CONSTRAINT statement
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

#### $createTableKeys

```php
protected $createTableKeys = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CREATE TABLE keys flag
</td></tr>
</table>

<table>
<tr><td>
Whether table keys are created from within the
CREATE TABLE statement.
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

#### $_unsigned

```php
protected $_unsigned = [
	'TINYINT',
	'SMALLINT',
	'MEDIUMINT',
	'INT',
	'INTEGER',
	'BIGINT',
	'REAL',
	'DOUBLE',
	'DOUBLE PRECISION',
	'FLOAT',
	'DECIMAL',
	'NUMERIC',
];
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
<td>array
</td>
</tr>
</table>


<hr>

#### $_quoted_table_options

```php
protected $_quoted_table_options = [
	'COMMENT',
	'COMPRESSION',
	'CONNECTION',
	'DATA DIRECTORY',
	'INDEX DIRECTORY',
	'ENCRYPTION',
	'PASSWORD',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Table Options list which required to be quoted
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

#### _createTableAttributes()

```php
protected function _createTableAttributes(array $attributes) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CREATE TABLE attributes
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
<td><code>$attributes</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Associative array of table attributes</td>
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
<summary><small>Source: 33 lines (129 - 161)</small></summary>

```php
protected function _createTableAttributes(array $attributes): string
{
	$sql = '';

	foreach (array_keys($attributes) as $key)
	{
		if (is_string($key))
		{
			$sql .= ' ' . strtoupper($key) . ' = ';

			if (in_array(strtoupper($key), $this->_quoted_table_options))
			{
				$sql .= $this->db->escape($attributes[$key]);
			}
			else
			{
				$sql .= $this->db->escapeString($attributes[$key]);
			}
		}
	}

	if (! empty($this->db->charset) && ! strpos($sql, 'CHARACTER SET') && ! strpos($sql, 'CHARSET'))
	{
		$sql .= ' DEFAULT CHARACTER SET = ' . $this->db->escapeString($this->db->charset);
	}

	if (! empty($this->db->DBCollat) && ! strpos($sql, 'COLLATE'))
	{
		$sql .= ' COLLATE = ' . $this->db->escapeString($this->db->DBCollat);
	}

	return $sql;
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
<td>string<br>string[]
</td>
</tr>
</table>





<details>
<summary><small>Source: 31 lines (173 - 203)</small></summary>

```php
protected function _alterTable(string $alter_type, string $table, $field)
{
	if ($alter_type === 'DROP')
	{
		return parent::_alterTable($alter_type, $table, $field);
	}

	$sql = 'ALTER TABLE ' . $this->db->escapeIdentifiers($table);
	foreach ($field as $i => $data)
	{
		if ($data['_literal'] !== false)
		{
			$field[$i] = ($alter_type === 'ADD') ? "\n\tADD " . $data['_literal'] : "\n\tMODIFY " . $data['_literal'];
		}
		else
		{
			if ($alter_type === 'ADD')
			{
				$field[$i]['_literal'] = "\n\tADD ";
			}
			else
			{
				$field[$i]['_literal'] = empty($data['new_name']) ? "\n\tMODIFY " : "\n\tCHANGE ";
			}

			$field[$i] = $field[$i]['_literal'] . $this->_processColumn($field[$i]);
		}
	}

	return [$sql . implode(',', $field)];
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
<summary><small>Source: 20 lines (213 - 232)</small></summary>

```php
protected function _processColumn(array $field): string
{
	$extra_clause = isset($field['after']) ? ' AFTER ' . $this->db->escapeIdentifiers($field['after']) : '';

	if (empty($extra_clause) && isset($field['first']) && $field['first'] === true)
	{
		$extra_clause = ' FIRST';
	}

	return $this->db->escapeIdentifiers($field['name'])
			. (empty($field['new_name']) ? '' : ' ' . $this->db->escapeIdentifiers($field['new_name']))
			. ' ' . $field['type'] . $field['length']
			. $field['unsigned']
			. $field['null']
			. $field['default']
			. $field['auto_increment']
			. $field['unique']
			. (empty($field['comment']) ? '' : ' COMMENT ' . $field['comment'])
			. $extra_clause;
}
```

</details>


<hr>

#### _processIndexes()

```php
protected function _processIndexes(string $table) : string
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
<td>(ignored)</td>
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
<summary><small>Source: 35 lines (242 - 276)</small></summary>

```php
protected function _processIndexes(string $table): string
{
	$sql = '';

	for ($i = 0, $c = count($this->keys); $i < $c; $i ++)
	{
		if (is_array($this->keys[$i]))
		{
			for ($i2 = 0, $c2 = count($this->keys[$i]); $i2 < $c2; $i2 ++)
			{
				if (! isset($this->fields[$this->keys[$i][$i2]]))
				{
					unset($this->keys[$i][$i2]);
					continue;
				}
			}
		}
		elseif (! isset($this->fields[$this->keys[$i]]))
		{
			unset($this->keys[$i]);
			continue;
		}

		is_array($this->keys[$i]) || $this->keys[$i] = [$this->keys[$i]];

		$unique = in_array($i, $this->uniqueKeys) ? 'UNIQUE ' : '';

		$sql .= ",\n\t{$unique}KEY " . $this->db->escapeIdentifiers(implode('_', $this->keys[$i]))
			. ' (' . implode(', ', $this->db->escapeIdentifiers($this->keys[$i])) . ')';
	}

	$this->keys = [];

	return $sql;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/MySQLi/Forge.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Connection.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/PreparedQuery.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>