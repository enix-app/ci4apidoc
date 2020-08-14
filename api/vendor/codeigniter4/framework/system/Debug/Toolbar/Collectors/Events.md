


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Toolbar/Collectors/Events.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Database.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Files.md">next</a></td>
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
<td>framework/system/Debug/Toolbar/Collectors/Events.php
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
<a href="../../../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md"><strong>CodeIgniter\View\RendererInterface</strong></a>
</td>
<td>RendererInterface</td>
</tr>
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
</table>



 
## CodeIgniter\Debug\Toolbar\Collectors\Events

<table style="text-align:left">
<tr><th>Class</th><td>Events</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Debug\Toolbar\Collectors\Events</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/BaseCollector.md">CodeIgniter\Debug\Toolbar\Collectors\BaseCollector</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Views collector
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
<td>Whether this collector has data that can
be displayed in the Timeline.</td>
</tr>
<tr>
<th><a href="#hasTabContent"><strong>hasTabContent</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this collector needs to display
content in a tab or not.</td>
</tr>
<tr>
<th><a href="#hasVarData"><strong>hasVarData</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this collector has data that
should be shown in the Vars tab.</td>
</tr>
<tr>
<th><a href="#title"><strong>title</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The &#039;title&#039; of this Collector.</td>
</tr>
<tr>
<th><a href="#viewer"><strong>viewer</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Instance of the Renderer service</td>
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
<th><a href="#formatTimelineData"><strong>formatTimelineData</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Child classes should implement this to return the timeline data
formatted for correct usage.</td>
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
protected $hasTimeline = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether this collector has data that can
be displayed in the Timeline.
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
Whether this collector needs to display
content in a tab or not.
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
Whether this collector has data that
should be shown in the Vars tab.
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
protected $title = 'Events';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The 'title' of this Collector.
</td></tr>
</table>

<table>
<tr><td>
Used to name things in the toolbar HTML.
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

#### $viewer

```php
protected $viewer;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instance of the Renderer service
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
Constructor.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (95 - 98)</small></summary>

```php
public function __construct()
{
	$this->viewer = Services::renderer();
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
Child classes should implement this to return the timeline data
formatted for correct usage.
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
<summary><small>Source: 18 lines (108 - 125)</small></summary>

```php
protected function formatTimelineData(): array
{
	$data = [];

	$rows = $this->viewer->getPerformanceData();

	foreach ($rows as $info)
	{
		$data[] = [
			'name'      => 'View: ' . $info['view'],
			'component' => 'Views',
			'start'     => $info['start'],
			'duration'  => $info['end'] - $info['start'],
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
<summary><small>Source: 27 lines (134 - 160)</small></summary>

```php
public function display(): array
{
	$data = [
		'events' => [],
	];

	foreach (\CodeIgniter\Events\Events::getPerformanceLogs() as $row)
	{
		$key = $row['event'];

		if (! array_key_exists($key, $data['events']))
		{
			$data['events'][$key] = [
				'event'    => $key,
				'duration' => number_format(($row['end'] - $row['start']) * 1000, 2),
				'count'    => 1,
			];

			continue;
		}

		$data['events'][$key]['duration'] += number_format(($row['end'] - $row['start']) * 1000, 2);
		$data['events'][$key]['count']++;
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
<summary><small>Source: 4 lines (169 - 172)</small></summary>

```php
public function getBadgeValue(): int
{
	return count(\CodeIgniter\Events\Events::getPerformanceLogs());
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
<summary><small>Source: 4 lines (183 - 186)</small></summary>

```php
public function icon(): string
{
	return 'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAEASURBVEhL7ZXNDcIwDIVTsRBH1uDQDdquUA6IM1xgCA6MwJUN2hk6AQzAz0vl0ETUxC5VT3zSU5w81/mRMGZysixbFEVR0jSKNt8geQU9aRpFmp/keX6AbjZ5oB74vsaN5lSzA4tLSjpBFxsjeSuRy4d2mDdQTWU7YLbXTNN05mKyovj5KL6B7q3hoy3KwdZxBlT+Ipz+jPHrBqOIynZgcZonoukb/0ckiTHqNvDXtXEAaygRbaB9FvUTjRUHsIYS0QaSp+Dw6wT4hiTmYHOcYZsdLQ2CbXa4ftuuYR4x9vYZgdb4vsFYUdmABMYeukK9/SUme3KMFQ77+Yfzh8eYF8+orDuDWU5LAAAAAElFTkSuQmCC';
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Toolbar/Collectors/Events.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Database.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Files.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>