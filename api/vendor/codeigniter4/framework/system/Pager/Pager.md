


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Pager/Pager.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/Exceptions/PagerException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerInterface.md">next</a></td>
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
<td>framework/system/Pager/Pager.php
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



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/Exceptions/PagerException.md"><strong>CodeIgniter\Pager\Exceptions\PagerException</strong></a>
</td>
<td>PagerException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md"><strong>CodeIgniter\View\RendererInterface</strong></a>
</td>
<td>RendererInterface</td>
</tr>
</table>



 
## CodeIgniter\Pager\Pager

<table style="text-align:left">
<tr><th>Class</th><td>Pager</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Pager\Pager</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerInterface.md">CodeIgniter\Pager\PagerInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Pager
</td></tr>
</table>

<table>
<tr><td>
The Pager class provides semi-automatic and manual methods for creating
pagination links and reading the current url's query variable, "page"
to determine the current page. This class can support multiple
paginations on a single page.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Pager
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
<th><a href="#groups"><strong>groups</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The group data.</td>
</tr>
<tr>
<th><a href="#segment"><strong>segment</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>URI segment for groups if provided.</td>
</tr>
<tr>
<th><a href="#config"><strong>config</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Our configuration instance.</td>
</tr>
<tr>
<th><a href="#view"><strong>view</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The view engine to render the links with.</td>
</tr>
<tr>
<th><a href="#only"><strong>only</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>List of only permitted queries</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor.</td>
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
<th><a href="#displayLinks"><strong>displayLinks</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Does the actual work of displaying the view file. Used internally
by links(), simpleLinks(), and makeLinks().</td>
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
<th><a href="#setSegment"><strong>setSegment</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets segment for a group.</td>
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
<th><a href="#hasMore"><strong>hasMore</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Tells whether this group of results has any more pages of results.</td>
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
<th><a href="#getFirstPage"><strong>getFirstPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines the first page # that should be shown.</td>
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
<tr>
<th><a href="#only"><strong>only</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets only allowed queries on pagination links.</td>
</tr>
<tr>
<th><a href="#ensureGroup"><strong>ensureGroup</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Ensures that an array exists for the group specified.</td>
</tr>
<tr>
<th><a href="#calculateCurrentPage"><strong>calculateCurrentPage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Calculating the current page</td>
</tr>

</table>





### Properties


<hr>

#### $groups

```php
protected $groups = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The group data.
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

#### $segment

```php
protected $segment = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
URI segment for groups if provided.
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

#### $config

```php
protected $config;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Our configuration instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Config\Pager
</td>
</tr>
</table>


<hr>

#### $view

```php
protected $view;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The view engine to render the links with.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\RendererInterface
</td>
</tr>
</table>


<hr>

#### $only

```php
protected $only = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
List of only permitted queries
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

#### __construct()

```php
public function __construct($config, RendererInterface $view)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor.
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
<td><em>\type
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$view</code></td>
<td><em>\RendererInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 5 lines (101 - 105)</small></summary>

```php
public function __construct($config, RendererInterface $view)
{
	$this->config = $config;
	$this->view   = $view;
}
```

</details>


<hr>

#### links()

```php
public function links(string $group = 'default', string $template = 'default_full') : string
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
<summary><small>Source: 6 lines (117 - 122)</small></summary>

```php
public function links(string $group = 'default', string $template = 'default_full'): string
{
	$this->ensureGroup($group);

	return $this->displayLinks($group, $template);
}
```

</details>


<hr>

#### simpleLinks()

```php
public function simpleLinks(string $group = 'default', string $template = 'default_simple') : string
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
<summary><small>Source: 6 lines (134 - 139)</small></summary>

```php
public function simpleLinks(string $group = 'default', string $template = 'default_simple'): string
{
	$this->ensureGroup($group);

	return $this->displayLinks($group, $template);
}
```

</details>


<hr>

#### makeLinks()

```php
public function makeLinks(int $page, int $perPage = null, int $total, string $template = 'default_full', int $segment = 0, ?string $group = 'default') : string
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

<tr>
<td>5.</td>
<td><code>$segment</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>(if page number is provided by URI segment)</td>
</tr>

<tr>
<td>6.</td>
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>optional group (i.e. if we'd like to define custom path)</td>
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
<summary><small>Source: 8 lines (156 - 163)</small></summary>

```php
public function makeLinks(int $page, int $perPage = null, int $total, string $template = 'default_full', int $segment = 0, ?string $group = 'default'): string
{
	$group = $group === '' ? 'default' : $group;

	$this->store($group, $page, $perPage ?? $this->config->perPage, $total, $segment);

	return $this->displayLinks($group, $template);
}
```

</details>


<hr>

#### displayLinks()

```php
protected function displayLinks(string $group, string $template) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does the actual work of displaying the view file. Used internally
by links(), simpleLinks(), and makeLinks().
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
<summary><small>Source: 12 lines (176 - 187)</small></summary>

