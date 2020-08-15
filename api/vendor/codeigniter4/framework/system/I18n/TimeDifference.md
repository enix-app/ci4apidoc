


 



<table>
<tr>
<td style="width:100%"><em>framework/system/I18n/TimeDifference.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Time.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Exceptions/ImageException.md">next</a></td>
</tr>
</table>







# CodeIgniter\I18n 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\I18n</td></tr>
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
<td><a href="https://opensource.org/licenses/MIT">https://opensource.org/licenses/MIT</a>    MIT License
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com">https://codeigniter.com</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>filesource</th>
<td>framework/system/I18n/TimeDifference.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Exceptions/I18nException.md">CodeIgniter\I18n\Exceptions\I18nException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Time.md">CodeIgniter\I18n\Time</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/TimeDifference.md">CodeIgniter\I18n\TimeDifference</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>DateTime</strong>
</td>
<td>DateTime</td>
</tr>
<tr>
<td>
<strong>IntlCalendar</strong>
</td>
<td>IntlCalendar</td>
</tr>
</table>



 
## CodeIgniter\I18n\TimeDifference

<table style="text-align:left">
<tr><th>Class</th><td>TimeDifference</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\I18n\TimeDifference</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class TimeDifference
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\I18n
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
<th><a href="#currentTime"><strong>currentTime</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The timestamp of the &quot;current&quot; time.</td>
</tr>
<tr>
<th><a href="#testTime"><strong>testTime</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The timestamp to compare the current time to.</td>
</tr>
<tr>
<th><a href="#eras"><strong>eras</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Eras.</td>
</tr>
<tr>
<th><a href="#years"><strong>years</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Years.</td>
</tr>
<tr>
<th><a href="#months"><strong>months</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Months.</td>
</tr>
<tr>
<th><a href="#weeks"><strong>weeks</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Weeks.</td>
</tr>
<tr>
<th><a href="#days"><strong>days</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Days.</td>
</tr>
<tr>
<th><a href="#hours"><strong>hours</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Hours.</td>
</tr>
<tr>
<th><a href="#minutes"><strong>minutes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Minutes.</td>
</tr>
<tr>
<th><a href="#seconds"><strong>seconds</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Seconds.</td>
</tr>
<tr>
<th><a href="#difference"><strong>difference</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Difference in seconds.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Note: both parameters are required to be in the same timezone. No timezone
shifting is done internally.</td>
</tr>
<tr>
<th><a href="#getYears"><strong>getYears</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of years of difference between the two.</td>
</tr>
<tr>
<th><a href="#getMonths"><strong>getMonths</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of months difference between the two dates.</td>
</tr>
<tr>
<th><a href="#getWeeks"><strong>getWeeks</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of weeks difference between the two dates.</td>
</tr>
<tr>
<th><a href="#getDays"><strong>getDays</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of days difference between the two dates.</td>
</tr>
<tr>
<th><a href="#getHours"><strong>getHours</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of hours difference between the two dates.</td>
</tr>
<tr>
<th><a href="#getMinutes"><strong>getMinutes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of minutes difference between the two dates.</td>
</tr>
<tr>
<th><a href="#getSeconds"><strong>getSeconds</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of seconds difference between the two dates.</td>
</tr>
<tr>
<th><a href="#humanize"><strong>humanize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Convert the time to human readable format</td>
</tr>
<tr>
<th><a href="#__get"><strong>__get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allow property-like access to our calculated values.</td>
</tr>
<tr>
<th><a href="#__isset"><strong>__isset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allow property-like checking for our calculated values.</td>
</tr>

</table>





### Properties


<hr>

#### $currentTime

```php
protected $currentTime;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The timestamp of the "current" time.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\IntlCalendar
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
The timestamp to compare the current time to.
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

#### $eras

```php
protected $eras = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Eras.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>float
</td>
</tr>
</table>


<hr>

#### $years

```php
protected $years = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Years.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>float
</td>
</tr>
</table>


<hr>

#### $months

```php
protected $months = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Months.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>float
</td>
</tr>
</table>


<hr>

#### $weeks

```php
protected $weeks = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Weeks.
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

#### $days

```php
protected $days = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Days.
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

#### $hours

```php
protected $hours = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Hours.
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

#### $minutes

```php
protected $minutes = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Minutes.
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

#### $seconds

```php
protected $seconds = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Seconds.
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

#### $difference

```php
protected $difference;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Difference in seconds.
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
public function __construct(DateTime $currentTime, DateTime $testTime)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Note: both parameters are required to be in the same timezone. No timezone
shifting is done internally.
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
<td><code>$currentTime</code></td>
<td><em>\DateTime
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$testTime</code></td>
<td><em>\DateTime
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 11 lines (130 - 140)</small></summary>

```php
public function __construct(DateTime $currentTime, DateTime $testTime)
{
	$this->difference = $currentTime->getTimestamp() - $testTime->getTimestamp();

	$current = IntlCalendar::fromDateTime($currentTime->format('Y-m-d H:i:s'));
	$time    = IntlCalendar::fromDateTime($testTime->format('Y-m-d H:i:s'))
					->getTime();

	$this->currentTime = $current;
	$this->testTime    = $time;
}
```

</details>


<hr>

#### getYears()

