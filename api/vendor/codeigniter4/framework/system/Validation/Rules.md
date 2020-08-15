


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/Rules.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FormatRules.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md">next</a></td>
</tr>
</table>







# CodeIgniter\Validation 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Validation</td></tr>
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
<td>framework/system/Validation/Rules.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/CreditCardRules.md">CodeIgniter\Validation\CreditCardRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md">CodeIgniter\Validation\Exceptions\ValidationException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FileRules.md">CodeIgniter\Validation\FileRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FormatRules.md">CodeIgniter\Validation\FormatRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Rules.md">CodeIgniter\Validation\Rules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md">CodeIgniter\Validation\Validation</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">CodeIgniter\Validation\ValidationInterface</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>Config\Database</strong>
</td>
<td>Database</td>
</tr>
</table>



 
## CodeIgniter\Validation\Rules

<table style="text-align:left">
<tr><th>Class</th><td>Rules</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Validation\Rules</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validation Rules.
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Validation
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
<th><a href="#differs"><strong>differs</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>The value does not match another field in $data.</td>
</tr>
<tr>
<th><a href="#equals"><strong>equals</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Equals the static value provided.</td>
</tr>
<tr>
<th><a href="#exact_length"><strong>exact_length</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns true if $str is $val characters long.</td>
</tr>
<tr>
<th><a href="#greater_than"><strong>greater_than</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Greater than</td>
</tr>
<tr>
<th><a href="#greater_than_equal_to"><strong>greater_than_equal_to</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Equal to or Greater than</td>
</tr>
<tr>
<th><a href="#is_not_unique"><strong>is_not_unique</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks the database to see if the given value exist.</td>
</tr>
<tr>
<th><a href="#in_list"><strong>in_list</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Value should be within an array of values</td>
</tr>
<tr>
<th><a href="#is_unique"><strong>is_unique</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks the database to see if the given value is unique. Can
ignore a single record by field/value to make it useful during
record updates.</td>
</tr>
<tr>
<th><a href="#less_than"><strong>less_than</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Less than</td>
</tr>
<tr>
<th><a href="#less_than_equal_to"><strong>less_than_equal_to</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Equal to or Less than</td>
</tr>
<tr>
<th><a href="#matches"><strong>matches</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Matches the value of another field in $data.</td>
</tr>
<tr>
<th><a href="#max_length"><strong>max_length</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns true if $str is $val or fewer characters in length.</td>
</tr>
<tr>
<th><a href="#min_length"><strong>min_length</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns true if $str is at least $val length.</td>
</tr>
<tr>
<th><a href="#not_equals"><strong>not_equals</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Does not equal the static value provided.</td>
</tr>
<tr>
<th><a href="#required"><strong>required</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Required</td>
</tr>
<tr>
<th><a href="#required_with"><strong>required_with</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>The field is required when any of the other required fields are present
in the data.</td>
</tr>
<tr>
<th><a href="#required_without"><strong>required_without</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>The field is required when all of the other fields are present
in the data but not required.</td>
</tr>

</table>






### Methods


<hr>

#### differs()

```php
public function differs(string $str = null, string $field, array $data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The value does not match another field in $data.
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

<tr>
<td>2.</td>
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$data</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Other field/value pairs</td>
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
<summary><small>Source: 4 lines (62 - 65)</small></summary>

```php
public function differs(string $str = null, string $field, array $data): bool
{
	return array_key_exists($field, $data) && $str !== $data[$field];
}
```

</details>


<hr>

#### equals()

```php
public function equals(string $str = null, string $val) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Equals the static value provided.
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

<tr>
<td>2.</td>
<td><code>$val</code></td>
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
<summary><small>Source: 4 lines (77 - 80)</small></summary>

```php
public function equals(string $str = null, string $val): bool
{
	return $str === $val;
}
```

</details>


<hr>

#### exact_length()

```php
public function exact_length(string $str = null, string $val) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns true if $str is $val characters long.
</td></tr>
</table>

<table>
<tr><td>
$val = "5" (one) | "5,8,12" (multiple values)
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

<tr>
<td>2.</td>
<td><code>$val</code></td>
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
<summary><small>Source: 13 lines (93 - 105)</small></summary>

```php
public function exact_length(string $str = null, string $val): bool
{
	$val = explode(',', $val);
	foreach ($val as $tmp)
	{
		if (is_numeric($tmp) && (int)$tmp === mb_strlen($str))
		{
			return true;
		}
	}

	return false;
}
```

</details>


<hr>

#### greater_than()

```php
public function greater_than(string $str = null, string $min) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Greater than
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

