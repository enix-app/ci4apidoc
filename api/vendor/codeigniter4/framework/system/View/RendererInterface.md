


 



<table>
<tr>
<td style="width:100%"><em>framework/system/View/RendererInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Plugins.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Table.md">next</a></td>
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
<td>framework/system/View/RendererInterface.php
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



 

 
## CodeIgniter\View\RendererInterface

<table style="text-align:left">
<tr><th>Interface</th><td>RendererInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\View\RendererInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Interface RendererInterface
</td></tr>
</table>

<table>
<tr><td>
The interface used for displaying Views and/or theme files.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\View
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
<th><a href="#render"><strong>render</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Builds the output based upon a file name and any
data that has already been set.</td>
</tr>
<tr>
<th><a href="#renderString"><strong>renderString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Builds the output based upon a string and any
data that has already been set.</td>
</tr>
<tr>
<th><a href="#setData"><strong>setData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets several pieces of view data at once.</td>
</tr>
<tr>
<th><a href="#setVar"><strong>setVar</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets a single piece of view data.</td>
</tr>
<tr>
<th><a href="#resetData"><strong>resetData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Removes all of the view data from the system.</td>
</tr>

</table>






### Methods


<hr>

#### render()

```php
public function render(string $view, array $options = null, bool $saveData = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Builds the output based upon a file name and any
data that has already been set.
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
<td><code>$view</code></td>
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
<td>Reserved for 3rd-party uses since
it might be needed to pass additional info
to other template engines.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$saveData</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>If true, will save data for use with any other calls,
if false, will clean the data after displaying the view,
   if not specified, use the config setting.</td>
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
<summary><small>Source: line 66</small></summary>

```php
public function render(string $view, array $options = null, bool $saveData = false): string;
```

</details>


<hr>

#### renderString()

```php
public function renderString(string $view, array $options = null, bool $saveData = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Builds the output based upon a string and any
data that has already been set.
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
<td><code>$view</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The view contents</td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Reserved for 3rd-party uses since
it might be needed to pass additional info
to other template engines.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$saveData</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>If true, will save data for use with any other calls,
if false, will clean the data after displaying the view,
   if not specified, use the config setting.</td>
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
<summary><small>Source: line 84</small></summary>

```php
public function renderString(string $view, array $options = null, bool $saveData = false): string;
```

</details>


<hr>

#### setData()

```php
public function setData(array $data = array(), string $context = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets several pieces of view data at once.
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

<tr>
<td>2.</td>
<td><code>$context</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The context to escape it for: html, css, js, url
If 'raw', no escaping will happen</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\RendererInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 97</small></summary>

```php
public function setData(array $data = [], string $context = null);
```

</details>


<hr>

#### setVar()

```php
public function setVar(string $name, $value = null, string $context = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets a single piece of view data.
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
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$context</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The context to escape it for: html, css, js, url
If 'raw' no escaping will happen</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\RendererInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 111</small></summary>

```php
public function setVar(string $name, $value = null, string $context = null);
```

</details>


<hr>

#### resetData()

```php
public function resetData()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes all of the view data from the system.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\RendererInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 120</small></summary>

```php
public function resetData();
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/View/RendererInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Plugins.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Table.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>