


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/Builder.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Utils.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Connection.md">next</a></td>
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
<td>framework/system/Database/Postgre/Builder.php
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseBuilder.md"><strong>CodeIgniter\Database\BaseBuilder</strong></a>
</td>
<td>BaseBuilder</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DatabaseException.md"><strong>CodeIgniter\Database\Exceptions\DatabaseException</strong></a>
</td>
<td>DatabaseException</td>
</tr>
</table>



 
## CodeIgniter\Database\Postgre\Builder

<table style="text-align:left">
<tr><th>Class</th><td>Builder</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\Postgre\Builder</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseBuilder.md">CodeIgniter\Database\BaseBuilder</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Builder for Postgre
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
<th><a href="#randomKeyword"><strong>randomKeyword</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>ORDER BY random keyword</td>
</tr>
<tr>
<th><a href="#supportedIgnoreStatements"><strong>supportedIgnoreStatements</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Specifies which sql statements
support the ignore option.</td>
</tr>

<tr>
<th><a href="#compileIgnore"><strong>compileIgnore</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Compile Ignore Statement</td>
</tr>
<tr>
<th><a href="#orderBy"><strong>orderBy</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>ORDER BY</td>
</tr>
<tr>
<th><a href="#increment"><strong>increment</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Increments a numeric column by the specified value.</td>
</tr>
<tr>
<th><a href="#decrement"><strong>decrement</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Decrements a numeric column by the specified value.</td>
</tr>
<tr>
<th><a href="#replace"><strong>replace</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Replace</td>
</tr>
<tr>
<th><a href="#delete"><strong>delete</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Delete</td>
</tr>
<tr>
<th><a href="#_limit"><strong>_limit</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>LIMIT string</td>
</tr>
<tr>
<th><a href="#_update"><strong>_update</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Update statement</td>
</tr>
<tr>
<th><a href="#_updateBatch"><strong>_updateBatch</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Update_Batch statement</td>
</tr>
<tr>
<th><a href="#_delete"><strong>_delete</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Delete statement</td>
</tr>
<tr>
<th><a href="#_truncate"><strong>_truncate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Truncate statement</td>
</tr>
<tr>
<th><a href="#_like_statement"><strong>_like_statement</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Platform independent LIKE statement builder.</td>
</tr>
<tr>
<th><a href="#join"><strong>join</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>JOIN</td>
</tr>

</table>





### Properties


<hr>

#### $randomKeyword