<tr>
<td>2.</td>
<td><code>$min</code></td>
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
<summary><small>Source: 4 lines (117 - 120)</small></summary>

```php
public function greater_than(string $str = null, string $min): bool
{
	return is_numeric($str) && $str > $min;
}
```

</details>


<hr>

#### greater_than_equal_to()

```php
public function greater_than_equal_to(string $str = null, string $min) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Equal to or Greater than
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

<tr>
<td>2.</td>
<td><code>$min</code></td>
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
<summary><small>Source: 4 lines (132 - 135)</small></summary>

```php
public function greater_than_equal_to(string $str = null, string $min): bool
{
	return is_numeric($str) && $str >= $min;
}
```

</details>


<hr>

#### is_not_unique()

```php
public function is_not_unique(string $str = null, string $field, array $data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks the database to see if the given value exist.
</td></tr>
</table>

<table>
<tr><td>
Can ignore records by field/value to filter (currently
accept only one filter).

Example:
   is_not_unique[table.field,where_field,where_value]
   is_not_unique[menu.id,active,1]
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

<tr>
<td>2.</td>
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$data</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 26 lines (154 - 179)</small></summary>

```php
public function is_not_unique(string $str = null, string $field, array $data): bool
{
	// Grab any data for exclusion of a single row.
	list($field, $where_field, $where_value) = array_pad(explode(',', $field), 3, null);

	// Break the table and field apart
	sscanf($field, '%[^.].%[^.]', $table, $field);

	$db = Database::connect($data['DBGroup'] ?? null);

	$row = $db->table($table)
			  ->select('1')
			  ->where($field, $str)
			  ->limit(1);

	if (! empty($where_field) && ! empty($where_value))
	{
		if (! preg_match('/^\{(\w+)\}$/', $where_value))
		{
			$row = $row->where($where_field, $where_value);
		}
	}

	return (bool) ($row->get()
					->getRow() !== null);
}
```

</details>


<hr>

#### in_list()

```php
public function in_list(string $value = null, string $list) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Value should be within an array of values
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
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$list</code></td>
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
<summary><small>Source: 8 lines (191 - 198)</small></summary>

```php
public function in_list(string $value = null, string $list): bool
{
	$list = explode(',', $list);
	$list = array_map(function ($value) {
		return trim($value);
	}, $list);
	return in_array($value, $list, true);
}
```

</details>


<hr>

#### is_unique()

```php
public function is_unique(string $str = null, string $field, array $data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks the database to see if the given value is unique. Can
ignore a single record by field/value to make it useful during
record updates.
</td></tr>
</table>

<table>
<tr><td>
Example:
is_unique[table.field,ignore_field,ignore_value]
is_unique[users.email,id,5]
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

<tr>
<td>2.</td>
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$data</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 26 lines (217 - 242)</small></summary>

```php
public function is_unique(string $str = null, string $field, array $data): bool
{
	// Grab any data for exclusion of a single row.
	list($field, $ignoreField, $ignoreValue) = array_pad(explode(',', $field), 3, null);

	// Break the table and field apart
	sscanf($field, '%[^.].%[^.]', $table, $field);

	$db = Database::connect($data['DBGroup'] ?? null);

	$row = $db->table($table)
			  ->select('1')
			  ->where($field, $str)
			  ->limit(1);

	if (! empty($ignoreField) && ! empty($ignoreValue))
	{
		if (! preg_match('/^\{(\w+)\}$/', $ignoreValue))
		{
			$row = $row->where("{$ignoreField} !=", $ignoreValue);
		}
	}

	return (bool) ($row->get()
					->getRow() === null);
}
```

</details>


<hr>

#### less_than()

```php
public function less_than(string $str = null, string $max) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Less than
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

<tr>
<td>2.</td>
<td><code>$max</code></td>
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
<summary><small>Source: 4 lines (254 - 257)</small></summary>

```php
public function less_than(string $str = null, string $max): bool
{
	return is_numeric($str) && $str < $max;
}
```

</details>


<hr>

#### less_than_equal_to()

```php
public function less_than_equal_to(string $str = null, string $max) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Equal to or Less than
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

<tr>
<td>2.</td>
<td><code>$max</code></td>
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
<summary><small>Source: 4 lines (269 - 272)</small></summary>

```php
public function less_than_equal_to(string $str = null, string $max): bool
{
	return is_numeric($str) && $str <= $max;
}
```

</details>


<hr>

#### matches()

```php
public function matches(string $str = null, string $field, array $data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Matches the value of another field in $data.
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

<tr>
<td>2.</td>
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$data</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Other field/value pairs</td>
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
<summary><small>Source: 4 lines (285 - 288)</small></summary>

```php
public function matches(string $str = null, string $field, array $data): bool
{
	return array_key_exists($field, $data) && $str === $data[$field];
}
```

</details>


<hr>

#### max_length()

```php
public function max_length(string $str = null, string $val) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns true if $str is $val or fewer characters in length.
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

<tr>
<td>2.</td>
<td><code>$val</code></td>
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
<summary><small>Source: 4 lines (300 - 303)</small></summary>

```php
public function max_length(string $str = null, string $val): bool
{
	return ($val >= mb_strlen($str));
}
```

</details>


<hr>

#### min_length()

```php
public function min_length(string $str = null, string $val) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns true if $str is at least $val length.
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

<tr>
<td>2.</td>
<td><code>$val</code></td>
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
<summary><small>Source: 4 lines (315 - 318)</small></summary>

```php
public function min_length(string $str = null, string $val): bool
{
	return ($val <= mb_strlen($str));
}
```

</details>


<hr>

#### not_equals()

```php
public function not_equals(string $str = null, string $val) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does not equal the static value provided.
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

<tr>
<td>2.</td>
<td><code>$val</code></td>
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
<summary><small>Source: 4 lines (330 - 333)</small></summary>

```php
public function not_equals(string $str = null, string $val): bool
{
	return $str !== $val;
}
```

</details>


<hr>

#### required()

```php
public function required($str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Required
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
<td>Value</td>
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
<summary><small>Source: 9 lines (344 - 352)</small></summary>

```php
public function required($str = null): bool
{
	if (is_object($str))
	{
		return true;
	}

	return is_array($str) ? ! empty($str) : (trim($str) !== '');
}
```

</details>


<hr>

#### required_with()

```php
public function required_with($str = null, string $fields, array $data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The field is required when any of the other required fields are present
in the data.
</td></tr>
</table>

<table>
<tr><td>
Example (field is required when the password field is present):

required_with[password]
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$fields</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>List of fields that we should check if present</td>
</tr>

<tr>
<td>3.</td>
<td><code>$data</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Complete list of fields from the form</td>
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
<summary><small>Source: 35 lines (370 - 404)</small></summary>

```php
public function required_with($str = null, string $fields, array $data): bool
{
	$fields = explode(',', $fields);

	// If the field is present we can safely assume that
	// the field is here, no matter whether the corresponding
	// search field is present or not.
	$present = $this->required($str ?? '');

	if ($present)
	{
		return true;
	}

	// Still here? Then we fail this test if
	// any of the fields are present in $data
	// as $fields is the lis
	$requiredFields = [];

	foreach ($fields as $field)
	{
		if (array_key_exists($field, $data))
		{
			$requiredFields[] = $field;
		}
	}

	// Remove any keys with empty values since, that means they
	// weren't truly there, as far as this is concerned.
	$requiredFields = array_filter($requiredFields, function ($item) use ($data) {
		return ! empty($data[$item]);
	});

	return empty($requiredFields);
}
```

</details>


<hr>

#### required_without()

```php
public function required_without($str = null, string $fields, array $data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The field is required when all of the other fields are present
in the data but not required.
</td></tr>
</table>

<table>
<tr><td>
Example (field is required when the id or email field is missing):

required_without[id,email]
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$fields</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$data</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 26 lines (422 - 447)</small></summary>

```php
public function required_without($str = null, string $fields, array $data): bool
{
	$fields = explode(',', $fields);

	// If the field is present we can safely assume that
	// the field is here, no matter whether the corresponding
	// search field is present or not.
	$present = $this->required($str ?? '');

	if ($present)
	{
		return true;
	}

	// Still here? Then we fail this test if
	// any of the fields are not present in $data
	foreach ($fields as $field)
	{
		if (! array_key_exists($field, $data))
		{
			return false;
		}
	}

	return true;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/Rules.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FormatRules.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>