```php
protected function displayLinks(string $group, string $template): string
{
	$pager = new PagerRenderer($this->getDetails($group));

	if (! array_key_exists($template, $this->config->templates))
	{
		throw PagerException::forInvalidTemplate($template);
	}

	return $this->view->setVar('pager', $pager)
					->render($this->config->templates[$template]);
}
```

</details>


<hr>

#### store()

```php
public function store(string $group, int $page, int $perPage = null, int $total, int $segment = 0)
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

<tr>
<td>5.</td>
<td><code>$segment</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 23 lines (203 - 225)</small></summary>

```php
public function store(string $group, int $page, int $perPage = null, int $total, int $segment = 0)
{
	if ($segment)
	{
		$this->setSegment($segment, $group);
	}

	$this->ensureGroup($group, $perPage);

	if ($segment > 0 && $this->groups[$group]['currentPage'] > 0)
	{
		$page = $this->groups[$group]['currentPage'];
	}

	$perPage                             = $perPage ?? $this->config->perPage;
	$pageCount                           = (int)ceil($total / $perPage);
	$this->groups[$group]['currentPage'] = $page > $pageCount ? $pageCount : $page;
	$this->groups[$group]['perPage']     = $perPage;
	$this->groups[$group]['total']       = $total;
	$this->groups[$group]['pageCount']   = $pageCount;

	return $this;
}
```

</details>


<hr>

#### setSegment()

```php
public function setSegment(int $number, string $group = 'default')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets segment for a group.
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
<td><code>$number</code></td>
<td><em>int
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
<summary><small>Source: 6 lines (237 - 242)</small></summary>

```php
public function setSegment(int $number, string $group = 'default')
{
	$this->segment[$group] = $number;

	return $this;
}
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
<summary><small>Source: 8 lines (254 - 261)</small></summary>

```php
public function setPath(string $path, string $group = 'default')
{
	$this->ensureGroup($group);

	$this->groups[$group]['uri']->setPath($path);

	return $this;
}
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
<summary><small>Source: 6 lines (272 - 277)</small></summary>

```php
public function getPageCount(string $group = 'default'): int
{
	$this->ensureGroup($group);

	return $this->groups[$group]['pageCount'];
}
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
<summary><small>Source: 6 lines (288 - 293)</small></summary>

```php
public function getCurrentPage(string $group = 'default'): int
{
	$this->ensureGroup($group);

	return $this->groups[$group]['currentPage'] ?: 1;
}
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
<summary><small>Source: 6 lines (304 - 309)</small></summary>

```php
public function hasMore(string $group = 'default'): bool
{
	$this->ensureGroup($group);

	return ($this->groups[$group]['currentPage'] * $this->groups[$group]['perPage']) < $this->groups[$group]['total'];
}
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
<summary><small>Source: 11 lines (320 - 330)</small></summary>

```php
public function getLastPage(string $group = 'default')
{
	$this->ensureGroup($group);

	if (! is_numeric($this->groups[$group]['total']) || ! is_numeric($this->groups[$group]['perPage']))
	{
		return null;
	}

	return (int)ceil($this->groups[$group]['total'] / $this->groups[$group]['perPage']);
}
```

</details>


<hr>

#### getFirstPage()

```php
public function getFirstPage(string $group = 'default') : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines the first page # that should be shown.
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
<summary><small>Source: 7 lines (341 - 347)</small></summary>

```php
public function getFirstPage(string $group = 'default'): int
{
	$this->ensureGroup($group);

	// @todo determine based on a 'surroundCount' value
	return 1;
}
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
<summary><small>Source: 34 lines (360 - 393)</small></summary>

```php
public function getPageURI(int $page = null, string $group = 'default', bool $returnObject = false)
{
	$this->ensureGroup($group);

	/**
	 * @var \CodeIgniter\HTTP\URI $uri
	 */
	$uri = $this->groups[$group]['uri'];

	$segment = $this->segment[$group] ?? 0;

	if ($segment)
	{
		$uri->setSegment($segment, $page);
	}
	else
	{
		$uri->addQuery($this->groups[$group]['pageSelector'], $page);
	}

	if ($this->only)
	{
		$query = array_intersect_key($_GET, array_flip($this->only));

		if (! $segment)
		{
			$query[$this->groups[$group]['pageSelector']] = $page;
		}

		$uri->setQueryArray($query);
	}

	return $returnObject === true ? $uri : (string) $uri;
}
```

</details>


<hr>

#### getNextPageURI()

```php
public function getNextPageURI(string $group = 'default', bool $returnObject = false)
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

