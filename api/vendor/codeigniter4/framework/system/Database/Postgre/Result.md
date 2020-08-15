


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/Result.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/PreparedQuery.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Utils.md">next</a></td>
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
<td>framework/system/Database/Postgre/Result.php
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseResult.md"><strong>CodeIgniter\Database\BaseResult</strong></a>
</td>
<td>BaseResult</td>
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



 
## CodeIgniter\Database\Postgre\Result

<table style="text-align:left">
<tr><th>Class</th><td>Result</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\Postgre\Result</td></tr>
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
Result for Postgre
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
	return pg_num_fields($this->resultID);
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
		$fieldNames[] = pg_field_name($this->resultID, $i);
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
<summary><small>Source: 18 lines (87 - 104)</small></summary>

```php
public function getFieldData(): array
{
	$retVal = [];

	for ($i = 0, $c = $this->getFieldCount(); $i < $c; $i ++)
	{
		$retVal[$i]             = new \stdClass();
		$retVal[$i]->name       = pg_field_name($this->resultID, $i);
		$retVal[$i]->type       = pg_field_type_oid($this->resultID, $i);
		$retVal[$i]->type_name  = pg_field_type($this->resultID, $i);
		$retVal[$i]->max_length = pg_field_size($this->resultID, $i);
		$retVal[$i]->length     = $retVal[$i]->max_length;
		// $retVal[$i]->primary_key = (int)($fieldData[$i]->flags & 2);
		// $retVal[$i]->default     = $fieldData[$i]->def;
	}

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
<summary><small>Source: 8 lines (113 - 120)</small></summary>

```php
public function freeResult()
{
	if (is_resource($this->resultID))
	{
		pg_free_result($this->resultID);
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





<details>
<summary><small>Source: 4 lines (133 - 136)</small></summary>

```php
public function dataSeek(int $n = 0)
{
	return pg_result_seek($this->resultID, $n);
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
<summary><small>Source: 4 lines (147 - 150)</small></summary>

```php
protected function fetchAssoc()
{
	return pg_fetch_assoc($this->resultID);
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
<td>object<br>bool<br>\Entity
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (163 - 170)</small></summary>

```php
protected function fetchObject(string $className = 'stdClass')
{
	if (is_subclass_of($className, Entity::class))
	{
		return empty($data = $this->fetchAssoc()) ? false : (new $className())->setAttributes($data);
	}
	return pg_fetch_object($this->resultID, null, $className);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/Result.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/PreparedQuery.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Utils.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>