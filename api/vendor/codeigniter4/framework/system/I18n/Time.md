


 



<table>
<tr>
<td style="width:100%"><em>framework/system/I18n/Time.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Exceptions/I18nException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/TimeDifference.md">next</a></td>
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
<td>framework/system/I18n/Time.php
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
<a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Exceptions/I18nException.md"><strong>CodeIgniter\I18n\Exceptions\I18nException</strong></a>
</td>
<td>I18nException</td>
</tr>
<tr>
<td>
<strong>DateInterval</strong>
</td>
<td>DateInterval</td>
</tr>
<tr>
<td>
<strong>DateTime</strong>
</td>
<td>DateTime</td>
</tr>
<tr>
<td>
<strong>DateTimeZone</strong>
</td>
<td>DateTimeZone</td>
</tr>
<tr>
<td>
<strong>IntlCalendar</strong>
</td>
<td>IntlCalendar</td>
</tr>
<tr>
<td>
<strong>IntlDateFormatter</strong>
</td>
<td>IntlDateFormatter</td>
</tr>
<tr>
<td>
<strong>Locale</strong>
</td>
<td>Locale</td>
</tr>
</table>



 
## CodeIgniter\I18n\Time

<table style="text-align:left">
<tr><th>Class</th><td>Time</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\I18n\Time</td></tr>
<tr><th>Extends</th><td><a href="">DateTime</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Time
</td></tr>
</table>

<table>
<tr><td>
A localized date/time package inspired
by Nesbot/Carbon and CakePHP/Chronos.

