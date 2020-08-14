


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Events/Events.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Entity.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/AlertError.md">next</a></td>
</tr>
</table>







# CodeIgniter\Events 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Events</td></tr>
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
<td>framework/system/Events/Events.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Events/Events.md">CodeIgniter\Events\Events</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
</table>



 
## CodeIgniter\Events\Events

<table style="text-align:left">
<tr><th>Class</th><td>Events</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Events\Events</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Events
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
<th><a href="#listeners"><strong>listeners</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>The list of listeners.</td>
</tr>
<tr>
<th><a href="#initialized"><strong>initialized</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Flag to let us know if we&#039;ve read from the Config file(s)
and have all of the defined events.</td>
</tr>
<tr>
<th><a href="#simulate"><strong>simulate</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>If true, events will not actually be fired.</td>
</tr>
<tr>
<th><a href="#performanceLog"><strong>performanceLog</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Stores information about the events
for display in the debug toolbar.</td>
</tr>
<tr>
<th><a href="#files"><strong>files</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>A list of found files.</td>
</tr>

<tr>
<th><a href="#initialize"><strong>initialize</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Ensures that we have a events file ready.</td>
</tr>
<tr>
<th><a href="#on"><strong>on</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Registers an action to happen on an event. The action can be any sort
of callable:</td>
</tr>
<tr>
<th><a href="#trigger"><strong>trigger</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Runs through all subscribed methods running them one at a time,
until either:
 a) All subscribers have finished or
 b) a method returns false, at which point execution of subscribers stops.</td>
</tr>
<tr>
<th><a href="#listeners"><strong>listeners</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns an array of listeners for a single event. They are
sorted by priority.</td>
</tr>
<tr>
<th><a href="#removeListener"><strong>removeListener</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Removes a single listener from an event.</td>
</tr>
<tr>
<th><a href="#removeAllListeners"><strong>removeAllListeners</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Removes all listeners.</td>
</tr>
<tr>
<th><a href="#setFiles"><strong>setFiles</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Sets the path to the file that routes are read from.</td>
</tr>
<tr>
<th><a href="#getFiles"><strong>getFiles</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the files that were found/loaded during this request.</td>
</tr>
<tr>
<th><a href="#simulate"><strong>simulate</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Turns simulation on or off. When on, events will not be triggered,
simply logged. Useful during testing when you don&#039;t actually want
the tests to run.</td>
</tr>
<tr>
<th><a href="#getPerformanceLogs"><strong>getPerformanceLogs</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Getter for the performance log records.</td>
</tr>

</table>





### Properties


<hr>

#### $listeners

```php
protected static $listeners = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The list of listeners.
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

#### $initialized

```php
protected static $initialized = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Flag to let us know if we've read from the Config file(s)
and have all of the defined events.
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

#### $simulate

```php
protected static $simulate = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
If true, events will not actually be fired.
</td></tr>
</table>

<table>
<tr><td>
Useful during testing.
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

#### $performanceLog

```php
protected static $performanceLog = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores information about the events
for display in the debug toolbar.
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

#### $files

```php
protected static $files = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A list of found files.
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

#### initialize()

```php
public static function initialize()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ensures that we have a events file ready.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 30 lines (97 - 126)</small></summary>

```php
public static function initialize()
{
	// Don't overwrite anything....
	if (static::$initialized)
	{
		return;
	}

	$config = config('Modules');

	$files = [APPPATH . 'Config/Events.php'];

	if ($config->shouldDiscover('events'))
	{
		$locator = Services::locator();
		$files   = $locator->search('Config/Events.php');
	}

	static::$files = $files;

	foreach (static::$files as $file)
	{
		if (is_file($file))
		{
			include $file;
		}
	}

	static::$initialized = true;
}
```

</details>


<hr>

#### on()

```php
public static function on($event_name, $callback, $priority = EVENT_PRIORITY_NORMAL)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Registers an action to happen on an event. The action can be any sort
of callable:
</td></tr>
</table>

<table>
<tr><td>
Events::on('create', 'myFunction');               // procedural function
Events::on('create', ['myClass', 'myMethod']);    // Class::method
Events::on('create', [$myInstance, 'myMethod']);  // Method on an existing instance
Events::on('create', function() });              // Closure
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
<td><code>$event_name</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$callback</code></td>
<td><em>callable
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$priority</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 17 lines (143 - 159)</small></summary>

```php
public static function on($event_name, $callback, $priority = EVENT_PRIORITY_NORMAL)
{
	if (! isset(static::$listeners[$event_name]))
	{
		static::$listeners[$event_name] = [
			true, // If there's only 1 item, it's sorted.
			[$priority],
			[$callback],
		];
	}
	else
	{
		static::$listeners[$event_name][0]   = false; // Not sorted
		static::$listeners[$event_name][1][] = $priority;
		static::$listeners[$event_name][2][] = $callback;
	}
}
```

</details>


<hr>

#### trigger()

```php
public static function trigger($eventName, ...$arguments) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs through all subscribed methods running them one at a time,
until either:
 a) All subscribers have finished or
 b) a method returns false, at which point execution of subscribers stops.
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
<td><code>$eventName</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$arguments</code></td>
<td><em>
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
<summary><small>Source: 33 lines (174 - 206)</small></summary>

