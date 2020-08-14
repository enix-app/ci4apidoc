


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Toolbar/Collectors/BaseCollector.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Config.md">next</a></td>
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
<td>framework/system/Debug/Toolbar/Collectors/BaseCollector.php
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
<a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Exceptions.md"><strong>CodeIgniter\Debug\Exceptions</strong></a>
</td>
<td>Exceptions</td>
</tr>
</table>



 
## CodeIgniter\Debug\Toolbar\Collectors\BaseCollector

<table style="text-align:left">
<tr><th>Class</th><td>BaseCollector</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Debug\Toolbar\Collectors\BaseCollector</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Base Toolbar collector
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
<th><a href="#hasLabel"><strong>hasLabel</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether this collector needs to display
a label or not.</td>
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
<th><a href="#getTitle"><strong>getTitle</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Gets the Collector&#039;s title.</td>
</tr>
<tr>
<th><a href="#getTitleDetails"><strong>getTitleDetails</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns any information that should be shown next to the title.</td>
</tr>
<tr>
<th><a href="#hasTabContent"><strong>hasTabContent</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Does this collector need it&#039;s own tab?</td>
</tr>
<tr>
<th><a href="#hasLabel"><strong>hasLabel</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Does this collector have a label?</td>
</tr>
<tr>
<th><a href="#hasTimelineData"><strong>hasTimelineData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Does this collector have information for the timeline?</td>
</tr>
<tr>
<th><a href="#timelineData"><strong>timelineData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Grabs the data for the timeline, properly formatted,
or returns an empty array.</td>
</tr>
<tr>
<th><a href="#hasVarData"><strong>hasVarData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Does this Collector have data that should be shown in the
&#039;Vars&#039; tab?</td>
</tr>
<tr>
<th><a href="#getVarData"><strong>getVarData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Gets a collection of data that should be shown in the &#039;Vars&#039; tab.</td>
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
<th><a href="#cleanPath"><strong>cleanPath</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Clean Path</td>
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
<td>Returns the HTML to display the icon. Should either
be SVG, or a base-64 encoded.</td>
</tr>
<tr>
<th><a href="#getAsArray"><strong>getAsArray</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return settings as an array.</td>
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
protected $hasTabContent = false;
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

#### $hasLabel

```php
protected $hasLabel = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether this collector needs to display
a label or not.
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
protected $title = '';
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







### Methods


<hr>

#### getTitle()

```php
public function getTitle(bool $safe = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets the Collector's title.
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
<td><code>$safe</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (97 - 105)</small></summary>

```php
public function getTitle(bool $safe = false): string
{
	if ($safe)
	{
		return str_replace(' ', '-', strtolower($this->title));
	}

	return $this->title;
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
Returns any information that should be shown next to the title.
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
<summary><small>Source: 4 lines (114 - 117)</small></summary>

```php
public function getTitleDetails(): string
{
	return '';
}
```

</details>


<hr>

#### hasTabContent()

```php
public function hasTabContent() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does this collector need it's own tab?
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
<summary><small>Source: 4 lines (126 - 129)</small></summary>

```php
public function hasTabContent(): bool
{
	return (bool) $this->hasTabContent;
}
```

</details>


<hr>

#### hasLabel()

```php
public function hasLabel() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does this collector have a label?
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
<summary><small>Source: 4 lines (138 - 141)</small></summary>

```php
public function hasLabel(): bool
{
	return (bool) $this->hasLabel;
}
```

</details>


<hr>

#### hasTimelineData()

```php
public function hasTimelineData() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does this collector have information for the timeline?
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
<summary><small>Source: 4 lines (150 - 153)</small></summary>

```php
public function hasTimelineData(): bool
{
	return (bool) $this->hasTimeline;
}
```

</details>


<hr>

#### timelineData()

```php
public function timelineData() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Grabs the data for the timeline, properly formatted,
or returns an empty array.
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
<summary><small>Source: 9 lines (163 - 171)</small></summary>

```php
public function timelineData(): array
{
	if (! $this->hasTimeline)
	{
		return [];
	}

	return $this->formatTimelineData();
}
```

</details>


<hr>

#### hasVarData()

```php
public function hasVarData() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does this Collector have data that should be shown in the
'Vars' tab?
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
<summary><small>Source: 4 lines (181 - 184)</small></summary>

```php
public function hasVarData(): bool
{
	return (bool) $this->hasVarData;
}
```

</details>


<hr>

#### getVarData()

```php
public function getVarData()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets a collection of data that should be shown in the 'Vars' tab.
</td></tr>
</table>

<table>
<tr><td>
The format is an array of sections, each with their own array
of key/value pairs:

 $data = [
     'section 1' => [
         'foo' => 'bar,
         'bar' => 'baz'
     ],
     'section 2' => [
         'foo' => 'bar,
         'bar' => 'baz'
     ],
 ];
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (206 - 209)</small></summary>

```php
public function getVarData()
{
	return null;
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

<table>
<tr><td>
Timeline data should be formatted into arrays that look like:

[
    'name'      => 'Database::Query',
    'component' => 'Database',
    'start'     => 10       // milliseconds
    'duration'  => 15       // milliseconds
]
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
<summary><small>Source: 4 lines (228 - 231)</small></summary>

```php
protected function formatTimelineData(): array
{
	return [];
}
```

</details>


<hr>

#### display()

```php
public function display()
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
<td>array<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (240 - 243)</small></summary>

```php
public function display()
{
	return [];
}
```

</details>


<hr>

#### cleanPath()

```php
public function cleanPath(string $file) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Clean Path
</td></tr>
</table>

<table>
<tr><td>
This makes nicer looking paths for the error output.
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
<td><code>$file</code></td>
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
<summary><small>Source: 4 lines (256 - 259)</small></summary>

```php
public function cleanPath(string $file): string
{
	return Exceptions::cleanPath($file);
}
```

</details>


<hr>

#### getBadgeValue()

```php
public function getBadgeValue()
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
<td>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (266 - 269)</small></summary>

```php
public function getBadgeValue()
{
	return null;
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

<table>
<tr><td>
If not, then the toolbar button won't get shown.
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
<summary><small>Source: 4 lines (278 - 281)</small></summary>

```php
public function isEmpty(): bool
{
	return false;
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
Returns the HTML to display the icon. Should either
be SVG, or a base-64 encoded.
</td></tr>
</table>

<table>
<tr><td>
Recommended dimensions are 24px x 24px
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
<summary><small>Source: 4 lines (291 - 294)</small></summary>

```php
public function icon(): string
{
	return '';
}
```

</details>


<hr>

#### getAsArray()

```php
public function getAsArray() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return settings as an array.
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
<summary><small>Source: 16 lines (301 - 316)</small></summary>

```php
public function getAsArray(): array
{
	return [
		'title'           => $this->getTitle(),
		'titleSafe'       => $this->getTitle(true),
		'titleDetails'    => $this->getTitleDetails(),
		'display'         => $this->display(),
		'badgeValue'      => $this->getBadgeValue(),
		'isEmpty'         => $this->isEmpty(),
		'hasTabContent'   => $this->hasTabContent(),
		'hasLabel'        => $this->hasLabel(),
		'icon'            => $this->icon(),
		'hasTimelineData' => $this->hasTimelineData(),
		'timelineData'    => $this->timelineData(),
	];
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Toolbar/Collectors/BaseCollector.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Config.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>