


 



<table>
<tr>
<td style="width:100%"><em>framework/system/View/Filters.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Parser.md">next</a></td>
</tr>
</table>







# CodeIgniter\View 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\View</td></tr>
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
<td>framework/system/View/Filters.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Cell.md">CodeIgniter\View\Cell</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md">CodeIgniter\View\Exceptions\ViewException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Filters.md">CodeIgniter\View\Filters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Parser.md">CodeIgniter\View\Parser</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Plugins.md">CodeIgniter\View\Plugins</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">CodeIgniter\View\RendererInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Table.md">CodeIgniter\View\Table</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/View.md">CodeIgniter\View\View</a></td></tr>
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
<tr>
<td>
<strong>NumberFormatter</strong>
</td>
<td>NumberFormatter</td>
</tr>
</table>



 
## CodeIgniter\View\Filters

<table style="text-align:left">
<tr><th>Class</th><td>Filters</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\View\Filters</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
View filters
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
<th><a href="#capitalize"><strong>capitalize</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns $value as all lowercase with the first letter capitalized.</td>
</tr>
<tr>
<th><a href="#date"><strong>date</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Formats a date into the given $format.</td>
</tr>
<tr>
<th><a href="#date_modify"><strong>date_modify</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Given a string or DateTime object, will return the date modified
by the given value. Returns the value as a unix timestamp</td>
</tr>
<tr>
<th><a href="#default"><strong>default</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns the given default value if $value is empty or undefined.</td>
</tr>
<tr>
<th><a href="#esc"><strong>esc</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Escapes the given value with our `esc()` helper function.</td>
</tr>
<tr>
<th><a href="#excerpt"><strong>excerpt</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns an excerpt of the given string.</td>
</tr>
<tr>
<th><a href="#highlight"><strong>highlight</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Highlights a given phrase within the text using &#039;&lt;mark&gt;&lt;/mark&gt;&#039; tags.</td>
</tr>
<tr>
<th><a href="#highlight_code"><strong>highlight_code</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Highlights code samples with HTML/CSS.</td>
</tr>
<tr>
<th><a href="#limit_chars"><strong>limit_chars</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Limits the number of characters to $limit, and trails of with an ellipsis.</td>
</tr>
<tr>
<th><a href="#limit_words"><strong>limit_words</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Limits the number of words to $limit, and trails of with an ellipsis.</td>
</tr>
<tr>
<th><a href="#local_number"><strong>local_number</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns the $value displayed in a localized manner.</td>
</tr>
<tr>
<th><a href="#local_currency"><strong>local_currency</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns the $value displayed as a currency string.</td>
</tr>
<tr>
<th><a href="#nl2br"><strong>nl2br</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a string with all instances of newline character (\n)
converted to an HTML &lt;br/&gt; tag.</td>
</tr>
<tr>
<th><a href="#prose"><strong>prose</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Takes a body of text and uses the auto_typography() method to
turn it into prettier, easier-to-read, prose.</td>
</tr>
<tr>
<th><a href="#round"><strong>round</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Rounds a given $value in one of 3 ways;</td>
</tr>
<tr>
<th><a href="#title"><strong>title</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a &quot;title case&quot; version of the string.</td>
</tr>

</table>






### Methods


<hr>

#### capitalize()

```php
public static function capitalize(string $value) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns $value as all lowercase with the first letter capitalized.
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (57 - 60)</small></summary>

```php
public static function capitalize(string $value): string
{
	return ucfirst(strtolower($value));
}
```

</details>


<hr>

#### date()

```php
public static function date($value, string $format) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Formats a date into the given $format.
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$format</code></td>
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
<summary><small>Source: 9 lines (72 - 80)</small></summary>

```php
public static function date($value, string $format): string
{
	if (is_string($value) && ! is_numeric($value))
	{
		$value = strtotime($value);
	}

	return date($format, $value);
}
```

</details>


<hr>

#### date_modify()

```php
public static function date_modify($value, string $adjustment) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Given a string or DateTime object, will return the date modified
by the given value. Returns the value as a unix timestamp
</td></tr>
</table>

<table>
<tr><td>
Example:
my_date|date_modify(+1 day)
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>internal</th>
<td>param string $format
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
<td><code>$value</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$adjustment</code></td>
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
<summary><small>Source: 6 lines (97 - 102)</small></summary>

```php
public static function date_modify($value, string $adjustment): string
{
	$value = static::date($value, 'Y-m-d H:i:s');

	return strtotime($adjustment, strtotime($value));
}
```

</details>


<hr>

#### default()

```php
public static function default($value, string $default) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the given default value if $value is empty or undefined.
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$default</code></td>
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
<summary><small>Source: 6 lines (114 - 119)</small></summary>

```php
public static function default($value, string $default): string
{
	return empty($value)
		? $default
		: $value;
}
```

</details>


<hr>

#### esc()

```php
public static function esc($value, string $context = 'html') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Escapes the given value with our `esc()` helper function.
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$context</code></td>
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
<summary><small>Source: 4 lines (131 - 134)</small></summary>

```php
public static function esc($value, string $context = 'html'): string
{
	return esc($value, $context);
}
```

</details>


<hr>

#### excerpt()

```php
public static function excerpt(string $value, string $phrase, int $radius = 100) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an excerpt of the given string.
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
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$phrase</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$radius</code></td>
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
<summary><small>Source: 6 lines (147 - 152)</small></summary>