```php
public static function trigger($eventName, ...$arguments): bool
{
	// Read in our Config/events file so that we have them all!
	if (! static::$initialized)
	{
		static::initialize();
	}

	$listeners = static::listeners($eventName);

	foreach ($listeners as $listener)
	{
		$start = microtime(true);

		$result = static::$simulate === false ? call_user_func($listener, ...$arguments) : true;

		if (CI_DEBUG)
		{
			static::$performanceLog[] = [
				'start' => $start,
				'end'   => microtime(true),
				'event' => strtolower($eventName),
			];
		}

		if ($result === false)
		{
			return false;
		}
	}

	return true;
}
```

</details>


<hr>

#### listeners()

```php
public static function listeners($event_name) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array of listeners for a single event. They are
sorted by priority.
</td></tr>
</table>

<table>
<tr><td>
If the listener could not be found, returns FALSE, or TRUE if
it was removed.
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
<td><code>$event_name</code></td>
<td><em>
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
<summary><small>Source: 19 lines (221 - 239)</small></summary>

```php
public static function listeners($event_name): array
{
	if (! isset(static::$listeners[$event_name]))
	{
		return [];
	}

	// The list is not sorted
	if (! static::$listeners[$event_name][0])
	{
		// Sort it!
		array_multisort(static::$listeners[$event_name][1], SORT_NUMERIC, static::$listeners[$event_name][2]);

		// Mark it as sorted already!
		static::$listeners[$event_name][0] = true;
	}

	return static::$listeners[$event_name][2];
}
```

</details>


<hr>

#### removeListener()

```php
public static function removeListener($event_name, callable $listener) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes a single listener from an event.
</td></tr>
</table>

<table>
<tr><td>
If the listener couldn't be found, returns FALSE, else TRUE if
it was removed.
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
<td><code>$event_name</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$listener</code></td>
<td><em>callable
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
<summary><small>Source: 20 lines (254 - 273)</small></summary>

```php
public static function removeListener($event_name, callable $listener): bool
{
	if (! isset(static::$listeners[$event_name]))
	{
		return false;
	}

	foreach (static::$listeners[$event_name][2] as $index => $check)
	{
		if ($check === $listener)
		{
			unset(static::$listeners[$event_name][1][$index]);
			unset(static::$listeners[$event_name][2][$index]);

			return true;
		}
	}

	return false;
}
```

</details>


<hr>

#### removeAllListeners()

```php
public static function removeAllListeners($event_name = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes all listeners.
</td></tr>
</table>

<table>
<tr><td>
If the event_name is specified, only listeners for that event will be
removed, otherwise all listeners for all events are removed.
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
<td><code>$event_name</code></td>
<td><em>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 11 lines (285 - 295)</small></summary>

```php
public static function removeAllListeners($event_name = null)
{
	if (! is_null($event_name))
	{
		unset(static::$listeners[$event_name]);
	}
	else
	{
		static::$listeners = [];
	}
}
```

</details>


<hr>

#### setFiles()

```php
public static function setFiles(array $files)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the path to the file that routes are read from.
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
<td><code>$files</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (304 - 307)</small></summary>

```php
public static function setFiles(array $files)
{
	static::$files = $files;
}
```

</details>


<hr>

#### getFiles()

```php
public function getFiles()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the files that were found/loaded during this request.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (316 - 319)</small></summary>

```php
public function getFiles()
{
	return static::$files;
}
```

</details>


<hr>

#### simulate()

```php
public static function simulate(bool $choice = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Turns simulation on or off. When on, events will not be triggered,
simply logged. Useful during testing when you don't actually want
the tests to run.
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
<td><code>$choice</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (330 - 333)</small></summary>

```php
public static function simulate(bool $choice = true)
{
	static::$simulate = $choice;
}
```

</details>


<hr>

#### getPerformanceLogs()

```php
public static function getPerformanceLogs()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Getter for the performance log records.
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
<summary><small>Source: 4 lines (342 - 345)</small></summary>

```php
public static function getPerformanceLogs()
{
	return static::$performanceLog;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Events/Events.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Entity.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/AlertError.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>