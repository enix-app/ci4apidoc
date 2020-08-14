


 



<table>
<tr>
<td style="width:100%"><em>framework/system/View/Table.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/View.md">next</a></td>
</tr>
</table>







# CodeIgniter\View 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\View</td></tr>
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

Copyright (c) 2014 - 2019, British Columbia Institute of Technology
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
<td>EllisLab Dev Team
</td>
</tr>
<tr style="vertical-align:top;">
<th>copyright</th>
<td>Copyright (c) 2008 - 2014, EllisLab, Inc. (<a href="https://ellislab.com">https://ellislab.com</a>/)
</td>
</tr>
<tr style="vertical-align:top;">
<th>copyright</th>
<td>Copyright (c) 2014 - 2019, British Columbia Institute of Technology (<a href="https://bcit.ca">https://bcit.ca</a>/)
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
<td>framework/system/View/Table.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Cell.md">CodeIgniter\View\Cell</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md">CodeIgniter\View\Exceptions\ViewException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Filters.md">CodeIgniter\View\Filters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Parser.md">CodeIgniter\View\Parser</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Plugins.md">CodeIgniter\View\Plugins</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">CodeIgniter\View\RendererInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Table.md">CodeIgniter\View\Table</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/View.md">CodeIgniter\View\View</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Database/BaseResult.md"><strong>CodeIgniter\Database\BaseResult</strong></a>
</td>
<td>BaseResult</td>
</tr>
</table>



 
## CodeIgniter\View\Table

<table style="text-align:left">
<tr><th>Class</th><td>Table</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\View\Table</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
HTML Table Generating Class
</td></tr>
</table>

<table>
<tr><td>
Lets you create tables manually or from database result objects, or arrays.
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
<th>subpackage</th>
<td>Libraries
</td>
</tr>
<tr style="vertical-align:top;">
<th>category</th>
<td>HTML Tables
</td>
</tr>
<tr style="vertical-align:top;">
<th>author</th>
<td>EllisLab Dev Team
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
<th><a href="#rows"><strong>rows</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Data for table rows</td>
</tr>
<tr>
<th><a href="#heading"><strong>heading</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Data for table heading</td>
</tr>
<tr>
<th><a href="#footing"><strong>footing</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Data for table footing</td>
</tr>
<tr>
<th><a href="#autoHeading"><strong>autoHeading</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Whether or not to automatically create the table header</td>
</tr>
<tr>
<th><a href="#caption"><strong>caption</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Table caption</td>
</tr>
<tr>
<th><a href="#template"><strong>template</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Table layout template</td>
</tr>
<tr>
<th><a href="#newline"><strong>newline</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Newline setting</td>
</tr>
<tr>
<th><a href="#emptyCells"><strong>emptyCells</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Contents of empty cells</td>
</tr>
<tr>
<th><a href="#function"><strong>function</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Callback for custom table layout</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set the template from the table config file if it exists</td>
</tr>
<tr>
<th><a href="#setTemplate"><strong>setTemplate</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set the template</td>
</tr>
<tr>
<th><a href="#setHeading"><strong>setHeading</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set the table heading</td>
</tr>
<tr>
<th><a href="#setFooting"><strong>setFooting</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set the table footing</td>
</tr>
<tr>
<th><a href="#makeColumns"><strong>makeColumns</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set columns. Takes a one-dimensional array as input and creates
a multi-dimensional array with a depth equal to the number of
columns. This allows a single array with many elements to be
displayed in a table that has a fixed column count.</td>
</tr>
<tr>
<th><a href="#setEmpty"><strong>setEmpty</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set &quot;empty&quot; cells</td>
</tr>
<tr>
<th><a href="#addRow"><strong>addRow</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Add a table row</td>
</tr>
<tr>
<th><a href="#_prepArgs"><strong>_prepArgs</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Prep Args</td>
</tr>
<tr>
<th><a href="#setCaption"><strong>setCaption</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Add a table caption</td>
</tr>
<tr>
<th><a href="#generate"><strong>generate</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Generate the table</td>
</tr>
<tr>
<th><a href="#clear"><strong>clear</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Clears the table arrays.  Useful if multiple tables are being generated</td>
</tr>
<tr>
<th><a href="#_setFromDBResult"><strong>_setFromDBResult</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Set table data from a database result object</td>
</tr>
<tr>
<th><a href="#_setFromArray"><strong>_setFromArray</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Set table data from an array</td>
</tr>
<tr>
<th><a href="#_compileTemplate"><strong>_compileTemplate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Compile Template</td>
</tr>
<tr>
<th><a href="#_defaultTemplate"><strong>_defaultTemplate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Default Template</td>
</tr>

</table>





### Properties


<hr>

#### $rows

```php
public $rows = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Data for table rows
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

#### $heading

```php
public $heading = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Data for table heading
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

#### $footing

```php
public $footing = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Data for table footing
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

#### $autoHeading

```php
public $autoHeading = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether or not to automatically create the table header
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

#### $caption

```php
public $caption;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Table caption
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

#### $template

```php
public $template;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Table layout template
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

#### $newline

```php
public $newline = "\n";
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Newline setting
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

#### $emptyCells

```php
public $emptyCells = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Contents of empty cells
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

#### $function

```php
public $function;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callback for custom table layout
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\function
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct($config = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the template from the table config file if it exists
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
<td><code>$config</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>(default: array())</td>
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
<summary><small>Source: 8 lines (126 - 133)</small></summary>

```php
public function __construct($config = [])
{
	// initialize config
	foreach ($config as $key => $val)
	{
		$this->template[$key] = $val;
	}
}
```

</details>


<hr>

#### setTemplate()

```php
public function setTemplate($template)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the template
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
<td><code>$template</code></td>
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
<summary><small>Source: 10 lines (143 - 152)</small></summary>

```php
public function setTemplate($template)
{
	if (! is_array($template))
	{
		return false;
	}

	$this->template = $template;
	return true;
}
```

</details>


<hr>

#### setHeading()

```php
public function setHeading()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the table heading
</td></tr>
</table>

<table>
<tr><td>
Can be passed as an array or discreet params
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (163 - 167)</small></summary>

```php
public function setHeading()
{
	$this->heading = $this->_prepArgs(func_get_args());
	return $this;
}
```

</details>


<hr>

#### setFooting()

```php
public function setFooting()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the table footing
</td></tr>
</table>

<table>
<tr><td>
Can be passed as an array or discreet params
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (176 - 180)</small></summary>

```php
public function setFooting()
{
	$this->footing = $this->_prepArgs(func_get_args());
	return $this;
}
```

</details>


<hr>

#### makeColumns()

```php
public function makeColumns($array = array(), $columnLimit = 0)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set columns. Takes a one-dimensional array as input and creates
a multi-dimensional array with a depth equal to the number of
columns. This allows a single array with many elements to be
displayed in a table that has a fixed column count.
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
<td><code>$array</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$columnLimit</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 35 lines (194 - 228)</small></summary>

```php
public function makeColumns($array = [], $columnLimit = 0)
{
	if (! is_array($array) || count($array) === 0 || ! is_int($columnLimit))
	{
		return false;
	}

	// Turn off the auto-heading feature since it's doubtful we
	// will want headings from a one-dimensional array
	$this->autoHeading = false;

	if ($columnLimit === 0)
	{
		return $array;
	}

	$new = [];
	do
	{
		$temp = array_splice($array, 0, $columnLimit);

		if (count($temp) < $columnLimit)
		{
			for ($i = count($temp); $i < $columnLimit; $i ++)
			{
				$temp[] = '&nbsp;';
			}
		}

		$new[] = $temp;
	}
	while (count($array) > 0);

	return $new;
}
```

</details>


<hr>

#### setEmpty()

```php
public function setEmpty($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set "empty" cells
</td></tr>
</table>

<table>
<tr><td>
Can be passed as an array or discreet params
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
<td>\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (240 - 244)</small></summary>

```php
public function setEmpty($value)
{
	$this->emptyCells = $value;
	return $this;
}
```

</details>


<hr>

#### addRow()

```php
public function addRow()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add a table row
</td></tr>
</table>

<table>
<tr><td>
Can be passed as an array or discreet params
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (255 - 259)</small></summary>

```php
public function addRow()
{
	$this->rows[] = $this->_prepArgs(func_get_args());
	return $this;
}
```

</details>


<hr>

#### _prepArgs()

```php
protected function _prepArgs($args)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prep Args
</td></tr>
</table>

<table>
<tr><td>
Ensures a standard associative array format for all cell data
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
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 17 lines (271 - 287)</small></summary>

```php
protected function _prepArgs($args)
{
	// If there is no $args[0], skip this and treat as an associative array
	// This can happen if there is only a single key, for example this is passed to table->generate
	// array(array('foo'=>'bar'))
	if (isset($args[0]) && count($args) === 1 && is_array($args[0]) && ! isset($args[0]['data']))
	{
		$args = $args[0];
	}

	foreach ($args as $key => $val)
	{
		is_array($val) || $args[$key] = ['data' => $val];
	}

	return $args;
}
```

</details>


<hr>

#### setCaption()

```php
public function setCaption($caption)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add a table caption
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
<td><code>$caption</code></td>
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
<td>\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (297 - 301)</small></summary>

```php
public function setCaption($caption)
{
	$this->caption = $caption;
	return $this;
}
```

</details>


<hr>

#### generate()

```php
public function generate($tableData = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generate the table
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
<td><code>$tableData</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 145 lines (311 - 455)</small></summary>

```php
public function generate($tableData = null)
{
	// The table data can optionally be passed to this function
	// either as a database result object or an array
	if (! empty($tableData))
	{
		if ($tableData instanceof BaseResult)
		{
			$this->_setFromDBResult($tableData);
		}
		elseif (is_array($tableData))
		{
			$this->_setFromArray($tableData);
		}
	}

	// Is there anything to display? No? Smite them!
	if (empty($this->heading) && empty($this->rows))
	{
		return 'Undefined table data';
	}

	// Compile and validate the template date
	$this->_compileTemplate();

	// Validate a possibly existing custom cell manipulation function
	if (isset($this->function) && ! is_callable($this->function))
	{
		$this->function = null;
	}

	// Build the table!

	$out = $this->template['table_open'] . $this->newline;

	// Add any caption here
	if ($this->caption)
	{
		$out .= '<caption>' . $this->caption . '</caption>' . $this->newline;
	}

	// Is there a table heading to display?
	if (! empty($this->heading))
	{
		$out .= $this->template['thead_open'] . $this->newline . $this->template['heading_row_start'] . $this->newline;

		foreach ($this->heading as $heading)
		{
			$temp = $this->template['heading_cell_start'];

			foreach ($heading as $key => $val)
			{
				if ($key !== 'data')
				{
					$temp = str_replace('<th', '<th ' . $key . '="' . $val . '"', $temp);
				}
			}

			$out .= $temp . (isset($heading['data']) ? $heading['data'] : '') . $this->template['heading_cell_end'];
		}

		$out .= $this->template['heading_row_end'] . $this->newline . $this->template['thead_close'] . $this->newline;
	}

	// Build the table rows
	if (! empty($this->rows))
	{
		$out .= $this->template['tbody_open'] . $this->newline;

		$i = 1;
		foreach ($this->rows as $row)
		{
			// We use modulus to alternate the row colors
			$name = fmod($i ++, 2) ? '' : 'alt_';

			$out .= $this->template['row_' . $name . 'start'] . $this->newline;

			foreach ($row as $cell)
			{
				$temp = $this->template['cell_' . $name . 'start'];

				foreach ($cell as $key => $val)
				{
					if ($key !== 'data')
					{
						$temp = str_replace('<td', '<td ' . $key . '="' . $val . '"', $temp);
					}
				}

				$cell = isset($cell['data']) ? $cell['data'] : '';
				$out .= $temp;

				if ($cell === '' || $cell === null)
				{
					$out .= $this->emptyCells;
				}
				elseif (isset($this->function))
				{
					$out .= call_user_func($this->function, $cell);
				}
				else
				{
					$out .= $cell;
				}

				$out .= $this->template['cell_' . $name . 'end'];
			}

			$out .= $this->template['row_' . $name . 'end'] . $this->newline;
		}
	}

	// Any table footing to display?
	if (! empty($this->footing))
	{
		$out .= $this->template['tfoot_open'] . $this->newline . $this->template['footing_row_start'] . $this->newline;

		foreach ($this->footing as $footing)
		{
			$temp = $this->template['footing_cell_start'];

			foreach ($footing as $key => $val)
			{
				if ($key !== 'data')
				{
					$temp = str_replace('<th', '<th ' . $key . '="' . $val . '"', $temp);
				}
			}

			$out .= $temp . (isset($footing['data']) ? $footing['data'] : '') . $this->template['footing_cell_end'];
		}

		$out .= $this->template['footing_row_end'] . $this->newline . $this->template['tfoot_close'] . $this->newline;
	}

	$out .= $this->template['tbody_close'] . $this->newline;

	// And finally, close off the table
	$out .= $this->template['table_close'];

	// Clear table class properties before generating the table
	$this->clear();

	return $out;
}
```

</details>


<hr>

#### clear()

```php
public function clear()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Clears the table arrays.  Useful if multiple tables are being generated
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Table
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (464 - 472)</small></summary>

```php
public function clear()
{
	$this->rows        = [];
	$this->heading     = [];
	$this->footing     = [];
	$this->autoHeading = true;
	$this->caption     = null;
	return $this;
}
```

</details>


<hr>

#### _setFromDBResult()

```php
protected function _setFromDBResult($object)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set table data from a database result object
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
<td><code>$object</code></td>
<td><em>\BaseResult
</em></td>
<td>false</td>
<td>Database result object</td>
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
<summary><small>Source: 13 lines (482 - 494)</small></summary>

```php
protected function _setFromDBResult($object)
{
	// First generate the headings from the table column names
	if ($this->autoHeading === true && empty($this->heading))
	{
		$this->heading = $this->_prepArgs($object->getFieldNames());
	}

	foreach ($object->getResultArray() as $row)
	{
		$this->rows[] = $this->_prepArgs($row);
	}
}
```

</details>


<hr>

#### _setFromArray()

```php
protected function _setFromArray($data)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set table data from an array
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 12 lines (504 - 515)</small></summary>

```php
protected function _setFromArray($data)
{
	if ($this->autoHeading === true && empty($this->heading))
	{
		$this->heading = $this->_prepArgs(array_shift($data));
	}

	foreach ($data as &$row)
	{
		$this->rows[] = $this->_prepArgs($row);
	}
}
```

</details>


<hr>

#### _compileTemplate()

```php
protected function _compileTemplate()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Compile Template
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
<summary><small>Source: 17 lines (524 - 540)</small></summary>

```php
protected function _compileTemplate()
{
	if ($this->template === null)
	{
		$this->template = $this->_defaultTemplate();
		return;
	}

	$this->temp = $this->_defaultTemplate();
	foreach (['table_open', 'thead_open', 'thead_close', 'heading_row_start', 'heading_row_end', 'heading_cell_start', 'heading_cell_end', 'tbody_open', 'tbody_close', 'row_start', 'row_end', 'cell_start', 'cell_end', 'row_alt_start', 'row_alt_end', 'cell_alt_start', 'cell_alt_end', 'table_close'] as $val)
	{
		if (! isset($this->template[$val]))
		{
			$this->template[$val] = $this->temp[$val];
		}
	}
}
```

</details>


<hr>

#### _defaultTemplate()

```php
protected function _defaultTemplate()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Default Template
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
<summary><small>Source: 29 lines (549 - 577)</small></summary>

```php
protected function _defaultTemplate()
{
	return [
		'table_open'         => '<table border="0" cellpadding="4" cellspacing="0">',
		'thead_open'         => '<thead>',
		'thead_close'        => '</thead>',
		'heading_row_start'  => '<tr>',
		'heading_row_end'    => '</tr>',
		'heading_cell_start' => '<th>',
		'heading_cell_end'   => '</th>',
		'tfoot_open'         => '<tfoot>',
		'tfoot_close'        => '</tfoot>',
		'footing_row_start'  => '<tr>',
		'footing_row_end'    => '</tr>',
		'footing_cell_start' => '<td>',
		'footing_cell_end'   => '</td>',
		'tbody_open'         => '<tbody>',
		'tbody_close'        => '</tbody>',
		'row_start'          => '<tr>',
		'row_end'            => '</tr>',
		'cell_start'         => '<td>',
		'cell_end'           => '</td>',
		'row_alt_start'      => '<tr>',
		'row_alt_end'        => '</tr>',
		'cell_alt_start'     => '<td>',
		'cell_alt_end'       => '</td>',
		'table_close'        => '</table>',
	];
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/View/Table.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/View.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:17**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>