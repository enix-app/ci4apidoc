


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Timer.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Iterator.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar.md">next</a></td>
</tr>
</table>







# CodeIgniter\Debug 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Debug</td></tr>
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
<td>framework/system/Debug/Timer.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Exceptions.md">CodeIgniter\Debug\Exceptions</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Iterator.md">CodeIgniter\Debug\Iterator</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Timer.md">CodeIgniter\Debug\Timer</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar.md">CodeIgniter\Debug\Toolbar</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/BaseCollector.md">CodeIgniter\Debug\Toolbar\Collectors\BaseCollector</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Config.md">CodeIgniter\Debug\Toolbar\Collectors\Config</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Database.md">CodeIgniter\Debug\Toolbar\Collectors\Database</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Events.md">CodeIgniter\Debug\Toolbar\Collectors\Events</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Files.md">CodeIgniter\Debug\Toolbar\Collectors\Files</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/History.md">CodeIgniter\Debug\Toolbar\Collectors\History</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Logs.md">CodeIgniter\Debug\Toolbar\Collectors\Logs</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Routes.md">CodeIgniter\Debug\Toolbar\Collectors\Routes</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Timers.md">CodeIgniter\Debug\Toolbar\Collectors\Timers</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Views.md">CodeIgniter\Debug\Toolbar\Collectors\Views</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Debug\Timer

<table style="text-align:left">
<tr><th>Class</th><td>Timer</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Debug\Timer</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Timer
</td></tr>
</table>

<table>
<tr><td>
Provides a simple way to measure the amount of time
that elapses between two points.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Debug
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
<th><a href="#timers"><strong>timers</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>List of all timers.</td>
</tr>

<tr>
<th><a href="#start"><strong>start</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Starts a timer running.</td>
</tr>
<tr>
<th><a href="#stop"><strong>stop</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Stops a running timer.</td>
</tr>
<tr>
<th><a href="#getElapsedTime"><strong>getElapsedTime</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the duration of a recorded timer.</td>
</tr>
<tr>
<th><a href="#getTimers"><strong>getTimers</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the array of timers, with the duration pre-calculated for you.</td>
</tr>
<tr>
<th><a href="#has"><strong>has</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks whether or not a timer with the specified name exists.</td>
</tr>

</table>





### Properties


<hr>

#### $timers

```php
protected $timers = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
List of all timers.
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

#### start()

```php
public function start(string $name, float $time = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Starts a timer running.
</td></tr>
</table>

<table>
<tr><td>
Multiple calls can be made to this method so that several
execution points can be measured.
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
<td>The name of this timer.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$time</code></td>
<td><em>float
</em></td>
<td>false</td>
<td>Allows user to provide time.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Timer
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (73 - 81)</small></summary>

```php
public function start(string $name, float $time = null)
{
	$this->timers[strtolower($name)] = [
		'start' => ! empty($time) ? $time : microtime(true),
		'end'   => null,
	];

	return $this;
}
```

</details>


<hr>

#### stop()

```php
public function stop(string $name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stops a running timer.
</td></tr>
</table>

<table>
<tr><td>
If the timer is not stopped before the timers() method is called,
it will be automatically stopped at that point.
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
<td>The name of this timer.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Timer
</td>
</tr>
</table>





<details>
<summary><small>Source: 13 lines (95 - 107)</small></summary>

```php
public function stop(string $name)
{
	$name = strtolower($name);

	if (empty($this->timers[$name]))
	{
		throw new \RuntimeException('Cannot stop timer: invalid name given.');
	}

	$this->timers[$name]['end'] = microtime(true);

	return $this;
}
```

</details>


<hr>

#### getElapsedTime()

```php
public function getElapsedTime(string $name, int $decimals = 4)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the duration of a recorded timer.
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
<td>The name of the timer.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$decimals</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Number of decimal places.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>null<br>float
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (121 - 138)</small></summary>

```php
public function getElapsedTime(string $name, int $decimals = 4)
{
	$name = strtolower($name);

	if (empty($this->timers[$name]))
	{
		return null;
	}

	$timer = $this->timers[$name];

	if (empty($timer['end']))
	{
		$timer['end'] = microtime(true);
	}

	return (float) number_format($timer['end'] - $timer['start'], $decimals);
}
```

</details>


<hr>

#### getTimers()

```php
public function getTimers(int $decimals = 4) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the array of timers, with the duration pre-calculated for you.
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
<td><code>$decimals</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Number of decimal places</td>
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
<summary><small>Source: 16 lines (149 - 164)</small></summary>

```php
public function getTimers(int $decimals = 4): array
{
	$timers = $this->timers;

	foreach ($timers as &$timer)
	{
		if (empty($timer['end']))
		{
			$timer['end'] = microtime(true);
		}

		$timer['duration'] = (float) number_format($timer['end'] - $timer['start'], $decimals);
	}

	return $timers;
}
```

</details>


<hr>

#### has()

```php
public function has(string $name) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks whether or not a timer with the specified name exists.
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
<summary><small>Source: 4 lines (175 - 178)</small></summary>

```php
public function has(string $name): bool
{
	return array_key_exists(strtolower($name), $this->timers);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Timer.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Iterator.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>