```php
protected $randomKeyword = [
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


<hr>

#### $supportedIgnoreStatements

```php
protected $supportedIgnoreStatements = [
	'insert' => 'ON CONFLICT DO NOTHING',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies which sql statements
support the ignore option.
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

#### compileIgnore()

```php
protected function compileIgnore(string $statement)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Compile Ignore Statement
</td></tr>
</table>

<table>
<tr><td>
Checks if the ignore option is supported by
the Database Driver for the specific statement.
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
<td><code>$statement</code></td>
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
<summary><small>Source: 11 lines (81 - 91)</small></summary>

```php
protected function compileIgnore(string $statement)
{
	$sql = parent::compileIgnore($statement);

	if (! empty($sql))
	{
		$sql = ' ' . trim($sql);
	}

	return $sql;
}
```

</details>


<hr>

#### orderBy()

```php
public function orderBy(string $orderBy, string $direction = '', bool $escape = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
ORDER BY
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
<td><code>$orderBy</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$direction</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>ASC, DESC or RANDOM</td>
</tr>

<tr>
<td>3.</td>
<td><code>$escape</code></td>
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
<td>\BaseBuilder
</td>
</tr>
</table>





<details>
<summary><small>Source: 22 lines (104 - 125)</small></summary>

```php
public function orderBy(string $orderBy, string $direction = '', bool $escape = null)
{
	$direction = strtoupper(trim($direction));
	if ($direction === 'RANDOM')
	{
		if (! is_float($orderBy) && ctype_digit((string) $orderBy))
		{
			$orderBy = (float) ($orderBy > 1 ? "0.{$orderBy}" : $orderBy);
		}

		if (is_float($orderBy))
		{
			$this->db->simpleQuery("SET SEED {$orderBy}");
		}

		$orderBy   = $this->randomKeyword[0];
		$direction = '';
		$escape    = false;
	}

	return parent::orderBy($orderBy, $direction, $escape);
}
```

</details>


<hr>

#### increment()

```php
public function increment(string $column, int $value = 1)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Increments a numeric column by the specified value.
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

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>int
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
<td>\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 8 lines (139 - 146)</small></summary>

```php
public function increment(string $column, int $value = 1)
{
	$column = $this->db->protectIdentifiers($column);

	$sql = $this->_update($this->QBFrom[0], [$column => "to_number({$column}, '9999999') + {$value}"]);

	return $this->db->query($sql, $this->binds, false);
}
```

</details>


<hr>

#### decrement()

```php
public function decrement(string $column, int $value = 1)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Decrements a numeric column by the specified value.
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

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>int
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
<td>\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 8 lines (160 - 167)</small></summary>

```php
public function decrement(string $column, int $value = 1)
{
	$column = $this->db->protectIdentifiers($column);

	$sql = $this->_update($this->QBFrom[0], [$column => "to_number({$column}, '9999999') - {$value}"]);

	return $this->db->query($sql, $this->binds, false);
}
```

</details>


<hr>

#### replace()

```php
public function replace(array $set = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replace
</td></tr>
</table>

<table>
<tr><td>
Compiles an replace into string and runs the query.
Because PostgreSQL doesn't support the replace into command,
we simply do a DELETE and an INSERT on the first key/value
combo, assuming that it's either the primary key or a unique key.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>internal</th>
<td>param true $bool returns the generated SQL, false executes the query.
</td>
</tr>
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
<td><code>$set</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>An associative array of insert values</td>
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
<td>\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 49 lines (185 - 233)</small></summary>

```php
public function replace(array $set = null)
{
	if ($set !== null)
	{
		$this->set($set);
	}

	if (! $this->QBSet)
	{
		if (CI_DEBUG)
		{
			throw new DatabaseException('You must use the "set" method to update an entry.');
		}
		// @codeCoverageIgnoreStart
		return false;
		// @codeCoverageIgnoreEnd
	}

	$table = $this->QBFrom[0];

	$set = $this->binds;

	// We need to grab out the actual values from
	// the way binds are stored with escape flag.
	array_walk($set, function (&$item) {
		$item = $item[0];
	});

	$keys   = array_keys($set);
	$values = array_values($set);

	$builder = $this->db->table($table);
	$exists  = $builder->where("$keys[0] = $values[0]", null, false)->get()->getFirstRow();

	if (empty($exists))
	{
		$result = $builder->insert($set);
	}
	else
	{
		array_pop($set);
		$result = $builder->update($set, "$keys[0] = $values[0]");
	}

	unset($builder);
	$this->resetWrite();

	return $result;
}
```

</details>


<hr>

#### delete()

```php
public function delete($where = '', int $limit = null, bool $reset_data = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Delete
</td></tr>
</table>

<table>
<tr><td>
Compiles a delete string and runs the query
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>internal</th>
<td>param the $mixed where clause
</td>
</tr>
<tr style="vertical-align:top;">
<th>internal</th>
<td>param the $mixed limit clause
</td>
</tr>
<tr style="vertical-align:top;">
<th>internal</th>
<td>param $bool
</td>
</tr>
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
<td><code>$where</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$limit</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$reset_data</code></td>
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
<td>\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 9 lines (252 - 260)</small></summary>

```php
public function delete($where = '', int $limit = null, bool $reset_data = true)
{
	if (! empty($limit) || ! empty($this->QBLimit))
	{
		throw new DatabaseException('PostgreSQL does not allow LIMITs on DELETE queries.');
	}

	return parent::delete($where, $limit, $reset_data);
}
```

</details>


<hr>

#### _limit()

```php
protected function _limit(string $sql, bool $offsetIgnore = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
LIMIT string
</td></tr>
</table>

<table>
<tr><td>
Generates a platform-specific LIMIT clause.
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
<td>SQL Query</td>
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
<summary><small>Source: 4 lines (273 - 276)</small></summary>

```php
protected function _limit(string $sql, bool $offsetIgnore = false): string
{
	return $sql . ' LIMIT ' . $this->QBLimit . ($this->QBOffset ? " OFFSET {$this->QBOffset}" : '');
}
```

</details>


<hr>

#### _update()

```php
protected function _update(string $table, array $values) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Update statement
</td></tr>
</table>

<table>
<tr><td>
Generates a platform-specific update string from the supplied data
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>internal</th>
<td>param the $string table name
</td>
</tr>
<tr style="vertical-align:top;">
<th>internal</th>
<td>param the $array update data
</td>
</tr>
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

<tr>
<td>2.</td>
<td><code>$values</code></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 10 lines (293 - 302)</small></summary>

```php
protected function _update(string $table, array $values): string
{
	if (! empty($this->QBLimit))
	{
		throw new DatabaseException('Postgres does not support LIMITs with UPDATE queries.');
	}

	$this->QBOrderBy = [];
	return parent::_update($table, $values);
}
```

</details>


<hr>

#### _updateBatch()

```php
protected function _updateBatch(string $table, array $values, string $index) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Update_Batch statement
</td></tr>
</table>

<table>
<tr><td>
Generates a platform-specific batch update string from the supplied data
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
<td><code>$values</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Update data</td>
</tr>

<tr>
<td>3.</td>
<td><code>$index</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>WHERE key</td>
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
<summary><small>Source: 28 lines (317 - 344)</small></summary>

```php
protected function _updateBatch(string $table, array $values, string $index): string
{
	$ids = [];
	foreach ($values as $val)
	{
		$ids[] = $val[$index];

		foreach (array_keys($val) as $field)
		{
			if ($field !== $index)
			{
				$final[$field][] = "WHEN {$val[$index]} THEN {$val[$field]}";
			}
		}
	}

	$cases = '';
	foreach ($final as $k => $v)
	{
		$cases .= "{$k} = (CASE {$index}\n"
				. implode("\n", $v)
				. "\nELSE {$k} END), ";
	}

	$this->where("{$index} IN(" . implode(',', $ids) . ')', null, false);

	return "UPDATE {$table} SET " . substr($cases, 0, -2) . $this->compileWhereHaving('QBWhere');
}
```

</details>


<hr>

#### _delete()

```php
protected function _delete(string $table) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Delete statement
</td></tr>
</table>

<table>
<tr><td>
Generates a platform-specific delete string from the supplied data
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
<td>The table name</td>
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
<summary><small>Source: 5 lines (357 - 361)</small></summary>

```php
protected function _delete(string $table): string
{
	$this->QBLimit = false;
	return parent::_delete($table);
}
```

</details>


<hr>

#### _truncate()

```php
protected function _truncate(string $table) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Truncate statement
</td></tr>
</table>

<table>
<tr><td>
Generates a platform-specific truncate string from the supplied data

If the database does not support the truncate() command,
then this method maps to 'DELETE FROM table'
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
<td>The table name</td>
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
<summary><small>Source: 4 lines (377 - 380)</small></summary>

```php
protected function _truncate(string $table): string
{
	return 'TRUNCATE ' . $table . ' RESTART IDENTITY';
}
```

</details>


<hr>

#### _like_statement()

```php
public function _like_statement(string $prefix = null, string $column, string $not = null, string $bind, bool $insensitiveSearch = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Platform independent LIKE statement builder.
</td></tr>
</table>

<table>
<tr><td>
In PostgreSQL, the ILIKE operator will perform case insensitive
searches according to the current locale.
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
<td><code>$prefix</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$column</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$not</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$bind</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$insensitiveSearch</code></td>
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
<summary><small>Source: 6 lines (400 - 405)</small></summary>

```php
public function _like_statement(string $prefix = null, string $column, string $not = null, string $bind, bool $insensitiveSearch = false): string
{
	$op = $insensitiveSearch === true ? 'ILIKE' : 'LIKE';

	return "{$prefix} {$column} {$not} {$op} :{$bind}:";
}
```

</details>


<hr>

#### join()

```php
public function join(string $table, string $cond, string $type = '', bool $escape = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
JOIN
</td></tr>
</table>

<table>
<tr><td>
Generates the JOIN portion of the query
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

<tr>
<td>2.</td>
<td><code>$cond</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The join condition</td>
</tr>

<tr>
<td>3.</td>
<td><code>$type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The type of join</td>
</tr>

<tr>
<td>4.</td>
<td><code>$escape</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether not to try to escape identifiers</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BaseBuilder
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (421 - 429)</small></summary>

```php
public function join(string $table, string $cond, string $type = '', bool $escape = null)
{
	if (! in_array('FULL OUTER', $this->joinTypes, true))
	{
		$this->joinTypes = array_merge($this->joinTypes, ['FULL OUTER']);
	}

	return parent::join($table, $cond, $type, $escape);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/Builder.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Utils.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Connection.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>