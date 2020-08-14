


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Interfaces/FabricatorModel.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Filters/CITestStreamFilter.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockAppConfig.md">next</a></td>
</tr>
</table>







# CodeIgniter\Test\Interfaces 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Test\Interfaces</td></tr>
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
<td>framework/system/Test/Interfaces/FabricatorModel.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Interfaces/FabricatorModel.md">CodeIgniter\Test\Interfaces\FabricatorModel</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>Faker\Generator</strong>
</td>
<td>Generator</td>
</tr>
</table>



 
## CodeIgniter\Test\Interfaces\FabricatorModel

<table style="text-align:left">
<tr><th>Interface</th><td>FabricatorModel</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Test\Interfaces\FabricatorModel</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
FabricatorModel
</td></tr>
</table>

<table>
<tr><td>
An interface defining the required methods and properties
needed for a model to qualify for use with the Fabricator class.
While interfaces cannot enforce properties, the following
are required for use with Fabricator:
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
<th><a href="#find"><strong>find</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Fetches the row of database from $this-&gt;table with a primary key
matching $id.</td>
</tr>
<tr>
<th><a href="#insert"><strong>insert</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Inserts data into the current table. If an object is provided,
it will attempt to convert it to an array.</td>
</tr>

</table>






### Methods


<hr>

#### find()

```php
public function find($id = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetches the row of database from $this->table with a primary key
matching $id.
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
<td><code>$id</code></td>
<td><em>mixed<br>array<br>null
</em></td>
<td>false</td>
<td>One primary key or an array of primary keys</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>object<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: line 65</small></summary>

```php
public function find($id = null);
```

</details>


<hr>

#### insert()

```php
public function insert($data = null, bool $returnID = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Inserts data into the current table. If an object is provided,
it will attempt to convert it to an array.
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
<td><em>array<br>object
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$returnID</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether insert ID should be returned or not.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int<br>string<br>bool
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: line 77</small></summary>

```php
public function insert($data = null, bool $returnID = true);
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Interfaces/FabricatorModel.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Filters/CITestStreamFilter.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockAppConfig.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>