<tr>
<td>2.</td>
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
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 20 lines (405 - 424)</small></summary>

```php
public function getNextPageURI(string $group = 'default', bool $returnObject = false)
{
	$this->ensureGroup($group);

	$last = $this->getLastPage($group);
	$curr = $this->getCurrentPage($group);
	$page = null;

	if (! empty($last) && ! empty($curr) && $last === $curr)
	{
		return null;
	}

	if ($last > $curr)
	{
		$page = $curr + 1;
	}

	return $this->getPageURI($page, $group, $returnObject);
}
```

</details>


<hr>

#### getPreviousPageURI()

```php
public function getPreviousPageURI(string $group = 'default', bool $returnObject = false)
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

<tr>
<td>2.</td>
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
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 20 lines (436 - 455)</small></summary>

```php
public function getPreviousPageURI(string $group = 'default', bool $returnObject = false)
{
	$this->ensureGroup($group);

	$first = $this->getFirstPage($group);
	$curr  = $this->getCurrentPage($group);
	$page  = null;

	if (! empty($first) && ! empty($curr) && $first === $curr)
	{
		return null;
	}

	if ($first < $curr)
	{
		$page = $curr - 1;
	}

	return $this->getPageURI($page, $group, $returnObject);
}
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
<summary><small>Source: 6 lines (466 - 471)</small></summary>

```php
public function getPerPage(string $group = 'default'): int
{
	$this->ensureGroup($group);

	return (int) $this->groups[$group]['perPage'];
}
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
<summary><small>Source: 15 lines (485 - 499)</small></summary>

```php
public function getDetails(string $group = 'default'): array
{
	if (! array_key_exists($group, $this->groups))
	{
		throw PagerException::forInvalidPaginationGroup($group);
	}

	$newGroup = $this->groups[$group];

	$newGroup['next']     = $this->getNextPageURI($group);
	$newGroup['previous'] = $this->getPreviousPageURI($group);
	$newGroup['segment']  = $this->segment[$group] ?? 0;

	return $newGroup;
}
```

</details>


<hr>

#### only()

```php
public function only(array $queries) : Pager
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets only allowed queries on pagination links.
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
<td><code>$queries</code></td>
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
<td>\Pager
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (510 - 515)</small></summary>

```php
public function only(array $queries):Pager
{
	$this->only = $queries;

	return $this;
}
```

</details>


<hr>

#### ensureGroup()

```php
protected function ensureGroup(string $group, int $perPage = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ensures that an array exists for the group specified.
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
<td><code>$perPage</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 23 lines (525 - 547)</small></summary>

```php
protected function ensureGroup(string $group, int $perPage = null)
{
	if (array_key_exists($group, $this->groups))
	{
		return;
	}

	$this->groups[$group] = [
		'uri'          => clone current_url(true),
		'hasMore'      => false,
		'total'        => null,
		'perPage'      => $perPage ?? $this->config->perPage,
		'pageCount'    => 1,
		'pageSelector' => $group === 'default' ? 'page' : 'page_' . $group,
	];

	$this->calculateCurrentPage($group);

	if ($_GET)
	{
		$this->groups[$group]['uri'] = $this->groups[$group]['uri']->setQueryArray($_GET);
	}
}
```

</details>


<hr>

#### calculateCurrentPage()

```php
protected function calculateCurrentPage(string $group)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Calculating the current page
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








<details>
<summary><small>Source: 22 lines (556 - 577)</small></summary>

```php
protected function calculateCurrentPage(string $group)
{
	if (array_key_exists($group, $this->segment))
	{
		try
		{
			$this->groups[$group]['currentPage'] = (int) $this->groups[$group]['uri']->setSilent(false)->getSegment($this->segment[$group]);
		}
		catch (\CodeIgniter\HTTP\Exceptions\HTTPException $e)
		{
			$this->groups[$group]['currentPage'] = 1;
		}
	}
	else
	{
		$pageSelector = $this->groups[$group]['pageSelector'];

		$page = (int) ($_GET[$pageSelector] ?? 1);

		$this->groups[$group]['currentPage'] = $page < 1 ? 1 : $page;
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Pager/Pager.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/Exceptions/PagerException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>