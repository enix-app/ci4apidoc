


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Pager/PagerRenderer.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/RESTful/ResourceController.md">next</a></td>
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
<td>framework/system/Pager/PagerRenderer.php
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



 

 
## CodeIgniter\Pager\PagerRenderer

<table style="text-align:left">
<tr><th>Class</th><td>PagerRenderer</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Pager\PagerRenderer</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class PagerRenderer
</td></tr>
</table>

<table>
<tr><td>
This class is passed to the view that describes the pagination,
and is used to get the link information and provide utility
methods needed to work with pagination.
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
<th><a href="#first"><strong>first</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>First page number.</td>
</tr>
<tr>
<th><a href="#last"><strong>last</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Last page number.</td>
</tr>
<tr>
<th><a href="#current"><strong>current</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Current page number.</td>
</tr>
<tr>
<th><a href="#total"><strong>total</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Total number of pages? unused?</td>
</tr>
<tr>
<th><a href="#pageCount"><strong>pageCount</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Page count?</td>
</tr>
<tr>
<th><a href="#uri"><strong>uri</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>URI base for pagination links</td>
</tr>
<tr>
<th><a href="#segment"><strong>segment</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Segment number used for pagination.</td>
</tr>
<tr>
<th><a href="#pageSelector"><strong>pageSelector</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Name of $_GET parameter</td>
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
<th><a href="#setSurroundCount"><strong>setSurroundCount</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the total number of links that should appear on either
side of the current page. Adjusts the first and last counts
to reflect it.</td>
</tr>
<tr>
<th><a href="#hasPrevious"><strong>hasPrevious</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if there is a &quot;previous&quot; page before our &quot;first&quot; page.</td>
</tr>
<tr>
<th><a href="#getPrevious"><strong>getPrevious</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a URL to the &quot;previous&quot; page. The previous page is NOT the
page before the current page, but is the page just before the
&quot;first&quot; page.</td>
</tr>
<tr>
<th><a href="#hasNext"><strong>hasNext</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if there is a &quot;next&quot; page after our &quot;last&quot; page.</td>
</tr>
<tr>
<th><a href="#getNext"><strong>getNext</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a URL to the &quot;next&quot; page. The next page is NOT, the
page after the current page, but is the page that follows the
&quot;last&quot; page.</td>
</tr>
<tr>
<th><a href="#getFirst"><strong>getFirst</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the URI of the first page.</td>
</tr>
<tr>
<th><a href="#getLast"><strong>getLast</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the URI of the last page.</td>
</tr>
<tr>
<th><a href="#getCurrent"><strong>getCurrent</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the URI of the current page.</td>
</tr>
<tr>
<th><a href="#links"><strong>links</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an array of links that should be displayed. Each link
is represented by another array containing of the URI the link
should go to, the title (number) of the link, and a boolean
value representing whether this link is active or not.</td>
</tr>
<tr>
<th><a href="#updatePages"><strong>updatePages</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Updates the first and last pages based on $surroundCount,
which is the number of links surrounding the active page
to show.</td>
</tr>
<tr>
<th><a href="#hasPreviousPage"><strong>hasPreviousPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if there is a &quot;previous&quot; page before our &quot;first&quot; page.</td>
</tr>
<tr>
<th><a href="#getPreviousPage"><strong>getPreviousPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a URL to the &quot;previous&quot; page.</td>
</tr>
<tr>
<th><a href="#hasNextPage"><strong>hasNextPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if there is a &quot;next&quot; page after our &quot;last&quot; page.</td>
</tr>
<tr>
<th><a href="#getNextPage"><strong>getNextPage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a URL to the &quot;next&quot; page.</td>
</tr>

</table>





### Properties


<hr>

#### $first

```php
protected $first;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
First page number.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $last

```php
protected $last;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Last page number.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $current

```php
protected $current;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Current page number.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $total

```php
protected $total;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Total number of pages? unused?
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $pageCount

```php
protected $pageCount;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Page count?
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $uri

```php
protected $uri;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
URI base for pagination links
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $segment

```php
protected $segment;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Segment number used for pagination.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $pageSelector

```php
protected $pageSelector;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Name of $_GET parameter
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(array $details)
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
<td><code>$details</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 11 lines (110 - 120)</small></summary>

```php
public function __construct(array $details)
{
	$this->first        = 1;
	$this->last         = $details['pageCount'];
	$this->current      = $details['currentPage'];
	$this->total        = $details['total'];
	$this->uri          = $details['uri'];
	$this->pageCount    = $details['pageCount'];
	$this->segment      = $details['segment'] ?? 0;
	$this->pageSelector = $details['pageSelector'] ?? 'page';
}
```

</details>


<hr>

#### setSurroundCount()

```php
public function setSurroundCount(int $count = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the total number of links that should appear on either
side of the current page. Adjusts the first and last counts
to reflect it.
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
<td><code>$count</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\PagerRenderer
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (133 - 138)</small></summary>

```php
public function setSurroundCount(int $count = null)
{
	$this->updatePages($count);

	return $this;
}
```

</details>


<hr>

#### hasPrevious()

```php
public function hasPrevious() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if there is a "previous" page before our "first" page.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (147 - 150)</small></summary>

```php
public function hasPrevious(): bool
{
	return $this->first > 1;
}
```

</details>


<hr>

#### getPrevious()

```php
public function getPrevious()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a URL to the "previous" page. The previous page is NOT the
page before the current page, but is the page just before the
"first" page.
</td></tr>
</table>

<table>
<tr><td>
You MUST call hasPrevious() first, or this value may be invalid.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 20 lines (163 - 182)</small></summary>

```php
public function getPrevious()
{
	if (! $this->hasPrevious())
	{
		return null;
	}

	$uri = clone $this->uri;

	if ($this->segment === 0)
	{
		$uri->addQuery($this->pageSelector, $this->first - 1);
	}
	else
	{
		$uri->setSegment($this->segment, $this->first - 1);
	}

	return (string) $uri;
}
```

</details>


<hr>

#### hasNext()

```php
public function hasNext() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if there is a "next" page after our "last" page.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (191 - 194)</small></summary>