Requires the intl PHP extension.
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
<th><a href="#timezone"><strong>timezone</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#locale"><strong>locale</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#toStringFormat"><strong>toStringFormat</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Format to use when displaying datetime through __toString</td>
</tr>
<tr>
<th><a href="#relativePattern"><strong>relativePattern</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Used to check time string to determine if it is relative time or not.</td>
</tr>
<tr>
<th><a href="#testNow"><strong>testNow</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td></td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Time constructor.</td>
</tr>
<tr>
<th><a href="#now"><strong>now</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a new Time instance with the timezone set.</td>
</tr>
<tr>
<th><a href="#parse"><strong>parse</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a new Time instance while parsing a datetime string.</td>
</tr>
<tr>
<th><a href="#today"><strong>today</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Return a new time with the time set to midnight.</td>
</tr>
<tr>
<th><a href="#yesterday"><strong>yesterday</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns an instance set to midnight yesterday morning.</td>
</tr>
<tr>
<th><a href="#tomorrow"><strong>tomorrow</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns an instance set to midnight tomorrow morning.</td>
</tr>
<tr>
<th><a href="#createFromDate"><strong>createFromDate</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a new instance based on the year, month and day. If any of those three
are left empty, will default to the current value.</td>
</tr>
<tr>
<th><a href="#createFromTime"><strong>createFromTime</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a new instance with the date set to today, and the time set to the values passed in.</td>
</tr>
<tr>
<th><a href="#create"><strong>create</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a new instance with the date time values individually set.</td>
</tr>
<tr>
<th><a href="#createFromFormat"><strong>createFromFormat</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Provides a replacement for DateTime&#039;s own createFromFormat function, that provides
more flexible timeZone handling</td>
</tr>
<tr>
<th><a href="#createFromTimestamp"><strong>createFromTimestamp</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a new instance with the datetime set based on the provided UNIX timestamp.</td>
</tr>
<tr>
<th><a href="#instance"><strong>instance</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Takes an instance of DateTime and returns an instance of Time with it&#039;s same values.</td>
</tr>
<tr>
<th><a href="#toDateTime"><strong>toDateTime</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Converts the current instance to a mutable DateTime object.</td>
</tr>
<tr>
<th><a href="#setTestNow"><strong>setTestNow</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Creates an instance of Time that will be returned during testing
when calling &#039;Time::now&#039; instead of the current time.</td>
</tr>
<tr>
<th><a href="#hasTestNow"><strong>hasTestNow</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns whether we have a testNow instance saved.</td>
</tr>
<tr>
<th><a href="#getYear"><strong>getYear</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the localized Year</td>
</tr>
<tr>
<th><a href="#getMonth"><strong>getMonth</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the localized Month</td>
</tr>
<tr>
<th><a href="#getDay"><strong>getDay</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the localized day of the month.</td>
</tr>
<tr>
<th><a href="#getHour"><strong>getHour</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the localized hour (in 24-hour format).</td>
</tr>
<tr>
<th><a href="#getMinute"><strong>getMinute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the localized minutes in the hour.</td>
</tr>
<tr>
<th><a href="#getSecond"><strong>getSecond</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the localized seconds</td>
</tr>
<tr>
<th><a href="#getDayOfWeek"><strong>getDayOfWeek</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the index of the day of the week</td>
</tr>
<tr>
<th><a href="#getDayOfYear"><strong>getDayOfYear</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the index of the day of the year</td>
</tr>
<tr>
<th><a href="#getWeekOfMonth"><strong>getWeekOfMonth</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the index of the week in the month</td>
</tr>
<tr>
<th><a href="#getWeekOfYear"><strong>getWeekOfYear</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the index of the week in the year</td>
</tr>
<tr>
<th><a href="#getAge"><strong>getAge</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the age in years from the &quot;current&quot; date and &#039;now&#039;</td>
</tr>
<tr>
<th><a href="#getQuarter"><strong>getQuarter</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the number of the current quarter for the year.</td>
</tr>
<tr>
<th><a href="#getDst"><strong>getDst</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Are we in daylight savings time currently?</td>
</tr>
<tr>
<th><a href="#getLocal"><strong>getLocal</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns boolean whether the passed timezone is the same as
the local timezone.</td>
</tr>
<tr>
<th><a href="#getUtc"><strong>getUtc</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns boolean whether object is in UTC.</td>
</tr>
<tr>
<th><a href="#getTimezoneName"><strong>getTimezoneName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the name of the current timezone.</td>
</tr>
<tr>
<th><a href="#setYear"><strong>setYear</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the current year for this instance.</td>
</tr>
<tr>
<th><a href="#setMonth"><strong>setMonth</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the month of the year.</td>
</tr>
<tr>
<th><a href="#setDay"><strong>setDay</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the day of the month.</td>
</tr>
<tr>
<th><a href="#setHour"><strong>setHour</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the hour of the day (24 hour cycle)</td>
</tr>
<tr>
<th><a href="#setMinute"><strong>setMinute</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the minute of the hour</td>
</tr>
<tr>
<th><a href="#setSecond"><strong>setSecond</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the second of the minute.</td>
</tr>
<tr>
<th><a href="#setValue"><strong>setValue</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Helper method to do the heavy lifting of the &#039;setX&#039; methods.</td>
</tr>
<tr>
<th><a href="#setTimezone"><strong>setTimezone</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new instance with the revised timezone.</td>
</tr>
<tr>
<th><a href="#setTimestamp"><strong>setTimestamp</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new instance with the date set to the new timestamp.</td>
</tr>
<tr>
<th><a href="#addSeconds"><strong>addSeconds</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $seconds added to the time.</td>
</tr>
<tr>
<th><a href="#addMinutes"><strong>addMinutes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $minutes added to the time.</td>
</tr>
<tr>
<th><a href="#addHours"><strong>addHours</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $hours added to the time.</td>
</tr>
<tr>
<th><a href="#addDays"><strong>addDays</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $days added to the time.</td>
</tr>
<tr>
<th><a href="#addMonths"><strong>addMonths</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $months added to the time.</td>
</tr>
<tr>
<th><a href="#addYears"><strong>addYears</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $years added to the time.</td>
</tr>
<tr>
<th><a href="#subSeconds"><strong>subSeconds</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $seconds subtracted from the time.</td>
</tr>
<tr>
<th><a href="#subMinutes"><strong>subMinutes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $minutes subtracted from the time.</td>
</tr>
<tr>
<th><a href="#subHours"><strong>subHours</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $hours subtracted from the time.</td>
</tr>
<tr>
<th><a href="#subDays"><strong>subDays</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $days subtracted from the time.</td>
</tr>
<tr>
<th><a href="#subMonths"><strong>subMonths</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $months subtracted from the time.</td>
</tr>
<tr>
<th><a href="#subYears"><strong>subYears</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a new Time instance with $hours subtracted from the time.</td>
</tr>
<tr>
<th><a href="#toDateTimeString"><strong>toDateTimeString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the localized value of the date in the format &#039;Y-m-d H:i:s&#039;</td>
</tr>
<tr>
<th><a href="#toDateString"><strong>toDateString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a localized version of the date in Y-m-d format.</td>
</tr>
<tr>
<th><a href="#toFormattedDateString"><strong>toFormattedDateString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a localized version of the date in nicer date format:</td>
</tr>
<tr>
<th><a href="#toTimeString"><strong>toTimeString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a localized version of the time in nicer date format:</td>
</tr>
<tr>
<th><a href="#toLocalizedString"><strong>toLocalizedString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the localized value of this instance in $format.</td>
</tr>
<tr>
<th><a href="#equals"><strong>equals</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines if the datetime passed in is equal to the current instance.</td>
</tr>
<tr>
<th><a href="#sameAs"><strong>sameAs</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Ensures that the times are identical, taking timezone into account.</td>
</tr>
<tr>
<th><a href="#isBefore"><strong>isBefore</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines if the current instance&#039;s time is before $testTime,
after converting to UTC.</td>
</tr>
<tr>
<th><a href="#isAfter"><strong>isAfter</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Determines if the current instance&#039;s time is after $testTime,
after converting in UTC.</td>
</tr>
<tr>
<th><a href="#humanize"><strong>humanize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a text string that is easily readable that describes
how long ago, or how long from now, a date is, like:</td>
</tr>
<tr>
<th><a href="#difference"><strong>difference</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#getUTCObject"><strong>getUTCObject</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns a Time instance with the timezone converted to UTC.</td>
</tr>
<tr>
<th><a href="#getCalendar"><strong>getCalendar</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the IntlCalendar object used for this object,
taking into account the locale, date, etc.</td>
</tr>
<tr>
<th><a href="#hasRelativeKeywords"><strong>hasRelativeKeywords</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Check a time string to see if it includes a relative date (like &#039;next Tuesday&#039;).</td>
</tr>
<tr>
<th><a href="#__toString"><strong>__toString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Outputs a short format version of the datetime.</td>
</tr>
<tr>
<th><a href="#__get"><strong>__get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allow for property-type access to any getX method...

Note that we cannot use this for any of our setX methods,
as they return new Time objects, but the __set ignores
return values.</td>
</tr>
<tr>
<th><a href="#__isset"><strong>__isset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allow for property-type checking to any getX method.</td>
</tr>

</table>





### Properties


<hr>

#### $timezone

```php
protected $timezone;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\DateTimeZone
</td>
</tr>
</table>


<hr>

#### $locale

```php
protected $locale;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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

#### $toStringFormat

```php
protected $toStringFormat = 'yyyy-MM-dd HH:mm:ss';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Format to use when displaying datetime through __toString
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

#### $relativePattern

```php
protected static $relativePattern = '/this|next|last|tomorrow|yesterday|midnight|today|[+-]|first|last|ago/i';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used to check time string to determine if it is relative time or not.
</td></tr>
</table>

<table>
<tr><td>
...
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

#### $testNow

```php
protected static $testNow;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(string $time = null, $timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Time constructor.
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
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
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
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 35 lines (105 - 139)</small></summary>

```php
public function __construct(string $time = null, $timezone = null, string $locale = null)
{
	// If no locale was provided, grab it from Locale (set by IncomingRequest for web requests)
	$this->locale = ! empty($locale) ? $locale : Locale::getDefault();

	// If a test instance has been provided, use it instead.
	if (is_null($time) && static::$testNow instanceof Time)
	{
		if (empty($timezone))
		{
			$timezone = static::$testNow->getTimezone();
		}

		$time = static::$testNow->toDateTimeString();
	}

	$timezone       = ! empty($timezone) ? $timezone : date_default_timezone_get();
	$this->timezone = $timezone instanceof DateTimeZone ? $timezone : new DateTimeZone($timezone);

	if (! empty($time))
	{
		// If the time string was a relative string (i.e. 'next Tuesday')
		// then we need to adjust the time going in so that we have a current
		// timezone to work with.
		if (is_string($time) && static::hasRelativeKeywords($time))
		{
			$instance = new DateTime('now', $this->timezone);
			$instance->modify($time);

			$time = $instance->format('Y-m-d H:i:s');
		}
	}

	return parent::__construct($time, $this->timezone);
}
```

</details>


<hr>

#### now()

```php
public static function now($timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with the timezone set.
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
<td><code>$timezone</code></td>
<td><em>string<br>\DateTimeZone<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (152 - 155)</small></summary>

```php
public static function now($timezone = null, string $locale = null)
{
	return new Time(null, $timezone, $locale);
}
```

</details>


<hr>

#### parse()

```php
public static function parse(string $datetime, $timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance while parsing a datetime string.
</td></tr>
</table>

<table>
<tr><td>
Example:
$time = Time::parse('first day of December 2008');
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
<td><code>$datetime</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (172 - 175)</small></summary>

```php
public static function parse(string $datetime, $timezone = null, string $locale = null)
{
	return new Time($datetime, $timezone, $locale);
}
```

</details>


<hr>

#### today()

```php
public static function today($timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return a new time with the time set to midnight.
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
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (188 - 191)</small></summary>

```php
public static function today($timezone = null, string $locale = null)
{
	return new Time(date('Y-m-d 00:00:00'), $timezone, $locale);
}
```

</details>


<hr>

#### yesterday()

```php
public static function yesterday($timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an instance set to midnight yesterday morning.
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
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (204 - 207)</small></summary>

```php
public static function yesterday($timezone = null, string $locale = null)
{
	return new Time(date('Y-m-d 00:00:00', strtotime('-1 day')), $timezone, $locale);
}
```

</details>


<hr>

#### tomorrow()

```php
public static function tomorrow($timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an instance set to midnight tomorrow morning.
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
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (220 - 223)</small></summary>

```php
public static function tomorrow($timezone = null, string $locale = null)
{
	return new Time(date('Y-m-d 00:00:00', strtotime('+1 day')), $timezone, $locale);
}
```

</details>


<hr>

#### createFromDate()

```php
public static function createFromDate(int $year = null, int $month = null, int $day = null, $timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new instance based on the year, month and day. If any of those three
are left empty, will default to the current value.
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
<td><code>$year</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$month</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$day</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (240 - 243)</small></summary>

```php
public static function createFromDate(int $year = null, int $month = null, int $day = null, $timezone = null, string $locale = null)
{
	return static::create($year, $month, $day, null, null, null, $timezone, $locale);
}
```

</details>


<hr>

#### createFromTime()

```php
public static function createFromTime(int $hour = null, int $minutes = null, int $seconds = null, $timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new instance with the date set to today, and the time set to the values passed in.
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
<td><code>$hour</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$minutes</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$seconds</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (259 - 262)</small></summary>

```php
public static function createFromTime(int $hour = null, int $minutes = null, int $seconds = null, $timezone = null, string $locale = null)
{
	return static::create(null, null, null, $hour, $minutes, $seconds, $timezone, $locale);
}
```

</details>


<hr>

#### create()

```php
public static function create(int $year = null, int $month = null, int $day = null, int $hour = null, int $minutes = null, int $seconds = null, $timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new instance with the date time values individually set.
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
<td><code>$year</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$month</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$day</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$hour</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$minutes</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>6.</td>
<td><code>$seconds</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>7.</td>
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>8.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 11 lines (281 - 291)</small></summary>

```php
public static function create(int $year = null, int $month = null, int $day = null, int $hour = null, int $minutes = null, int $seconds = null, $timezone = null, string $locale = null)
{
	$year    = is_null($year) ? date('Y') : $year;
	$month   = is_null($month) ? date('m') : $month;
	$day     = is_null($day) ? date('d') : $day;
	$hour    = empty($hour) ? 0 : $hour;
	$minutes = empty($minutes) ? 0 : $minutes;
	$seconds = empty($seconds) ? 0 : $seconds;

	return new Time(date('Y-m-d H:i:s', strtotime("{$year}-{$month}-{$day} {$hour}:{$minutes}:{$seconds}")), $timezone, $locale);
}
```

</details>


<hr>

#### createFromFormat()

```php
public static function createFromFormat($format, $datetime, $timeZone = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides a replacement for DateTime's own createFromFormat function, that provides
more flexible timeZone handling
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
<td><code>$format</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$datetime</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$timeZone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 6 lines (306 - 311)</small></summary>

```php
public static function createFromFormat($format, $datetime, $timeZone = null)
{
	$date = parent::createFromFormat($format, $datetime);

	return new Time($date->format('Y-m-d H:i:s'), $timeZone);
}
```

</details>


<hr>

#### createFromTimestamp()

```php
public static function createFromTimestamp(int $timestamp, $timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new instance with the datetime set based on the provided UNIX timestamp.
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
<td><code>$timestamp</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (325 - 328)</small></summary>

```php
public static function createFromTimestamp(int $timestamp, $timezone = null, string $locale = null)
{
	return new Time(date('Y-m-d H:i:s', $timestamp), $timezone, $locale);
}
```

</details>


<hr>

#### instance()

```php
public static function instance(DateTime $dateTime, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes an instance of DateTime and returns an instance of Time with it's same values.
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
<td><code>$dateTime</code></td>
<td><em>\DateTime
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 7 lines (341 - 347)</small></summary>

```php
public static function instance(DateTime $dateTime, string $locale = null)
{
	$date     = $dateTime->format('Y-m-d H:i:s');
	$timezone = $dateTime->getTimezone();

	return new Time($date, $timezone, $locale);
}
```

</details>


<hr>

#### toDateTime()

```php
public function toDateTime()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts the current instance to a mutable DateTime object.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\DateTime
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 7 lines (357 - 363)</small></summary>

```php
public function toDateTime()
{
	$dateTime = new DateTime(null, $this->getTimezone());
	$dateTime->setTimestamp(parent::getTimestamp());

	return $dateTime;
}
```

</details>


<hr>

#### setTestNow()

```php
public static function setTestNow($datetime = null, $timezone = null, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Creates an instance of Time that will be returned during testing
when calling 'Time::now' instead of the current time.
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
<td><code>$datetime</code></td>
<td><em>\CodeIgniter\I18n\Time<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
<td><em>\DateTimeZone<br>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
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
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 21 lines (379 - 399)</small></summary>

```php
public static function setTestNow($datetime = null, $timezone = null, string $locale = null)
{
	// Reset the test instance
	if (is_null($datetime))
	{
		static::$testNow = null;
		return;
	}

	// Convert to a Time instance
	if (is_string($datetime))
	{
		$datetime = new Time($datetime, $timezone, $locale);
	}
	elseif ($datetime instanceof DateTime && ! $datetime instanceof Time)
	{
		$datetime = new Time($datetime->format('Y-m-d H:i:s'), $timezone);
	}

	static::$testNow = $datetime;
}
```

</details>


<hr>

#### hasTestNow()

```php
public static function hasTestNow() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns whether we have a testNow instance saved.
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
<summary><small>Source: 4 lines (408 - 411)</small></summary>

```php
public static function hasTestNow(): bool
{
	return ! is_null(static::$testNow);
}
```

</details>


<hr>

#### getYear()

```php
public function getYear() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the localized Year
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (424 - 427)</small></summary>

```php
public function getYear(): string
{
	return $this->toLocalizedString('y');
}
```

</details>


<hr>

#### getMonth()

```php
public function getMonth() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the localized Month
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (437 - 440)</small></summary>

```php
public function getMonth(): string
{
	return $this->toLocalizedString('M');
}
```

</details>


<hr>

#### getDay()

```php
public function getDay() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the localized day of the month.
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (450 - 453)</small></summary>

```php
public function getDay(): string
{
	return $this->toLocalizedString('d');
}
```

</details>


<hr>

#### getHour()

```php
public function getHour() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the localized hour (in 24-hour format).
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (463 - 466)</small></summary>

```php
public function getHour(): string
{
	return $this->toLocalizedString('H');
}
```

</details>


<hr>

#### getMinute()

```php
public function getMinute() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the localized minutes in the hour.
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (476 - 479)</small></summary>

```php
public function getMinute(): string
{
	return $this->toLocalizedString('m');
}
```

</details>


<hr>

#### getSecond()

```php
public function getSecond() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the localized seconds
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (489 - 492)</small></summary>

```php
public function getSecond(): string
{
	return $this->toLocalizedString('s');
}
```

</details>


<hr>

#### getDayOfWeek()

```php
public function getDayOfWeek() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the index of the day of the week
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (502 - 505)</small></summary>

```php
public function getDayOfWeek(): string
{
	return $this->toLocalizedString('c');
}
```

</details>


<hr>

#### getDayOfYear()

```php
public function getDayOfYear() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the index of the day of the year
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (515 - 518)</small></summary>

```php
public function getDayOfYear(): string
{
	return $this->toLocalizedString('D');
}
```

</details>


<hr>

#### getWeekOfMonth()

```php
public function getWeekOfMonth() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the index of the week in the month
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (528 - 531)</small></summary>

```php
public function getWeekOfMonth(): string
{
	return $this->toLocalizedString('W');
}
```

</details>


<hr>

#### getWeekOfYear()

```php
public function getWeekOfYear() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the index of the week in the year
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (541 - 544)</small></summary>

```php
public function getWeekOfYear(): string
{
	return $this->toLocalizedString('w');
}
```

</details>


<hr>

#### getAge()

```php
public function getAge()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the age in years from the "current" date and 'now'
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 8 lines (554 - 561)</small></summary>

```php
public function getAge()
{
	$now  = Time::now()->getTimestamp();
	$time = $this->getTimestamp();

	// future dates have no age
	return max(0, date('Y', $now) - date('Y', $time));
}
```

</details>


<hr>

#### getQuarter()

```php
public function getQuarter() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the number of the current quarter for the year.
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (571 - 574)</small></summary>

```php
public function getQuarter(): string
{
	return $this->toLocalizedString('Q');
}
```

</details>


<hr>

#### getDst()

```php
public function getDst() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Are we in daylight savings time currently?
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
<summary><small>Source: 18 lines (583 - 600)</small></summary>

```php
public function getDst(): bool
{
	// grab the transactions that would affect today
	$start       = strtotime('-1 year', $this->getTimestamp());
	$end         = strtotime('+2 year', $start);
	$transitions = $this->timezone->getTransitions($start, $end);

	$daylightSaving = false;
	foreach ($transitions as $transition)
	{
		if ($transition['time'] > $this->format('U'))
		{
			$daylightSaving = (bool) $transition['isdst'] ?? $daylightSaving;
			break;
		}
	}
	return $daylightSaving;
}
```

</details>


<hr>

#### getLocal()

```php
public function getLocal() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns boolean whether the passed timezone is the same as
the local timezone.
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
<summary><small>Source: 6 lines (610 - 615)</small></summary>

```php
public function getLocal(): bool
{
	$local = date_default_timezone_get();

	return $local === $this->timezone->getName();
}
```

</details>


<hr>

#### getUtc()

```php
public function getUtc() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns boolean whether object is in UTC.
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
<summary><small>Source: 4 lines (624 - 627)</small></summary>

```php
public function getUtc(): bool
{
	return $this->getOffset() === 0;
}
```

</details>


<hr>

#### getTimezoneName()

```php
public function getTimezoneName() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the name of the current timezone.
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
<summary><small>Source: 4 lines (634 - 637)</small></summary>

```php
public function getTimezoneName(): string
{
	return $this->timezone->getName();
}
```

</details>


<hr>

#### setYear()

```php
public function setYear($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the current year for this instance.
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
<td><code>$value</code></td>
<td><em>int<br>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (651 - 654)</small></summary>

```php
public function setYear($value)
{
	return $this->setValue('year', $value);
}
```

</details>


<hr>

#### setMonth()

```php
public function setMonth($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the month of the year.
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
<td><code>$value</code></td>
<td><em>int<br>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 14 lines (664 - 677)</small></summary>

```php
public function setMonth($value)
{
	if (is_numeric($value) && $value < 1 || $value > 12)
	{
		throw I18nException::forInvalidMonth($value);
	}

	if (is_string($value) && ! is_numeric($value))
	{
		$value = date('m', strtotime("{$value} 1 2017"));
	}

	return $this->setValue('month', $value);
}
```

</details>


<hr>

#### setDay()

```php
public function setDay($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the day of the month.
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
<td><code>$value</code></td>
<td><em>int<br>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 16 lines (687 - 702)</small></summary>

```php
public function setDay($value)
{
	if ($value < 1 || $value > 31)
	{
		throw I18nException::forInvalidDay($value);
	}

	$date    = $this->getYear() . '-' . $this->getMonth();
	$lastDay = date('t', strtotime($date));
	if ($value > $lastDay)
	{
		throw I18nException::forInvalidOverDay($lastDay, $value);
	}

	return $this->setValue('day', $value);
}
```

</details>


<hr>

#### setHour()

```php
public function setHour($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the hour of the day (24 hour cycle)
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
<td><code>$value</code></td>
<td><em>int<br>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 9 lines (712 - 720)</small></summary>

```php
public function setHour($value)
{
	if ($value < 0 || $value > 23)
	{
		throw I18nException::forInvalidHour($value);
	}

	return $this->setValue('hour', $value);
}
```

</details>


<hr>

#### setMinute()

```php
public function setMinute($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the minute of the hour
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
<td><code>$value</code></td>
<td><em>int<br>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 9 lines (730 - 738)</small></summary>

```php
public function setMinute($value)
{
	if ($value < 0 || $value > 59)
	{
		throw I18nException::forInvalidMinutes($value);
	}

	return $this->setValue('minute', $value);
}
```

</details>


<hr>

#### setSecond()

```php
public function setSecond($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the second of the minute.
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
<td><code>$value</code></td>
<td><em>int<br>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 9 lines (748 - 756)</small></summary>

```php
public function setSecond($value)
{
	if ($value < 0 || $value > 59)
	{
		throw I18nException::forInvalidSeconds($value);
	}

	return $this->setValue('second', $value);
}
```

</details>


<hr>

#### setValue()

```php
protected function setValue(string $name, $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Helper method to do the heavy lifting of the 'setX' methods.
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
<td><code>$value</code></td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 7 lines (767 - 773)</small></summary>

```php
protected function setValue(string $name, $value)
{
	list($year, $month, $day, $hour, $minute, $second) = explode('-', $this->format('Y-n-j-G-i-s'));
	$$name                                             = $value;

	return Time::create($year, $month, $day, $hour, $minute, $second, $this->getTimezoneName(), $this->locale);
}
```

</details>


<hr>

#### setTimezone()

```php
public function setTimezone($timezone)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new instance with the revised timezone.
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
<td><code>$timezone</code></td>
<td><em>string<br>\DateTimeZone
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 5 lines (783 - 787)</small></summary>

```php
public function setTimezone($timezone)
{
	$timezone = $timezone instanceof DateTimeZone ? $timezone : new DateTimeZone($timezone);
	return Time::instance($this->toDateTime()->setTimezone($timezone), $this->locale);
}
```

</details>


<hr>

#### setTimestamp()

```php
public function setTimestamp($timestamp)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new instance with the date set to the new timestamp.
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
<td><code>$timestamp</code></td>
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
<td>\CodeIgniter\I18n\Time
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 6 lines (797 - 802)</small></summary>

```php
public function setTimestamp($timestamp)
{
	$time = date('Y-m-d H:i:s', $timestamp);

	return Time::parse($time, $this->timezone, $this->locale);
}
```

</details>


<hr>

#### addSeconds()

```php
public function addSeconds(int $seconds)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $seconds added to the time.
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
<td><code>$seconds</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (815 - 820)</small></summary>

```php
public function addSeconds(int $seconds)
{
	$time = clone($this);

	return $time->add(DateInterval::createFromDateString("{$seconds} seconds"));
}
```

</details>


<hr>

#### addMinutes()

```php
public function addMinutes(int $minutes)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $minutes added to the time.
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
<td><code>$minutes</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (829 - 834)</small></summary>

```php
public function addMinutes(int $minutes)
{
	$time = clone($this);

	return $time->add(DateInterval::createFromDateString("{$minutes} minutes"));
}
```

</details>


<hr>

#### addHours()

```php
public function addHours(int $hours)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $hours added to the time.
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
<td><code>$hours</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (843 - 848)</small></summary>

```php
public function addHours(int $hours)
{
	$time = clone($this);

	return $time->add(DateInterval::createFromDateString("{$hours} hours"));
}
```

</details>


<hr>

#### addDays()

```php
public function addDays(int $days)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $days added to the time.
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
<td><code>$days</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (857 - 862)</small></summary>

```php
public function addDays(int $days)
{
	$time = clone($this);

	return $time->add(DateInterval::createFromDateString("{$days} days"));
}
```

</details>


<hr>

#### addMonths()

```php
public function addMonths(int $months)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $months added to the time.
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
<td><code>$months</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (871 - 876)</small></summary>

```php
public function addMonths(int $months)
{
	$time = clone($this);

	return $time->add(DateInterval::createFromDateString("{$months} months"));
}
```

</details>


<hr>

#### addYears()

```php
public function addYears(int $years)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $years added to the time.
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
<td><code>$years</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (885 - 890)</small></summary>

```php
public function addYears(int $years)
{
	$time = clone($this);

	return $time->add(DateInterval::createFromDateString("{$years} years"));
}
```

</details>


<hr>

#### subSeconds()

```php
public function subSeconds(int $seconds)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $seconds subtracted from the time.
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
<td><code>$seconds</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (899 - 904)</small></summary>

```php
public function subSeconds(int $seconds)
{
	$time = clone($this);

	return $time->sub(DateInterval::createFromDateString("{$seconds} seconds"));
}
```

</details>


<hr>

#### subMinutes()

```php
public function subMinutes(int $minutes)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $minutes subtracted from the time.
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
<td><code>$minutes</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (913 - 918)</small></summary>

```php
public function subMinutes(int $minutes)
{
	$time = clone($this);

	return $time->sub(DateInterval::createFromDateString("{$minutes} minutes"));
}
```

</details>


<hr>

#### subHours()

```php
public function subHours(int $hours)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $hours subtracted from the time.
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
<td><code>$hours</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (927 - 932)</small></summary>

```php
public function subHours(int $hours)
{
	$time = clone($this);

	return $time->sub(DateInterval::createFromDateString("{$hours} hours"));
}
```

</details>


<hr>

#### subDays()

```php
public function subDays(int $days)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $days subtracted from the time.
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
<td><code>$days</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (941 - 946)</small></summary>

```php
public function subDays(int $days)
{
	$time = clone($this);

	return $time->sub(DateInterval::createFromDateString("{$days} days"));
}
```

</details>


<hr>

#### subMonths()

```php
public function subMonths(int $months)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $months subtracted from the time.
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
<td><code>$months</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (955 - 960)</small></summary>

```php
public function subMonths(int $months)
{
	$time = clone($this);

	return $time->sub(DateInterval::createFromDateString("{$months} months"));
}
```

</details>


<hr>

#### subYears()

```php
public function subYears(int $years)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a new Time instance with $hours subtracted from the time.
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
<td><code>$years</code></td>
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
<td>static
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (969 - 974)</small></summary>

```php
public function subYears(int $years)
{
	$time = clone($this);

	return $time->sub(DateInterval::createFromDateString("{$years} years"));
}
```

</details>


<hr>

#### toDateTimeString()

```php
public function toDateTimeString()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the localized value of the date in the format 'Y-m-d H:i:s'
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>







<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (985 - 988)</small></summary>

```php
public function toDateTimeString()
{
	return $this->toLocalizedString('yyyy-MM-dd HH:mm:ss');
}
```

</details>


<hr>

#### toDateString()

```php
public function toDateString()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a localized version of the date in Y-m-d format.
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (998 - 1001)</small></summary>

```php
public function toDateString()
{
	return $this->toLocalizedString('yyyy-MM-dd');
}
```

</details>


<hr>

#### toFormattedDateString()

```php
public function toFormattedDateString()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a localized version of the date in nicer date format:
</td></tr>
</table>

<table>
<tr><td>
i.e. Apr 1, 2017
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (1013 - 1016)</small></summary>

```php
public function toFormattedDateString()
{
	return $this->toLocalizedString('MMM d, yyyy');
}
```

</details>


<hr>

#### toTimeString()

```php
public function toTimeString()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a localized version of the time in nicer date format:
</td></tr>
</table>

<table>
<tr><td>
i.e. 13:20:33
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (1028 - 1031)</small></summary>

```php
public function toTimeString()
{
	return $this->toLocalizedString('HH:mm:ss');
}
```

</details>


<hr>

#### toLocalizedString()

```php
public function toLocalizedString(string $format = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the localized value of this instance in $format.
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
<td><code>$format</code></td>
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
<td>string<br>bool
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 6 lines (1043 - 1048)</small></summary>

```php
public function toLocalizedString(string $format = null)
{
	$format = $format ?? $this->toStringFormat;

	return IntlDateFormatter::formatObject($this->toDateTime(), $format, $this->locale);
}
```

</details>


<hr>

#### equals()

```php
public function equals($testTime, string $timezone = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines if the datetime passed in is equal to the current instance.
</td></tr>
</table>

<table>
<tr><td>
Equal in this case means that they represent the same moment in time,
and are not required to be in the same timezone, as both times are
converted to UTC and compared that way.
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
<td><code>$testTime</code></td>
<td><em>\Time<br>\DateTime<br>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 10 lines (1067 - 1076)</small></summary>

```php
public function equals($testTime, string $timezone = null): bool
{
	$testTime = $this->getUTCObject($testTime, $timezone);

	$ourTime = $this->toDateTime()
			->setTimezone(new DateTimeZone('UTC'))
			->format('Y-m-d H:i:s');

	return $testTime->format('Y-m-d H:i:s') === $ourTime;
}
```

</details>


<hr>

#### sameAs()

```php
public function sameAs($testTime, string $timezone = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ensures that the times are identical, taking timezone into account.
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
<td><code>$testTime</code></td>
<td><em>\Time<br>\DateTime<br>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 18 lines (1089 - 1106)</small></summary>

```php
public function sameAs($testTime, string $timezone = null): bool
{
	if ($testTime instanceof DateTime)
	{
		$testTime = $testTime->format('Y-m-d H:i:s');
	}
	else if (is_string($testTime))
	{
		$timezone = $timezone ?: $this->timezone;
		$timezone = $timezone instanceof DateTimeZone ? $timezone : new DateTimeZone($timezone);
		$testTime = new DateTime($testTime, $timezone);
		$testTime = $testTime->format('Y-m-d H:i:s');
	}

	$ourTime = $this->toDateTimeString();

	return $testTime === $ourTime;
}
```

</details>


<hr>

#### isBefore()

```php
public function isBefore($testTime, string $timezone = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines if the current instance's time is before $testTime,
after converting to UTC.
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
<td><code>$testTime</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 7 lines (1120 - 1126)</small></summary>

```php
public function isBefore($testTime, string $timezone = null): bool
{
	$testTime = $this->getUTCObject($testTime, $timezone)->getTimestamp();
	$ourTime  = $this->getTimestamp();

	return $ourTime < $testTime;
}
```

</details>


<hr>

#### isAfter()

```php
public function isAfter($testTime, string $timezone = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines if the current instance's time is after $testTime,
after converting in UTC.
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
<td><code>$testTime</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 7 lines (1140 - 1146)</small></summary>

```php
public function isAfter($testTime, string $timezone = null): bool
{
	$testTime = $this->getUTCObject($testTime, $timezone)->getTimestamp();
	$ourTime  = $this->getTimestamp();

	return $ourTime > $testTime;
}
```

</details>


<hr>

#### humanize()

```php
public function humanize()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a text string that is easily readable that describes
how long ago, or how long from now, a date is, like:
</td></tr>
</table>

<table>
<tr><td>
- 3 weeks ago
- in 4 days
- 6 hours ago
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 58 lines (1164 - 1221)</small></summary>

```php
public function humanize()
{
	$now  = IntlCalendar::fromDateTime(Time::now($this->timezone)->toDateTimeString());
	$time = $this->getCalendar()->getTime();

	$years   = $now->fieldDifference($time, IntlCalendar::FIELD_YEAR);
	$months  = $now->fieldDifference($time, IntlCalendar::FIELD_MONTH);
	$days    = $now->fieldDifference($time, IntlCalendar::FIELD_DAY_OF_YEAR);
	$hours   = $now->fieldDifference($time, IntlCalendar::FIELD_HOUR_OF_DAY);
	$minutes = $now->fieldDifference($time, IntlCalendar::FIELD_MINUTE);

	$phrase = null;

	if ($years !== 0)
	{
		$phrase = lang('Time.years', [abs($years)]);
		$before = $years < 0;
	}
	else if ($months !== 0)
	{
		$phrase = lang('Time.months', [abs($months)]);
		$before = $months < 0;
	}
	else if ($days !== 0 && (abs($days) >= 7))
	{
		$weeks  = ceil($days / 7);
		$phrase = lang('Time.weeks', [abs($weeks)]);
		$before = $days < 0;
	}
	else if ($days !== 0)
	{
		$before = $days < 0;

		// Yesterday/Tomorrow special cases
		if (abs($days) === 1)
		{
			return $before ? lang('Time.yesterday') : lang('Time.tomorrow');
		}

		$phrase = lang('Time.days', [abs($days)]);
	}
	else if ($hours !== 0)
	{
		// Display the actual time instead of a regular phrase.
		return $this->format('g:i a');
	}
	else if ($minutes !== 0)
	{
		$phrase = lang('Time.minutes', [abs($minutes)]);
		$before = $minutes < 0;
	}
	else
	{
		return lang('Time.now');
	}

	return $before ? lang('Time.ago', [$phrase]) : lang('Time.inFuture', [$phrase]);
}
```

</details>


<hr>

#### difference()

```php
public function difference($testTime, string $timezone = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td><code>$testTime</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
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
<td>\CodeIgniter\I18n\TimeDifference
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 7 lines (1230 - 1236)</small></summary>

```php
public function difference($testTime, string $timezone = null)
{
	$testTime = $this->getUTCObject($testTime, $timezone);
	$ourTime  = $this->getUTCObject($this);

	return new TimeDifference($ourTime, $testTime);
}
```

</details>


<hr>

#### getUTCObject()

```php
public function getUTCObject($time, string $timezone = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a Time instance with the timezone converted to UTC.
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$timezone</code></td>
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
<td>\DateTime<br>static
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 21 lines (1251 - 1271)</small></summary>

```php
public function getUTCObject($time, string $timezone = null)
{
	if ($time instanceof Time)
	{
		$time = $time->toDateTime()
				->setTimezone(new DateTimeZone('UTC'));
	}
	elseif ($time instanceof DateTime)
	{
		$time = $time->setTimezone(new DateTimeZone('UTC'));
	}
	elseif (is_string($time))
	{
		$timezone = $timezone ?: $this->timezone;
		$timezone = $timezone instanceof DateTimeZone ? $timezone : new DateTimeZone($timezone);
		$time     = new DateTime($time, $timezone);
		$time     = $time->setTimezone(new DateTimeZone('UTC'));
	}

	return $time;
}
```

</details>


<hr>

#### getCalendar()

```php
public function getCalendar()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the IntlCalendar object used for this object,
taking into account the locale, date, etc.
</td></tr>
</table>

<table>
<tr><td>
Primarily used internally to provide the difference and comparison functions,
but available for public consumption if they need it.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\IntlCalendar
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (1285 - 1288)</small></summary>

```php
public function getCalendar()
{
	return IntlCalendar::fromDateTime($this->toDateTimeString());
}
```

</details>


<hr>

#### hasRelativeKeywords()

```php
protected static function hasRelativeKeywords(string $time) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Check a time string to see if it includes a relative date (like 'next Tuesday').
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
<summary><small>Source: 10 lines (1299 - 1308)</small></summary>

```php
protected static function hasRelativeKeywords(string $time): bool
{
	// skip common format with a '-' in it
	if (preg_match('/[0-9]{4}-[0-9]{1,2}-[0-9]{1,2}/', $time) !== 1)
	{
		return preg_match(static::$relativePattern, $time) > 0;
	}

	return false;
}
```

</details>


<hr>

#### __toString()

```php
public function __toString() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Outputs a short format version of the datetime.
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (1318 - 1321)</small></summary>

```php
public function __toString(): string
{
	return IntlDateFormatter::formatObject($this->toDateTime(), $this->toStringFormat, $this->locale);
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
Allow for property-type access to any getX method...

Note that we cannot use this for any of our setX methods,
as they return new Time objects, but the __set ignores
return values.
</td></tr>
</table>

<table>
<tr><td>
See <a href="http://php.net/manual/en/language.oop5.overloading.php">http://php.net/manual/en/language.oop5.overloading.php</a>
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
<summary><small>Source: 11 lines (1337 - 1347)</small></summary>

```php
public function __get($name)
{
	$method = 'get' . ucfirst($name);

	if (method_exists($this, $method))
	{
		return $this->$method();
	}

	return null;
}
```

</details>


<hr>

#### __isset()

```php
public function __isset($name) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allow for property-type checking to any getX method.
</td></tr>
</table>

<table>
<tr><td>
..
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
<summary><small>Source: 6 lines (1358 - 1363)</small></summary>

```php
public function __isset($name): bool
{
	$method = 'get' . ucfirst($name);

	return method_exists($this, $method);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/I18n/Time.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/Exceptions/I18nException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/I18n/TimeDifference.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>