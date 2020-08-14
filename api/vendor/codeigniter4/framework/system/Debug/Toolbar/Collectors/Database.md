


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Toolbar/Collectors/Database.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Config.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Events.md">next</a></td>
</tr>
</table>







# CodeIgniter\Debug\Toolbar\Collectors 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Debug\Toolbar\Collectors</td></tr>
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
<td>framework/system/Debug/Toolbar/Collectors/Database.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/BaseCollector.md">CodeIgniter\Debug\Toolbar\Collectors\BaseCollector</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Config.md">CodeIgniter\Debug\Toolbar\Collectors\Config</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Database.md">CodeIgniter\Debug\Toolbar\Collectors\Database</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Events.md">CodeIgniter\Debug\Toolbar\Collectors\Events</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Files.md">CodeIgniter\Debug\Toolbar\Collectors\Files</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/History.md">CodeIgniter\Debug\Toolbar\Collectors\History</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Logs.md">CodeIgniter\Debug\Toolbar\Collectors\Logs</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Routes.md">CodeIgniter\Debug\Toolbar\Collectors\Routes</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Timers.md">CodeIgniter\Debug\Toolbar\Collectors\Timers</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Views.md">CodeIgniter\Debug\Toolbar\Collectors\Views</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Database/Query.md"><strong>CodeIgniter\Database\Query</strong></a>
</td>
<td>Query</td>
</tr>
</table>



 
## CodeIgniter\Debug\Toolbar\Collectors\Database

<table style="text-align:left">
<tr><th>Class</th><td>Database</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Debug\Toolbar\Collectors\Database</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/BaseCollector.md">CodeIgniter\Debug\Toolbar\Collectors\BaseCollector</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Collector for the Database tab of the Debug Toolbar.
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
<th><a href="#hasTimeline"><strong>hasTimeline</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this collector has timeline data.</td>
</tr>
<tr>
<th><a href="#hasTabContent"><strong>hasTabContent</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this collector should display its own tab.</td>
</tr>
<tr>
<th><a href="#hasVarData"><strong>hasVarData</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this collector has data for the Vars tab.</td>
</tr>
<tr>
<th><a href="#title"><strong>title</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name used to reference this collector in the toolbar.</td>
</tr>
<tr>
<th><a href="#connections"><strong>connections</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Array of database connections.</td>
</tr>
<tr>
<th><a href="#queries"><strong>queries</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>The query instances that have been collected
through the DBQuery Event.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor</td>
</tr>
<tr>
<th><a href="#collect"><strong>collect</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>The static method used during Events to collect
data.</td>
</tr>
<tr>
<th><a href="#formatTimelineData"><strong>formatTimelineData</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Returns timeline data formatted for the toolbar.</td>
</tr>
<tr>
<th><a href="#display"><strong>display</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the data of this collector to be formatted in the toolbar</td>
</tr>
<tr>
<th><a href="#getBadgeValue"><strong>getBadgeValue</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Gets the &quot;badge&quot; value for the button.</td>
</tr>
<tr>
<th><a href="#getTitleDetails"><strong>getTitleDetails</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Information to be displayed next to the title.</td>
</tr>
<tr>
<th><a href="#isEmpty"><strong>isEmpty</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Does this collector have any data collected?</td>
</tr>
<tr>
<th><a href="#icon"><strong>icon</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Display the icon.</td>
</tr>

</table>





### Properties


<hr>

#### $hasTimeline

```php
protected $hasTimeline = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether this collector has timeline data.
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

#### $hasTabContent

```php
protected $hasTabContent = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether this collector should display its own tab.
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

#### $hasVarData

```php
protected $hasVarData = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether this collector has data for the Vars tab.
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

#### $title

```php
protected $title = 'Database';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name used to reference this collector in the toolbar.
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

#### $connections

```php
protected $connections;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Array of database connections.
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

#### $queries

```php
protected static $queries = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The query instances that have been collected
through the DBQuery Event.
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
public function __construct()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (98 - 101)</small></summary>

```php
public function __construct()
{
	$this->connections = \Config\Database::getConnections();
}
```

</details>


<hr>

#### collect()