```php
public static function excerpt(string $value, string $phrase, int $radius = 100): string
{
	helper('text');

	return excerpt($value, $phrase, $radius);
}
```

</details>


<hr>

#### highlight()

```php
public static function highlight(string $value, string $phrase) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Highlights a given phrase within the text using '<mark></mark>' tags.
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
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$phrase</code></td>
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
<summary><small>Source: 6 lines (164 - 169)</small></summary>

```php
public static function highlight(string $value, string $phrase): string
{
	helper('text');

	return highlight_phrase($value, $phrase);
}
```

</details>


<hr>

#### highlight_code()

```php
public static function highlight_code($value) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Highlights code samples with HTML/CSS.
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (180 - 185)</small></summary>

```php
public static function highlight_code($value): string
{
	helper('text');

	return highlight_code($value);
}
```

</details>


<hr>

#### limit_chars()

```php
public static function limit_chars($value, int $limit = 500) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Limits the number of characters to $limit, and trails of with an ellipsis.
</td></tr>
</table>

<table>
<tr><td>
Will break at word break so may be more or less than $limit.
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$limit</code></td>
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
<summary><small>Source: 6 lines (198 - 203)</small></summary>

```php
public static function limit_chars($value, int $limit = 500): string
{
	helper('text');

	return character_limiter($value, $limit);
}
```

</details>


<hr>

#### limit_words()

```php
public static function limit_words($value, int $limit = 100) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Limits the number of words to $limit, and trails of with an ellipsis.
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$limit</code></td>
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
<summary><small>Source: 6 lines (215 - 220)</small></summary>

```php
public static function limit_words($value, int $limit = 100): string
{
	helper('text');

	return word_limiter($value, $limit);
}
```

</details>


<hr>

#### local_number()

```php
public static function local_number($value, string $type = 'decimal', int $precision = 4, string $locale = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the $value displayed in a localized manner.
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
<td><em>
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
<td><code>$type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
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
<summary><small>Source: 16 lines (234 - 249)</small></summary>

```php
public static function local_number($value, string $type = 'decimal', int $precision = 4, string $locale = null): string
{
	helper('number');

	$types = [
		'decimal'    => NumberFormatter::DECIMAL,
		'currency'   => NumberFormatter::CURRENCY,
		'percent'    => NumberFormatter::PERCENT,
		'scientific' => NumberFormatter::SCIENTIFIC,
		'spellout'   => NumberFormatter::SPELLOUT,
		'ordinal'    => NumberFormatter::ORDINAL,
		'duration'   => NumberFormatter::DURATION,
	];

	return format_number($value, $precision, $locale, ['type' => $types[$type]]);
}
```

</details>


<hr>

#### local_currency()

```php
public static function local_currency($value, string $currency, string $locale = null, $fraction = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the $value displayed as a currency string.
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
<td><em>
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
<td><em>string<br>null
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
<summary><small>Source: 12 lines (263 - 274)</small></summary>

```php
public static function local_currency($value, string $currency, string $locale = null, $fraction = null): string
{
	helper('number');

	$options = [
		'type'     => NumberFormatter::CURRENCY,
		'currency' => $currency,
		'fraction' => $fraction,
	];

	return format_number($value, 2, $locale, $options);
}
```

</details>


<hr>

#### nl2br()

```php
public static function nl2br(string $value) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a string with all instances of newline character (\n)
converted to an HTML <br/> tag.
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
<summary><small>Source: 6 lines (284 - 289)</small></summary>

```php
public static function nl2br(string $value): string
{
	$typography = Services::typography();

	return $typography->nl2brExceptPre($value);
}
```

</details>


<hr>

#### prose()

```php
public static function prose(string $value) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes a body of text and uses the auto_typography() method to
turn it into prettier, easier-to-read, prose.
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
<summary><small>Source: 6 lines (301 - 306)</small></summary>

```php
public static function prose(string $value): string
{
	$typography = Services::typography();

	return $typography->autoTypography($value);
}
```

</details>


<hr>

#### round()

```php
public static function round(string $value, $precision = 2, string $type = 'common') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Rounds a given $value in one of 3 ways;
</td></tr>
</table>

<table>
<tr><td>
- common    Normal rounding
- ceil      always rounds up
- floor     always rounds down
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
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$precision</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$type</code></td>
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
<summary><small>Source: 21 lines (323 - 343)</small></summary>

```php
public static function round(string $value, $precision = 2, string $type = 'common'): string
{
	if (! is_numeric($precision))
	{
		$type      = $precision;
		$precision = 2;
	}

	switch ($type)
	{
		case 'common':
			return round($value, $precision);
		case 'ceil':
			return ceil($value);
		case 'floor':
			return floor($value);
	}

	// Still here, just return the value.
	return $value;
}
```

</details>


<hr>

#### title()

```php
public static function title(string $value) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a "title case" version of the string.
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
<summary><small>Source: 4 lines (354 - 357)</small></summary>

```php
public static function title(string $value): string
{
	return ucwords(strtolower($value));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/View/Filters.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Parser.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>