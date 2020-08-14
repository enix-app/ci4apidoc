


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/SQLite3/Result.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/PreparedQuery.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Table.md">next</a></td>
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
<td>framework/system/Database/SQLite3/Result.php
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseResult.md"><strong>CodeIgniter\Database\BaseResult</strong></a>
</td>
<td>BaseResult</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DatabaseException.md"><strong>CodeIgniter\Database\Exceptions\DatabaseException</strong></a>
</td>
<td>DatabaseException</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/ResultInterface.md"><strong>CodeIgniter\Database\ResultInterface</strong></a>
</td>
<td>ResultInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Entity.md"><strong>CodeIgniter\Entity</strong></a>
</td>
<td>Entity</td>
</tr>
</table>



 
## CodeIgniter\Database\SQLite3\Result

<table style="text-align:left">
<tr><th>Class</th><td>Result</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\SQLite3\Result</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseResult.md">CodeIgniter\Database\BaseResult</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/ResultInterface.md">CodeIgniter\Database\ResultInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Result for SQLite3
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
<th><a href="#getFieldCount"><strong>getFieldCount</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Gets the number of fields in the result set.</td>
</tr>
<tr>
<th><a href="#getFieldNames"><strong>getFieldNames</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Generates an array of column names in the result set.</td>
</tr>
<tr>
<th><a href="#getFieldData"><strong>getFieldData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Generates an array of objects representing field meta-data.</td>
</tr>
<tr>
<th><a href="#freeResult"><strong>freeResult</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Frees the current result.</td>
</tr>
<tr>
<th><a href="#dataSeek"><strong>dataSeek</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Moves the internal pointer to the desired offset. This is called
internally before fetching results to make sure the result set
starts at zero.</td>
</tr>
<tr>
<th><a href="#fetchAssoc"><strong>fetchAssoc</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Returns the result set as an array.</td>
</tr>
<tr>
<th><a href="#fetchObject"><strong>fetchObject</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Returns the result set as an object.</td>
</tr>

</table>






### Methods


<hr>

#### getFieldCount()

```php
public function getFieldCount() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets the number of fields in the result set.
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
<summary><small>Source: 4 lines (57 - 60)</small></summary>

```php
public function getFieldCount(): int
{
	return $this->resultID->numColumns();
}
```

</details>


<hr>

#### getFieldNames()

```php
public function getFieldNames() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates an array of column names in the result set.
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
<summary><small>Source: 10 lines (69 - 78)</small></summary>

```php
public function getFieldNames(): array
{
	$fieldNames = [];
	for ($i = 0, $c = $this->getFieldCount(); $i < $c; $i ++)
	{
		$fieldNames[] = $this->resultID->columnName($i);
	}

	return $fieldNames;
}
```

</details>


<hr>

#### getFieldData()

```php
public function getFieldData() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates an array of objects representing field meta-data.
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
<summary><small>Source: 27 lines (87 - 113)</small></summary>

```php
public function getFieldData(): array
{
	static $data_types = [
		SQLITE3_INTEGER => 'integer',
		SQLITE3_FLOAT   => 'float',
		SQLITE3_TEXT    => 'text',
		SQLITE3_BLOB    => 'blob',
		SQLITE3_NULL    => 'null',
	];

	$retVal = [];
	$this->resultID->fetchArray(SQLITE3_NUM);

	for ($i = 0, $c = $this->getFieldCount(); $i < $c; $i ++)
	{
		$retVal[$i]             = new \stdClass();
		$retVal[$i]->name       = $this->resultID->columnName($i);
		$type                   = $this->resultID->columnType($i);
		$retVal[$i]->type       = $type;
		$retVal[$i]->type_name  = isset($data_types[$type]) ? $data_types[$type] : null;
		$retVal[$i]->max_length = null;
		$retVal[$i]->length     = null;
	}
	$this->resultID->reset();

	return $retVal;
}
```

</details>


<hr>

#### freeResult()

```php
public function freeResult()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Frees the current result.
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
<summary><small>Source: 8 lines (122 - 129)</small></summary>

```php
public function freeResult()
{
	if (is_object($this->resultID))
	{
		$this->resultID->finalize();
		$this->resultID = false;
	}
}
```

</details>


<hr>

#### dataSeek()

```php
public function dataSeek(int $n = 0)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Moves the internal pointer to the desired offset. This is called
internally before fetching results to make sure the result set
starts at zero.
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
<td><code>$n</code></td>
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
<td>\CodeIgniter\Database\Exceptions\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 9 lines (143 - 151)</small></summary>

```php
public function dataSeek(int $n = 0)
{
	if ($n !== 0)
	{
		throw new DatabaseException('SQLite3 doesn\'t support seeking to other offset.');
	}

	return $this->resultID->reset();
}
```

</details>


<hr>

#### fetchAssoc()

```php
protected function fetchAssoc()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the result set as an array.
</td></tr>
</table>

<table>
<tr><td>
Overridden by driver classes.
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
<summary><small>Source: 4 lines (162 - 165)</small></summary>

```php
protected function fetchAssoc()
{
	return $this->resultID->fetchArray(SQLITE3_ASSOC);
}
```

</details>


<hr>

#### fetchObject()

```php
protected function fetchObject(string $className = 'stdClass')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the result set as an object.
</td></tr>
</table>

<table>
<tr><td>
Overridden by child classes.
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
<td><code>$className</code></td>
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
<td>object<br>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 29 lines (178 - 206)</small></summary>

```php
protected function fetchObject(string $className = 'stdClass')
{
	// No native support for fetching rows as objects
	if (($row = $this->fetchAssoc()) === false)
	{
		return false;
	}
	elseif ($className === 'stdClass')
	{
		return (object) $row;
	}

	$classObj = new $className();

	if (is_subclass_of($className, Entity::class))
	{
		return $classObj->setAttributes($row);
	}

	$classSet = \Closure::bind(function ($key, $value) {
		$this->$key = $value;
	}, $classObj, $className
	);
	foreach (array_keys($row) as $key)
	{
		$classSet($key, $row[$key]);
	}
	return $classObj;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/SQLite3/Result.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/PreparedQuery.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/SQLite3/Table.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>