```php
public static function collect(Query $query)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The static method used during Events to collect
data.
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>internal</th>
<td>param $ array \CodeIgniter\Database\Query
</td>
</tr>
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
<td><code>$query</code></td>
<td><em>\CodeIgniter\Database\Query
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 12 lines (113 - 124)</small></summary>

```php
public static function collect(Query $query)
{
	$config = config('Toolbar');

	// Provide default in case it's not set
	$max = $config->maxQueries ?: 100;

	if (count(static::$queries) < $max)
	{
		static::$queries[] = $query;
	}
}
```

</details>


<hr>

#### formatTimelineData()

```php
protected function formatTimelineData() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns timeline data formatted for the toolbar.
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
<summary><small>Source: 27 lines (133 - 159)</small></summary>

```php
protected function formatTimelineData(): array
{
	$data = [];

	foreach ($this->connections as $alias => $connection)
	{
		// Connection Time
		$data[] = [
			'name'      => 'Connecting to Database: "' . $alias . '"',
			'component' => 'Database',
			'start'     => $connection->getConnectStart(),
			'duration'  => $connection->getConnectDuration(),
		];
	}

	foreach (static::$queries as $query)
	{
		$data[] = [
			'name'      => 'Query',
			'component' => 'Database',
			'start'     => $query->getStartTime(true),
			'duration'  => $query->getDuration(),
		];
	}

	return $data;
}
```

</details>


<hr>

#### display()

```php
public function display() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the data of this collector to be formatted in the toolbar
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
<summary><small>Source: 58 lines (168 - 225)</small></summary>

```php
public function display(): array
{
	// Key words we want bolded
	$highlight = [
		'SELECT',
		'DISTINCT',
		'FROM',
		'WHERE',
		'AND',
		'LEFT&nbsp;JOIN',
		'RIGHT&nbsp;JOIN',
		'JOIN',
		'ORDER&nbsp;BY',
		'GROUP&nbsp;BY',
		'LIMIT',
		'INSERT',
		'INTO',
		'VALUES',
		'UPDATE',
		'OR&nbsp;',
		'HAVING',
		'OFFSET',
		'NOT&nbsp;IN',
		'IN',
		'LIKE',
		'NOT&nbsp;LIKE',
		'COUNT',
		'MAX',
		'MIN',
		'ON',
		'AS',
		'AVG',
		'SUM',
		'(',
		')',
	];

	$data = [
		'queries' => [],
	];

	foreach (static::$queries as $query)
	{
		$sql = $query->getQuery();

		foreach ($highlight as $term)
		{
			$sql = str_replace($term, "<strong>{$term}</strong>", $sql);
		}

		$data['queries'][] = [
			'duration' => ($query->getDuration(5) * 1000) . ' ms',
			'sql'      => $sql,
		];
	}

	return $data;
}
```

</details>


<hr>

#### getBadgeValue()

```php
public function getBadgeValue() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets the "badge" value for the button.
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
<summary><small>Source: 4 lines (234 - 237)</small></summary>

```php
public function getBadgeValue(): int
{
	return count(static::$queries);
}
```

</details>


<hr>

#### getTitleDetails()

```php
public function getTitleDetails() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Information to be displayed next to the title.
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
<summary><small>Source: 5 lines (246 - 250)</small></summary>

```php
public function getTitleDetails(): string
{
	return '(' . count(static::$queries) . ' Queries across ' . ($countConnection = count($this->connections)) . ' Connection' .
			($countConnection > 1 ? 's' : '') . ')';
}
```

</details>


<hr>

#### isEmpty()

```php
public function isEmpty() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does this collector have any data collected?
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
<summary><small>Source: 4 lines (259 - 262)</small></summary>

```php
public function isEmpty(): bool
{
	return empty(static::$queries);
}
```

</details>


<hr>

#### icon()

```php
public function icon() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Display the icon.
</td></tr>
</table>

<table>
<tr><td>
Icon from <a href="https://icons8.com">https://icons8.com</a> - 1em package
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
<summary><small>Source: 4 lines (273 - 276)</small></summary>

```php
public function icon(): string
{
	return 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAADMSURBVEhLY6A3YExLSwsA4nIycQDIDIhRWEBqamo/UNF/SjDQjF6ocZgAKPkRiFeEhoYyQ4WIBiA9QAuWAPEHqBAmgLqgHcolGQD1V4DMgHIxwbCxYD+QBqcKINseKo6eWrBioPrtQBq/BcgY5ht0cUIYbBg2AJKkRxCNWkDQgtFUNJwtABr+F6igE8olGQD114HMgHIxAVDyAhA/AlpSA8RYUwoeXAPVex5qHCbIyMgwBCkAuQJIY00huDBUz/mUlBQDqHGjgBjAwAAACexpph6oHSQAAAAASUVORK5CYII=';
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Toolbar/Collectors/Database.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Config.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Events.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>