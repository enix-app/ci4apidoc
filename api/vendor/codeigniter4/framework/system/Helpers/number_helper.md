


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/number_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/url_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/number_helper.md">next</a></td>
</tr>
</table>




 



# Number Helper


<hr>

## number_to_size()

```php
function number_to_size($num, int $precision = 1, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Formats a numbers as bytes, based on size, and adds the appropriate suffix
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
<td><code>$num</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Will be cast as int</td>
</tr>

<tr>
<td>2.</td>
<td><code>$precision</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$locale</code></td>
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
<td>bool<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 46 lines (58 - 103)</small></summary>

```php
function number_to_size($num, int $precision = 1, string $locale = null)
{
	// Strip any formatting & ensure numeric input
	try
	{
		$num = 0 + str_replace(',', '', $num);
	}
	catch (\ErrorException $ee)
	{
		return false;
	}

	// ignore sub part
	$generalLocale = $locale;
	if (! empty($locale) && ( $underscorePos = strpos($locale, '_')))
	{
		$generalLocale = substr($locale, 0, $underscorePos);
	}

	if ($num >= 1000000000000)
	{
		$num  = round($num / 1099511627776, $precision);
		$unit = lang('Number.terabyteAbbr', [], $generalLocale);
	}
	elseif ($num >= 1000000000)
	{
		$num  = round($num / 1073741824, $precision);
		$unit = lang('Number.gigabyteAbbr', [], $generalLocale);
	}
	elseif ($num >= 1000000)
	{
		$num  = round($num / 1048576, $precision);
		$unit = lang('Number.megabyteAbbr', [], $generalLocale);
	}
	elseif ($num >= 1000)
	{
		$num  = round($num / 1024, $precision);
		$unit = lang('Number.kilobyteAbbr', [], $generalLocale);
	}
	else
	{
		$unit = lang('Number.bytes', [], $generalLocale);
	}

	return format_number($num, $precision, $locale, ['after' => ' ' . $unit]);
}
```

</details>


<hr>

## number_to_amount()

```php
function number_to_amount($num, int $precision = 0, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts numbers to a more readable representation
when dealing with very large numbers (in the thousands or above),
up to the quadrillions, because you won't often deal with numbers
larger than that.
</td></tr>
</table>

<table>
<tr><td>
It uses the "short form" numbering system as this is most commonly
used within most English-speaking countries today.
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
<td><code>$num</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$precision</code></td>
<td><em>int
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
<td>bool<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 49 lines (127 - 175)</small></summary>

```php
function number_to_amount($num, int $precision = 0, string $locale = null)
{
	// Strip any formatting & ensure numeric input
	try
	{
		$num = 0 + str_replace(',', '', $num);
	}
	catch (\ErrorException $ee)
	{
		return false;
	}

	$suffix = '';

	// ignore sub part
	$generalLocale = $locale;
	if (! empty($locale) && ( $underscorePos = strpos($locale, '_')))
	{
		$generalLocale = substr($locale, 0, $underscorePos);
	}

	if ($num > 1000000000000000)
	{
		$suffix = lang('Number.quadrillion', [], $generalLocale);
		$num    = round(($num / 1000000000000000), $precision);
	}
	elseif ($num > 1000000000000)
	{
		$suffix = lang('Number.trillion', [], $generalLocale);
		$num    = round(($num / 1000000000000), $precision);
	}
	else if ($num > 1000000000)
	{
		$suffix = lang('Number.billion', [], $generalLocale);
		$num    = round(($num / 1000000000), $precision);
	}
	else if ($num > 1000000)
	{
		$suffix = lang('Number.million', [], $generalLocale);
		$num    = round(($num / 1000000), $precision);
	}
	else if ($num > 1000)
	{
		$suffix = lang('Number.thousand', [], $generalLocale);
		$num    = round(($num / 1000), $precision);
	}

	return format_number($num, $precision, $locale, ['after' => $suffix]);
}
```

</details>


<hr>

## number_to_currency()

```php
function number_to_currency(float $num, string $currency, string $locale = null, int $fraction = null) : string
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
<td><code>$num</code></td>
<td><em>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$currency</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$locale</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$fraction</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (190 - 197)</small></summary>

```php
function number_to_currency(float $num, string $currency, string $locale = null, int $fraction = null): string
{
	return format_number($num, 1, $locale, [
		'type'     => NumberFormatter::CURRENCY,
		'currency' => $currency,
		'fraction' => $fraction,
	]);
}
```

</details>


<hr>

## format_number()

```php
function format_number(float $num, int $precision = 1, string $locale = null, array $options = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A general purpose, locale-aware, number_format method.
</td></tr>
</table>

<table>
<tr><td>
Used by all of the functions of the number_helper.
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
<td><code>$num</code></td>
<td><em>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$precision</code></td>
<td><em>int
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

<tr>
<td>4.</td>
<td><code>$options</code></td>
<td><em>array
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
<summary><small>Source: 47 lines (215 - 261)</small></summary>

```php
function format_number(float $num, int $precision = 1, string $locale = null, array $options = []): string
{
	// Locale is either passed in here, negotiated with client, or grabbed from our config file.
	$locale = $locale ?? \Config\Services::request()->getLocale();

	// Type can be any of the NumberFormatter options, but provide a default.
	$type = (int) ($options['type'] ?? NumberFormatter::DECIMAL);

	$formatter = new NumberFormatter($locale, $type);

	// Try to format it per the locale
	if ($type === NumberFormatter::CURRENCY)
	{
		$formatter->setAttribute(NumberFormatter::FRACTION_DIGITS, $options['fraction']);
		$output = $formatter->formatCurrency($num, $options['currency']);
	}
	else
	{
		// In order to specify a precision, we'll have to modify
		// the pattern used by NumberFormatter.
		$pattern = '#,##0.' . str_repeat('#', $precision);

		$formatter->setPattern($pattern);
		$output = $formatter->format($num);
	}

	// This might lead a trailing period if $precision == 0
	$output = trim($output, '. ');

	if (intl_is_failure($formatter->getErrorCode()))
	{
		throw new BadFunctionCallException($formatter->getErrorMessage());
	}

	// Add on any before/after text.
	if (isset($options['before']) && is_string($options['before']))
	{
		$output = $options['before'] . $output;
	}

	if (isset($options['after']) && is_string($options['after']))
	{
		$output .= $options['after'];
	}

	return $output;
}
```

</details>


<hr>

## number_to_roman()

```php
function number_to_roman(string $num) : ?string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Convert a number to a roman numeral.
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
<td><code>$num</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>it will convert to int</td>
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
<summary><small>Source: 67 lines (275 - 341)</small></summary>

```php
function number_to_roman(string $num): ?string
{
	$num = (int) $num;
	if ($num < 1 || $num > 3999)
	{
		return null;
	}

	$_number_to_roman = function ($num, $th) use (&$_number_to_roman) {
		$return = '';
		$key1   = null;
		$key2   = null;
		switch ($th) {
			case 1:
				$key1  = 'I';
				$key2  = 'V';
				$key_f = 'X';
				break;
			case 2:
				$key1  = 'X';
				$key2  = 'L';
				$key_f = 'C';
				break;
			case 3:
				$key1  = 'C';
				$key2  = 'D';
				$key_f = 'M';
				break;
			case 4:
				$key1 = 'M';
				break;
		}
		$n = $num % 10;
		switch ($n) {
			case 1:
			case 2:
			case 3:
				$return = str_repeat($key1, $n);
				break;
			case 4:
				$return = $key1 . $key2;
				break;
			case 5:
				$return = $key2;
				break;
			case 6:
			case 7:
			case 8:
				$return = $key2 . str_repeat($key1, $n - 5);
				break;
			case 9:
				$return = $key1 . $key_f;
				break;
		}
		switch ($num) {
			case 10:
				$return = $key_f;
				break;
		}
		if ($num > 10)
		{
			$return = $_number_to_roman($num / 10, ++ $th) . $return;
		}
		return $return;
	};
	return $_number_to_roman($num, 1);
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/number_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/url_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/number_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:07**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>