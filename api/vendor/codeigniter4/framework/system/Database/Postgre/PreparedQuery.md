


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/PreparedQuery.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Forge.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Result.md">next</a></td>
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
<td>framework/system/Database/Postgre/PreparedQuery.php
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BasePreparedQuery.md"><strong>CodeIgniter\Database\BasePreparedQuery</strong></a>
</td>
<td>BasePreparedQuery</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/PreparedQueryInterface.md"><strong>CodeIgniter\Database\PreparedQueryInterface</strong></a>
</td>
<td>PreparedQueryInterface</td>
</tr>
</table>



 
## CodeIgniter\Database\Postgre\PreparedQuery

<table style="text-align:left">
<tr><th>Class</th><td>PreparedQuery</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\Postgre\PreparedQuery</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BasePreparedQuery.md">CodeIgniter\Database\BasePreparedQuery</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/PreparedQueryInterface.md">CodeIgniter\Database\PreparedQueryInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prepared query for Postgre
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
<th><a href="#name"><strong>name</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores the name this query can be
used under by postgres. Only used internally.</td>
</tr>
<tr>
<th><a href="#result"><strong>result</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The result resource from a successful
pg_exec. Or false.</td>
</tr>

<tr>
<th><a href="#_prepare"><strong>_prepare</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Prepares the query against the database, and saves the connection
info necessary to execute the query later.</td>
</tr>
<tr>
<th><a href="#_execute"><strong>_execute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Takes a new set of data and runs it against the currently
prepared query. Upon success, will return a Results object.</td>
</tr>
<tr>
<th><a href="#_getResult"><strong>_getResult</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the result object for the prepared query.</td>
</tr>
<tr>
<th><a href="#parameterize"><strong>parameterize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Replaces the ? placeholders with $1, $2, etc parameters for use
within the prepared query.</td>
</tr>

</table>





### Properties


<hr>

#### $name

```php
protected $name;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the name this query can be
used under by postgres. Only used internally.
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

#### $result

```php
protected $result;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The result resource from a successful
pg_exec. Or false.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>











### Methods


<hr>

#### _prepare()

```php
public function _prepare(string $sql, array $options = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prepares the query against the database, and saves the connection
info necessary to execute the query later.
</td></tr>
</table>

<table>
<tr><td>
NOTE: This version is based on SQL code. Child classes should
override this method.
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
<td><code>$options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Passed to the connection's prepare statement.
Unused in the MySQLi driver.</td>
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
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 18 lines (83 - 100)</small></summary>

```php
public function _prepare(string $sql, array $options = [])
{
	$this->name = random_int(1, 10000000000000000);

	$sql = $this->parameterize($sql);

	// Update the query object since the parameters are slightly different
	// than what was put in.
	$this->query->setQuery($sql);

	if (! $this->statement = pg_prepare($this->db->connID, $this->name, $sql))
	{
		$this->errorCode   = 0;
		$this->errorString = pg_last_error($this->db->connID);
	}

	return $this;
}
```

</details>


<hr>

#### _execute()

```php
public function _execute(array $data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes a new set of data and runs it against the currently
prepared query. Upon success, will return a Results object.
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
<summary><small>Source: 11 lines (112 - 122)</small></summary>

```php
public function _execute(array $data): bool
{
	if (is_null($this->statement))
	{
		throw new \BadMethodCallException('You must call prepare before trying to execute a prepared statement.');
	}

	$this->result = pg_execute($this->db->connID, $this->name, $data);

	return (bool) $this->result;
}
```

</details>


<hr>

#### _getResult()

```php
public function _getResult()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the result object for the prepared query.
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
<summary><small>Source: 4 lines (131 - 134)</small></summary>

```php
public function _getResult()
{
	return $this->result;
}
```

</details>


<hr>

#### parameterize()

```php
public function parameterize(string $sql) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replaces the ? placeholders with $1, $2, etc parameters for use
within the prepared query.
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (146 - 155)</small></summary>

```php
public function parameterize(string $sql): string
{
	// Track our current value
	$count = 0;

	return preg_replace_callback('/\?/', function ($matches) use (&$count) {
		$count ++;
		return "\${$count}";
	}, $sql);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/Postgre/PreparedQuery.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Forge.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/Postgre/Result.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>