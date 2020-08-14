


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Database/MySQLi/Builder.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/ModelFactory.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Connection.md">next</a></td>
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
<td>framework/system/Database/MySQLi/Builder.php
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



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseBuilder.md"><strong>CodeIgniter\Database\BaseBuilder</strong></a>
</td>
<td>BaseBuilder</td>
</tr>
</table>



 
## CodeIgniter\Database\MySQLi\Builder

<table style="text-align:left">
<tr><th>Class</th><td>Builder</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Database\MySQLi\Builder</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseBuilder.md">CodeIgniter\Database\BaseBuilder</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Builder for MySQLi
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
<th><a href="#escapeChar"><strong>escapeChar</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Identifier escape character</td>
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
<th><a href="#_fromTables"><strong>_fromTables</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>FROM tables</td>
</tr>

</table>





### Properties


<hr>

#### $escapeChar

```php
protected $escapeChar = '`';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Identifier escape character
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

#### $supportedIgnoreStatements

```php
protected $supportedIgnoreStatements = [
	'update' => 'IGNORE',
	'insert' => 'IGNORE',
	'delete' => 'IGNORE',
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

#### _fromTables()

```php
protected function _fromTables() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
FROM tables
</td></tr>
</table>

<table>
<tr><td>
Groups tables in FROM clauses if needed, so there is no confusion
about operator precedence.

Note: This is only used (and overridden) by MySQL.
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
<summary><small>Source: 9 lines (79 - 87)</small></summary>

```php
protected function _fromTables(): string
{
	if (! empty($this->QBJoin) && count($this->QBFrom) > 1)
	{
		return '(' . implode(', ', $this->QBFrom) . ')';
	}

	return implode(', ', $this->QBFrom);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Database/MySQLi/Builder.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/ModelFactory.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Database/MySQLi/Connection.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>