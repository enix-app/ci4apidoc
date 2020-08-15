


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Iterator.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Exceptions.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Timer.md">next</a></td>
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
<td>framework/system/Debug/Iterator.php
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



 

 
## CodeIgniter\Debug\Iterator

<table style="text-align:left">
<tr><th>Class</th><td>Iterator</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Debug\Iterator</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Iterator for debugging.
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
<th><a href="#tests"><strong>tests</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores the tests that we are to run.</td>
</tr>
<tr>
<th><a href="#results"><strong>results</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores the results of each of the tests.</td>
</tr>

<tr>
<th><a href="#add"><strong>add</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Adds a test to run.</td>
</tr>
<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runs through all of the tests that have been added, recording
time to execute the desired number of iterations, and the approximate
memory usage used during those iterations.</td>
</tr>
<tr>
<th><a href="#getReport"><strong>getReport</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get results.</td>
</tr>

</table>





### Properties


<hr>

#### $tests

```php
protected $tests = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the tests that we are to run.
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

#### $results

```php
protected $results = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the results of each of the tests.
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

#### add()

```php
public function add(string $name, \Closure $closure)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Adds a test to run.
</td></tr>
</table>

<table>
<tr><td>
Tests are simply closures that the user can define any sequence of
things to happen during the test.
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
<td><code>$closure</code></td>
<td><em>\Closure
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
<summary><small>Source: 8 lines (74 - 81)</small></summary>

```php
public function add(string $name, \Closure $closure)
{
	$name = strtolower($name);

	$this->tests[$name] = $closure;

	return $this;
}
```

</details>


<hr>

#### run()

```php
public function run(int $iterations = 1000, bool $output = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs through all of the tests that have been added, recording
time to execute the desired number of iterations, and the approximate
memory usage used during those iterations.
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
<td><code>$iterations</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$output</code></td>
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
<summary><small>Source: 33 lines (95 - 127)</small></summary>

```php
public function run(int $iterations = 1000, bool $output = true)
{
	foreach ($this->tests as $name => $test)
	{
		// clear memory before start
		gc_collect_cycles();

		$start     = microtime(true);
		$start_mem = $max_memory = memory_get_usage(true);

		for ($i = 0; $i < $iterations; $i ++)
		{
			$result = $test();

			$max_memory = max($max_memory, memory_get_usage(true));

			unset($result);
		}

		$this->results[$name] = [
			'time'   => microtime(true) - $start,
			'memory' => $max_memory - $start_mem,
			'n'      => $iterations,
		];
	}

	if ($output)
	{
		return $this->getReport();
	}

	return null;
}
```

</details>


<hr>

#### getReport()

```php
public function getReport() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get results.
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
<summary><small>Source: 40 lines (136 - 175)</small></summary>

```php
public function getReport(): string
{
	if (empty($this->results))
	{
		return 'No results to display.';
	}

	helper('number');

	// Template
	$tpl = '<table>
		<thead>
			<tr>
				<td>Test</td>
				<td>Time</td>
				<td>Memory</td>
			</tr>
		</thead>
		<tbody>
			{rows}
		</tbody>
	</table>';

	$rows = '';

	foreach ($this->results as $name => $result)
	{
		$memory = number_to_size($result['memory'], 4);

		$rows .= "<tr>
			<td>{$name}</td>
			<td>" . number_format($result['time'], 4) . "</td>
			<td>{$memory}</td>
		</tr>";
	}

	$tpl = str_replace('{rows}', $rows, $tpl);

	return $tpl . '<br/>';
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Debug/Iterator.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Exceptions.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Timer.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>