


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/Forge.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Connection.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/PreparedQuery.md">next</a></td>
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
<td>framework/system/Database/Postgre/Forge.php
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



 

 
## CodeIgniter\Database\Postgre\Forge

<table style="text-align:left">
<tr><th>Class</th><td>Forge</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\Postgre\Forge</td></tr>
<tr><th>Extends</th><td><a href="">CodeIgniter\Database\Postgre\CodeIgniter\Database\Forge</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Forge for Postgre
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
<th><a href="#checkDatabaseExistStr"><strong>checkDatabaseExistStr</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CHECK DATABASE EXIST statement</td>
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
<th><a href="#_dropTable"><strong>_dropTable</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Drop Table</td>
</tr>

</table>





### Properties


<hr>

#### $checkDatabaseExistStr

```php
protected $checkDatabaseExistStr = 'SELECT 1 FROM pg_database WHERE datname = ?';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CHECK DATABASE EXIST statement
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
protected $dropConstraintStr = 'ALTER TABLE %s DROP CONSTRAINT %s';
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

#### $_unsigned

```php
protected $_unsigned = [
	'INT2'     => 'INTEGER',
	'SMALLINT' => 'INTEGER',
	'INT'      => 'BIGINT',
	'INT4'     => 'BIGINT',
	'INTEGER'  => 'BIGINT',
	'INT8'     => 'NUMERIC',
	'BIGINT'   => 'NUMERIC',
	'REAL'     => 'DOUBLE PRECISION',
	'FLOAT'    => 'DOUBLE PRECISION',
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
<summary><small>Source: 4 lines (94 - 97)</small></summary>

```php
protected function _createTableAttributes(array $attributes): string
{
	return '';
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
<summary><small>Source: 50 lines (110 - 159)</small></summary>

```php
protected function _alterTable(string $alter_type, string $table, $field)
{
	if (in_array($alter_type, ['DROP', 'ADD'], true))
	{
		return parent::_alterTable($alter_type, $table, $field);
	}

	$sql  = 'ALTER TABLE ' . $this->db->escapeIdentifiers($table);
	$sqls = [];
	foreach ($field as $data)
	{
		if ($data['_literal'] !== false)
		{
			return false;
		}

		if (version_compare($this->db->getVersion(), '8', '>=') && isset($data['type']))
		{
			$sqls[] = $sql . ' ALTER COLUMN ' . $this->db->escapeIdentifiers($data['name'])
					. " TYPE {$data['type']}{$data['length']}";
		}

		if (! empty($data['default']))
		{
			$sqls[] = $sql . ' ALTER COLUMN ' . $this->db->escapeIdentifiers($data['name'])
					. " SET DEFAULT {$data['default']}";
		}

		if (isset($data['null']))
		{
			$sqls[] = $sql . ' ALTER COLUMN ' . $this->db->escapeIdentifiers($data['name'])
					. ($data['null'] === true ? ' DROP' : ' SET') . ' NOT NULL';
		}

		if (! empty($data['new_name']))
		{
			$sqls[] = $sql . ' RENAME COLUMN ' . $this->db->escapeIdentifiers($data['name'])
					. ' TO ' . $this->db->escapeIdentifiers($data['new_name']);
		}

		if (! empty($data['comment']))
		{
			$sqls[] = 'COMMENT ON COLUMN' . $this->db->escapeIdentifiers($table)
					. '.' . $this->db->escapeIdentifiers($data['name'])
					. " IS {$data['comment']}";
		}
	}

	return $sqls;
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
<summary><small>Source: 9 lines (169 - 177)</small></summary>

```php
protected function _processColumn(array $field): string
{
	return $this->db->escapeIdentifiers($field['name'])
			. ' ' . $field['type'] . $field['length']
			. $field['default']
			. $field['null']
			. $field['auto_increment']
			. $field['unique'];
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
<summary><small>Source: 25 lines (190 - 214)</small></summary>

```php
protected function _attributeType(array &$attributes)
{
	// Reset field lengths for data types that don't support it
	if (isset($attributes['CONSTRAINT']) && stripos($attributes['TYPE'], 'int') !== false)
	{
		$attributes['CONSTRAINT'] = null;
	}

	switch (strtoupper($attributes['TYPE']))
	{
		case 'TINYINT':
			$attributes['TYPE']     = 'SMALLINT';
			$attributes['UNSIGNED'] = false;
			break;
		case 'MEDIUMINT':
			$attributes['TYPE']     = 'INTEGER';
			$attributes['UNSIGNED'] = false;
			break;
		case 'DATETIME':
			$attributes['TYPE'] = 'TIMESTAMP';
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
<summary><small>Source: 7 lines (226 - 232)</small></summary>

```php
protected function _attributeAutoIncrement(array &$attributes, array &$field)
{
	if (! empty($attributes['AUTO_INCREMENT']) && $attributes['AUTO_INCREMENT'] === true)
	{
		$field['type'] = $field['type'] === 'NUMERIC' || $field['type'] === 'BIGINT' ? 'BIGSERIAL' : 'SERIAL';
	}
}
```

</details>


<hr>

#### _dropTable()

```php
protected function _dropTable(string $table, bool $if_exists, bool $cascade) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Drop Table
</td></tr>
</table>

<table>
<tr><td>
Generates a platform-specific DROP TABLE string
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
<td><code>$if_exists</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to add an IF EXISTS condition</td>
</tr>

<tr>
<td>3.</td>
<td><code>$cascade</code></td>
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
<summary><small>Source: 11 lines (247 - 257)</small></summary>

```php
protected function _dropTable(string $table, bool $if_exists, bool $cascade): string
{
	$sql = parent::_dropTable($table, $if_exists, $cascade);

	if ($cascade === true)
	{
		$sql .= ' CASCADE';
	}

	return $sql;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/Forge.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Connection.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/PreparedQuery.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>