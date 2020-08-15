


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/date_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/array_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/url_helper.md">next</a></td>
</tr>
</table>




 



# Date Helper


<hr>

## now()

```php
function now(string $timezone = null) : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get "now" time
</td></tr>
</table>

<table>
<tr><td>
Returns time() based on the timezone parameter or on the
app_timezone() setting
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
<summary><small>Source: 14 lines (59 - 72)</small></summary>

```php
function now(string $timezone = null): int
{
	$timezone = empty($timezone) ? app_timezone() : $timezone;

	if ($timezone === 'local' || $timezone === date_default_timezone_get())
	{
		return time();
	}

	$datetime = new DateTime('now', new DateTimeZone($timezone));
	sscanf($datetime->format('j-n-Y G:i:s'), '%d-%d-%d %d:%d:%d', $day, $month, $year, $hour, $minute, $second);

	return mktime($hour, $minute, $second, $month, $day, $year);
}
```

</details>


<hr>

## timezone_select()

```php
function timezone_select(string $class = '', string $default = '', int $what = \DateTimeZone::ALL, string $country = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates a select field of all available timezones
</td></tr>
</table>

<table>
<tr><td>
Returns a string with the formatted HTML
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
<td><code>$class</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Optional class to apply to the select field</td>
</tr>

<tr>
<td>2.</td>
<td><code>$default</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Default value for initial selection</td>
</tr>

<tr>
<td>3.</td>
<td><code>$what</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>One of the DateTimeZone class constants (for listIdentifiers)</td>
</tr>

<tr>
<td>4.</td>
<td><code>$country</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>A two-letter ISO 3166-1 compatible country code (for listIdentifiers)</td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 13 lines (90 - 102)</small></summary>

```php
function timezone_select(string $class = '', string $default = '', int $what = \DateTimeZone::ALL, string $country = null): string
{
	$timezones = \DateTimeZone::listIdentifiers($what, $country);

	$buffer = "<select name='timezone' class='{$class}'>" . PHP_EOL;
	foreach ($timezones as $timezone)
	{
		$selected = ($timezone === $default) ? 'selected' : '';
		$buffer  .= "<option value='{$timezone}' {$selected}>{$timezone}</option>" . PHP_EOL;
	}

	return $buffer . ('</select>' . PHP_EOL);
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/date_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/array_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/url_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:06**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>