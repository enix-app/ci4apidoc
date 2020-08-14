


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Throttle/Throttler.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Test/TestLogger.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/ThrottlerInterface.md">next</a></td>
</tr>
</table>







# CodeIgniter\Throttle 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Throttle</td></tr>
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
<td>framework/system/Throttle/Throttler.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/Throttler.md">CodeIgniter\Throttle\Throttler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/ThrottlerInterface.md">CodeIgniter\Throttle\ThrottlerInterface</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md"><strong>CodeIgniter\Cache\CacheInterface</strong></a>
</td>
<td>CacheInterface</td>
</tr>
</table>



 
## CodeIgniter\Throttle\Throttler

<table style="text-align:left">
<tr><th>Class</th><td>Throttler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Throttle\Throttler</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/ThrottlerInterface.md">CodeIgniter\Throttle\ThrottlerInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Throttler
</td></tr>
</table>

<table>
<tr><td>
Uses an implementation of the Token Bucket algorithm to implement a
"rolling window" type of throttling that can be used for rate limiting
an API or any other request.

Each "token" in the "bucket" is equivalent to a single request
for the purposes of this implementation.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Throttle
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
<th><a href="#cache"><strong>cache</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Container for throttle counters.</td>
</tr>
<tr>
<th><a href="#tokenTime"><strong>tokenTime</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The number of seconds until the next token is available.</td>
</tr>
<tr>
<th><a href="#prefix"><strong>prefix</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The prefix applied to all keys to
minimize potential conflicts.</td>
</tr>
<tr>
<th><a href="#testTime"><strong>testTime</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Timestamp to use (during testing)</td>
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
<th><a href="#getTokenTime"><strong>getTokenTime</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of seconds until the next available token will
be released for usage.</td>
</tr>
<tr>
<th><a href="#check"><strong>check</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Restricts the number of requests made by a single IP address within
a set number of seconds.</td>
</tr>
<tr>
<th><a href="#setTestTime"><strong>setTestTime</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used during testing to set the current timestamp to use.</td>
</tr>
<tr>
<th><a href="#time"><strong>time</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the test time, defaulting to current.</td>
</tr>

</table>





### Properties


<hr>

#### $cache

```php
protected $cache;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Container for throttle counters.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Cache\CacheInterface
</td>
</tr>
</table>


<hr>

#### $tokenTime

```php
protected $tokenTime = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The number of seconds until the next token is available.
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

#### $prefix

```php
protected $prefix = 'throttler_';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The prefix applied to all keys to
minimize potential conflicts.
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

#### $testTime

```php
protected $testTime;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Timestamp to use (during testing)
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
public function __construct(CacheInterface $cache)
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
<td><code>$cache</code></td>
<td><em>\type
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\type
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (98 - 101)</small></summary>

```php
public function __construct(CacheInterface $cache)
{
	$this->cache = $cache;
}
```

</details>


<hr>

#### getTokenTime()

```php
public function getTokenTime() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of seconds until the next available token will
be released for usage.
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
<summary><small>Source: 4 lines (111 - 114)</small></summary>

```php
public function getTokenTime(): int
{
	return $this->tokenTime;
}
```

</details>


<hr>

#### check()

```php
public function check(string $key, int $capacity, int $seconds, int $cost = 1) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Restricts the number of requests made by a single IP address within
a set number of seconds.
</td></tr>
</table>

<table>
<tr><td>
Example:

 if (! $throttler->check($request->ipAddress(), 60, MINUTE))
{
     die('You submitted over 60 requests within a minute.');
}
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>internal</th>
<td>param int $maxRequests
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
<td><code>$key</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The name to use as the "bucket" name.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$capacity</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The number of requests the "bucket" can hold</td>
</tr>

<tr>
<td>3.</td>
<td><code>$seconds</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The time it takes the "bucket" to completely refill</td>
</tr>

<tr>
<td>4.</td>
<td><code>$cost</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The number of tokens this action uses.</td>
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
<summary><small>Source: 47 lines (137 - 183)</small></summary>

```php
public function check(string $key, int $capacity, int $seconds, int $cost = 1): bool
{
	$tokenName = $this->prefix . $key;

	// Check to see if the bucket has even been created yet.
	if (($tokens = $this->cache->get($tokenName)) === null)
	{
		// If it hasn't been created, then we'll set it to the maximum
		// capacity - 1, and save it to the cache.
		$this->cache->save($tokenName, $capacity - $cost, $seconds);
		$this->cache->save($tokenName . 'Time', time(), $seconds);

		return true;
	}

	// If $tokens > 0, then we need to replenish the bucket
	// based on how long it's been since the last update.
	$throttleTime = $this->cache->get($tokenName . 'Time');
	$elapsed      = $this->time() - $throttleTime;

	// Number of tokens to add back per second
	$rate = $capacity / $seconds;

	// How many seconds till a new token is available.
	// We must have a minimum wait of 1 second for a new token.
	// Primarily stored to allow devs to report back to users.
	$newTokenAvailable = (1 / $rate) - $elapsed;
	$this->tokenTime   = max(1, $newTokenAvailable);

	// Add tokens based up on number per second that
	// should be refilled, then checked against capacity
	// to be sure the bucket didn't overflow.
	$tokens += $rate * $elapsed;
	$tokens  = $tokens > $capacity ? $capacity : $tokens;

	// If $tokens >= 1, then we are safe to perform the action, but
	// we need to decrement the number of available tokens.
	if ($tokens >= 1)
	{
		$this->cache->save($tokenName, $tokens - $cost, $seconds);
		$this->cache->save($tokenName . 'Time', time(), $seconds);

		return true;
	}

	return false;
}
```

</details>


<hr>

#### setTestTime()

```php
public function setTestTime(int $time)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used during testing to set the current timestamp to use.
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
<td><code>$time</code></td>
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
<summary><small>Source: 6 lines (194 - 199)</small></summary>

```php
public function setTestTime(int $time)
{
	$this->testTime = $time;

	return $this;
}
```

</details>


<hr>

#### time()

```php
public function time() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the test time, defaulting to current.
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
<summary><small>Source: 4 lines (208 - 211)</small></summary>

```php
public function time(): int
{
	return $this->testTime ?? time();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Throttle/Throttler.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Test/TestLogger.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/ThrottlerInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>