```php
public function hasNext(): bool
{
	return $this->pageCount > $this->last;
}
```

</details>


<hr>

#### getNext()

```php
public function getNext()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a URL to the "next" page. The next page is NOT, the
page after the current page, but is the page that follows the
"last" page.
</td></tr>
</table>

<table>
<tr><td>
You MUST call hasNext() first, or this value may be invalid.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 20 lines (207 - 226)</small></summary>

```php
public function getNext()
{
	if (! $this->hasNext())
	{
		return null;
	}

	$uri = clone $this->uri;

	if ($this->segment === 0)
	{
		$uri->addQuery($this->pageSelector, $this->last + 1);
	}
	else
	{
		$uri->setSegment($this->segment, $this->last + 1);
	}

	return (string) $uri;
}
```

</details>


<hr>

#### getFirst()

```php
public function getFirst() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the URI of the first page.
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
<summary><small>Source: 15 lines (235 - 249)</small></summary>

```php
public function getFirst(): string
{
	$uri = clone $this->uri;

	if ($this->segment === 0)
	{
		$uri->addQuery($this->pageSelector, 1);
	}
	else
	{
		$uri->setSegment($this->segment, 1);
	}

	return (string) $uri;
}
```

</details>


<hr>

#### getLast()

```php
public function getLast() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the URI of the last page.
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
<summary><small>Source: 15 lines (258 - 272)</small></summary>

```php
public function getLast(): string
{
	$uri = clone $this->uri;

	if ($this->segment === 0)
	{
		$uri->addQuery($this->pageSelector, $this->pageCount);
	}
	else
	{
		$uri->setSegment($this->segment, $this->pageCount);
	}

	return (string) $uri;
}
```

</details>


<hr>

#### getCurrent()

```php
public function getCurrent() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the URI of the current page.
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
<summary><small>Source: 15 lines (281 - 295)</small></summary>

```php
public function getCurrent(): string
{
	$uri = clone $this->uri;

	if ($this->segment === 0)
	{
		$uri->addQuery($this->pageSelector, $this->current);
	}
	else
	{
		$uri->setSegment($this->segment, $this->current);
	}

	return (string) $uri;
}
```

</details>


<hr>

#### links()

```php
public function links() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array of links that should be displayed. Each link
is represented by another array containing of the URI the link
should go to, the title (number) of the link, and a boolean
value representing whether this link is active or not.
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
<summary><small>Source: 17 lines (307 - 323)</small></summary>

```php
public function links(): array
{
	$links = [];

	$uri = clone $this->uri;

	for ($i = $this->first; $i <= $this->last; $i ++)
	{
		$links[] = [
			'uri'    => (string) ($this->segment === 0 ? $uri->addQuery($this->pageSelector, $i) : $uri->setSegment($this->segment, $i)),
			'title'  => (int) $i,
			'active' => ($i === $this->current),
		];
	}

	return $links;
}
```

</details>


<hr>

#### updatePages()

```php
protected function updatePages(int $count = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Updates the first and last pages based on $surroundCount,
which is the number of links surrounding the active page
to show.
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
<td><code>$count</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td>The new "surroundCount"</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 10 lines (334 - 343)</small></summary>

```php
protected function updatePages(int $count = null)
{
	if (is_null($count))
	{
		return;
	}

	$this->first = $this->current - $count > 0 ? (int) ($this->current - $count) : 1;
	$this->last  = $this->current + $count <= $this->pageCount ? (int) ($this->current + $count) : (int) $this->pageCount;
}
```

</details>


<hr>

#### hasPreviousPage()

```php
public function hasPreviousPage() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if there is a "previous" page before our "first" page.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (352 - 355)</small></summary>

```php
public function hasPreviousPage(): bool
{
	return $this->current > 1;
}
```

</details>


<hr>

#### getPreviousPage()

```php
public function getPreviousPage()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a URL to the "previous" page.
</td></tr>
</table>

<table>
<tr><td>
You MUST call hasPreviousPage() first, or this value may be invalid.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 20 lines (366 - 385)</small></summary>

```php
public function getPreviousPage()
{
	if (! $this->hasPreviousPage())
	{
		return null;
	}

	$uri = clone $this->uri;

	if ($this->segment === 0)
	{
		$uri->addQuery($this->pageSelector, $this->current - 1);
	}
	else
	{
		$uri->setSegment($this->segment, $this->current - 1);
	}

	return (string) $uri;
}
```

</details>


<hr>

#### hasNextPage()

```php
public function hasNextPage() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if there is a "next" page after our "last" page.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (394 - 397)</small></summary>

```php
public function hasNextPage(): bool
{
	return $this->current < $this->last;
}
```

</details>


<hr>

#### getNextPage()

```php
public function getNextPage()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a URL to the "next" page.
</td></tr>
</table>

<table>
<tr><td>
You MUST call hasNextPage() first, or this value may be invalid.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 20 lines (408 - 427)</small></summary>

```php
public function getNextPage()
{
	if (! $this->hasNextPage())
	{
		return null;
	}

	$uri = clone $this->uri;

	if ($this->segment === 0)
	{
		$uri->addQuery($this->pageSelector, $this->current + 1);
	}
	else
	{
		$uri->setSegment($this->segment, $this->current + 1);
	}

	return (string) $uri;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Pager/PagerRenderer.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/RESTful/ResourceController.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:18**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>