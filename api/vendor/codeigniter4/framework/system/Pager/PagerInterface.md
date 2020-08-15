


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Pager/PagerInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/Pager.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerRenderer.md">next</a></td>
</tr>
</table>







# CodeIgniter\Pager 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Pager</td></tr>
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
<td>framework/system/Pager/PagerInterface.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/Exceptions/PagerException.md">CodeIgniter\Pager\Exceptions\PagerException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/Pager.md">CodeIgniter\Pager\Pager</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerInterface.md">CodeIgniter\Pager\PagerInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerRenderer.md">CodeIgniter\Pager\PagerRenderer</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Pager\PagerInterface

<table style="text-align:left">
<tr><th>Interface</th><td>PagerInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Pager\PagerInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Expected behavior for a Pager
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
<th><a href="#links"><strong>links</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Handles creating and displaying the</td>
</tr>
<tr>
<th><a href="#simpleLinks"><strong>simpleLinks</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Creates simple Next/Previous links, instead of full pagination.</td>
</tr>
<tr>
<th><a href="#makeLinks"><strong>makeLinks</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows for a simple, manual, form of pagination where all of the data
is provided by the user. The URL is the current URI.</td>
</tr>
<tr>
<th><a href="#store"><strong>store</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Stores a set of pagination data for later display. Most commonly used
by the model to automate the process.</td>
</tr>
<tr>
<th><a href="#setPath"><strong>setPath</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the path that an aliased group of links will use.</td>
</tr>
<tr>
<th><a href="#getPageCount"><strong>getPageCount</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the total number of pages.</td>
</tr>
<tr>
<th><a href="#getCurrentPage"><strong>getCurrentPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of the current page of results.</td>
</tr>
<tr>
<th><a href="#getPageURI"><strong>getPageURI</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the URI for a specific page for the specified group.</td>
</tr>
<tr>
<th><a href="#hasMore"><strong>hasMore</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Tells whether this group of results has any more pages of results.</td>
</tr>
<tr>
<th><a href="#getFirstPage"><strong>getFirstPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the first page.</td>
</tr>
<tr>
<th><a href="#getLastPage"><strong>getLastPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the last page, if we have a total that we can calculate with.</td>
</tr>
<tr>
<th><a href="#getNextPageURI"><strong>getNextPageURI</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the full URI to the next page of results, or null.</td>
</tr>
<tr>
<th><a href="#getPreviousPageURI"><strong>getPreviousPageURI</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the full URL to the previous page of results, or null.</td>
</tr>
<tr>
<th><a href="#getPerPage"><strong>getPerPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of results per page that should be shown.</td>
</tr>
<tr>
<th><a href="#getDetails"><strong>getDetails</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an array with details about the results, including
total, per_page, current_page, last_page, next_url, prev_url, from, to.</td>
</tr>

</table>






### Methods


<hr>

#### links()

```php
public function links(string $group = 'default', string $template = 'default') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles creating and displaying the
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
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$template</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The output template alias to render.</td>
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
<summary><small>Source: line 56</small></summary>

```php
public function links(string $group = 'default', string $template = 'default'): string;
```

</details>


<hr>

#### simpleLinks()

```php
public function simpleLinks(string $group = 'default', string $template = 'default') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Creates simple Next/Previous links, instead of full pagination.
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
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$template</code></td>
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
<summary><small>Source: line 68</small></summary>

```php
public function simpleLinks(string $group = 'default', string $template = 'default'): string;
```

</details>


<hr>

#### makeLinks()

```php
public function makeLinks(int $page, int $perPage, int $total, string $template = 'default') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows for a simple, manual, form of pagination where all of the data
is provided by the user. The URL is the current URI.
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
<td><code>$page</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$perPage</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$total</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$template</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The output template alias to render.</td>
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
<summary><small>Source: line 83</small></summary>

```php
public function makeLinks(int $page, int $perPage, int $total, string $template = 'default'): string;
```

</details>


<hr>

#### store()

```php
public function store(string $group, int $page, int $perPage, int $total)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores a set of pagination data for later display. Most commonly used
by the model to automate the process.
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
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$page</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$perPage</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$total</code></td>
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
<summary><small>Source: line 98</small></summary>

```php
public function store(string $group, int $page, int $perPage, int $total);
```

</details>


<hr>

#### setPath()

```php
public function setPath(string $path, string $group = 'default')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the path that an aliased group of links will use.
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
<td><code>$path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$group</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: line 110</small></summary>

```php
public function setPath(string $path, string $group = 'default');
```

</details>


<hr>

#### getPageCount()

```php
public function getPageCount(string $group = 'default') : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the total number of pages.
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
<td><code>$group</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: line 121</small></summary>

```php
public function getPageCount(string $group = 'default'): int;
```

</details>


<hr>

#### getCurrentPage()

```php
public function getCurrentPage(string $group = 'default') : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of the current page of results.
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
<td><code>$group</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: line 132</small></summary>

```php
public function getCurrentPage(string $group = 'default'): int;
```

</details>


<hr>

#### getPageURI()

```php
public function getPageURI(int $page = null, string $group = 'default', bool $returnObject = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the URI for a specific page for the specified group.
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
<td><code>$page</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$returnObject</code></td>
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
<td>string<br>\CodeIgniter\HTTP\URI
</td>
</tr>
</table>





<details>
<summary><small>Source: line 145</small></summary>

```php
public function getPageURI(int $page = null, string $group = 'default', bool $returnObject = false);
```

</details>


<hr>

#### hasMore()

```php
public function hasMore(string $group = 'default') : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Tells whether this group of results has any more pages of results.
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
<td><code>$group</code></td>
<td><em>string<br>null
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
<summary><small>Source: line 156</small></summary>

```php
public function hasMore(string $group = 'default'): bool;
```

</details>


<hr>

#### getFirstPage()

```php
public function getFirstPage(string $group = 'default')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the first page.
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
<td><code>$group</code></td>
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
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: line 167</small></summary>

```php
public function getFirstPage(string $group = 'default');
```

</details>


<hr>

#### getLastPage()

```php
public function getLastPage(string $group = 'default')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the last page, if we have a total that we can calculate with.
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
<td><code>$group</code></td>
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
<td>int<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: line 178</small></summary>

```php
public function getLastPage(string $group = 'default');
```

</details>


<hr>

#### getNextPageURI()

```php
public function getNextPageURI(string $group = 'default')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the full URI to the next page of results, or null.
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
<td><code>$group</code></td>
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
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: line 189</small></summary>

```php
public function getNextPageURI(string $group = 'default');
```

</details>


<hr>

#### getPreviousPageURI()

```php
public function getPreviousPageURI(string $group = 'default')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the full URL to the previous page of results, or null.
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
<td><code>$group</code></td>
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
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: line 200</small></summary>

```php
public function getPreviousPageURI(string $group = 'default');
```

</details>


<hr>

#### getPerPage()

```php
public function getPerPage(string $group = 'default') : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of results per page that should be shown.
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
<td><code>$group</code></td>
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
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: line 211</small></summary>

```php
public function getPerPage(string $group = 'default'): int;
```

</details>


<hr>

#### getDetails()

```php
public function getDetails(string $group = 'default') : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array with details about the results, including
total, per_page, current_page, last_page, next_url, prev_url, from, to.
</td></tr>
</table>

<table>
<tr><td>
Does not include the actual data. This data is suitable for adding
a 'data' object to with the result set and converting to JSON.
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
<td><code>$group</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: line 225</small></summary>

```php
public function getDetails(string $group = 'default'): array;
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Pager/PagerInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/Pager.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerRenderer.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:18**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>