```php
public function getYears(bool $raw = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of years of difference between the two.
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
<td><code>$raw</code></td>
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
<td>float<br>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (151 - 160)</small></summary>

```php
public function getYears(bool $raw = false)
{
	if ($raw)
	{
		return $this->difference / YEAR;
	}

	$time = clone($this->currentTime);
	return $time->fieldDifference($this->testTime, IntlCalendar::FIELD_YEAR);
}
```

</details>


<hr>

#### getMonths()

```php
public function getMonths(bool $raw = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of months difference between the two dates.
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
<td><code>$raw</code></td>
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
<td>float<br>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (169 - 178)</small></summary>

```php
public function getMonths(bool $raw = false)
{
	if ($raw)
	{
		return $this->difference / MONTH;
	}

	$time = clone($this->currentTime);
	return $time->fieldDifference($this->testTime, IntlCalendar::FIELD_MONTH);
}
```

</details>


<hr>

#### getWeeks()

```php
public function getWeeks(bool $raw = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of weeks difference between the two dates.
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
<td><code>$raw</code></td>
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
<td>float<br>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (187 - 196)</small></summary>

```php
public function getWeeks(bool $raw = false)
{
	if ($raw)
	{
		return $this->difference / WEEK;
	}

	$time = clone($this->currentTime);
	return (int)($time->fieldDifference($this->testTime, IntlCalendar::FIELD_DAY_OF_YEAR) / 7);
}
```

</details>


<hr>

#### getDays()

```php
public function getDays(bool $raw = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of days difference between the two dates.
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
<td><code>$raw</code></td>
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
<td>float<br>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (205 - 214)</small></summary>

```php
public function getDays(bool $raw = false)
{
	if ($raw)
	{
		return $this->difference / DAY;
	}

	$time = clone($this->currentTime);
	return $time->fieldDifference($this->testTime, IntlCalendar::FIELD_DAY_OF_YEAR);
}
```

</details>


<hr>

#### getHours()

```php
public function getHours(bool $raw = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of hours difference between the two dates.
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
<td><code>$raw</code></td>
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
<td>float<br>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (223 - 232)</small></summary>

```php
public function getHours(bool $raw = false)
{
	if ($raw)
	{
		return $this->difference / HOUR;
	}

	$time = clone($this->currentTime);
	return $time->fieldDifference($this->testTime, IntlCalendar::FIELD_HOUR_OF_DAY);
}
```

</details>


<hr>

#### getMinutes()

```php
public function getMinutes(bool $raw = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of minutes difference between the two dates.
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
<td><code>$raw</code></td>
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
<td>float<br>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (241 - 250)</small></summary>

```php
public function getMinutes(bool $raw = false)
{
	if ($raw)
	{
		return $this->difference / MINUTE;
	}

	$time = clone($this->currentTime);
	return $time->fieldDifference($this->testTime, IntlCalendar::FIELD_MINUTE);
}
```

</details>


<hr>

#### getSeconds()

```php
public function getSeconds(bool $raw = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of seconds difference between the two dates.
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
<td><code>$raw</code></td>
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
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (259 - 268)</small></summary>

```php
public function getSeconds(bool $raw = false)
{
	if ($raw)
	{
		return $this->difference;
	}

	$time = clone($this->currentTime);
	return $time->fieldDifference($this->testTime, IntlCalendar::FIELD_SECOND);
}
```

</details>


<hr>

#### humanize()

```php
public function humanize(string $locale = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Convert the time to human readable format
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
<td><code>$locale</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 52 lines (277 - 328)</small></summary>

```php
public function humanize(string $locale = null): string
{
	$current = clone($this->currentTime);

	$years   = $current->fieldDifference($this->testTime, IntlCalendar::FIELD_YEAR);
	$months  = $current->fieldDifference($this->testTime, IntlCalendar::FIELD_MONTH);
	$days    = $current->fieldDifference($this->testTime, IntlCalendar::FIELD_DAY_OF_YEAR);
	$hours   = $current->fieldDifference($this->testTime, IntlCalendar::FIELD_HOUR_OF_DAY);
	$minutes = $current->fieldDifference($this->testTime, IntlCalendar::FIELD_MINUTE);

	$phrase = null;

	if ($years !== 0)
	{
		$phrase = lang('Time.years', [abs($years)], $locale);
		$before = $years < 0;
	}
	elseif ($months !== 0)
	{
		$phrase = lang('Time.months', [abs($months)], $locale);
		$before = $months < 0;
	}
	elseif ($days !== 0 && (abs($days) >= 7))
	{
		$weeks  = ceil($days / 7);
		$phrase = lang('Time.weeks', [abs($weeks)], $locale);
		$before = $days < 0;
	}
	elseif ($days !== 0)
	{
		$phrase = lang('Time.days', [abs($days)], $locale);
		$before = $days < 0;
	}
	elseif ($hours !== 0)
	{
		$phrase = lang('Time.hours', [abs($hours)], $locale);
		$before = $hours < 0;
	}
	elseif ($minutes !== 0)
	{
		$phrase = lang('Time.minutes', [abs($minutes)], $locale);
		$before = $minutes < 0;
	}
	else
	{
		return lang('Time.now', [], $locale);
	}

	return $before
		? lang('Time.ago', [$phrase], $locale)
		: lang('Time.inFuture', [$phrase], $locale);
}
```

</details>


<hr>

#### __get()

```php
public function __get($name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allow property-like access to our calculated values.
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 12 lines (337 - 348)</small></summary>

```php
public function __get($name)
{
	$name   = ucfirst(strtolower($name));
	$method = "get{$name}";

	if (method_exists($this, $method))
	{
		return $this->{$method}($name);
	}

	return null;
}
```

</details>


<hr>

#### __isset()

```php
public function __isset($name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allow property-like checking for our calculated values.
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
<summary><small>Source: 7 lines (357 - 363)</small></summary>

```php
public function __isset($name)
{
	$name   = ucfirst(strtolower($name));
	$method = "get{$name}";

	return method_exists($this, $method);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/I18n/TimeDifference.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Time.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Exceptions/ImageException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>