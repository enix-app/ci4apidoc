


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/text_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/html_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/xml_helper.md">next</a></td>
</tr>
</table>




 



# Text Helper


<hr>

## word_limiter()

```php
function word_limiter(string $str, int $limit = 100, string $end_char = '&#8230;') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Word Limiter
</td></tr>
</table>

<table>
<tr><td>
Limits a string to X number of words.
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
<td><code>$str</code></td>
<td><em>string
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

<tr>
<td>3.</td>
<td><code>$end_char</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the end character. Usually an ellipsis</td>
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
<summary><small>Source: 16 lines (61 - 76)</small></summary>

```php
function word_limiter(string $str, int $limit = 100, string $end_char = '&#8230;'): string
{
	if (trim($str) === '')
	{
		return $str;
	}

	preg_match('/^\s*+(?:\S++\s*+){1,' . (int) $limit . '}/', $str, $matches);

	if (strlen($str) === strlen($matches[0]))
	{
		$end_char = '';
	}

	return rtrim($matches[0]) . $end_char;
}
```

</details>


<hr>

## character_limiter()

```php
function character_limiter(string $str, int $n = 500, string $end_char = '&#8230;') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Character Limiter
</td></tr>
</table>

<table>
<tr><td>
Limits the string based on the character count.  Preserves complete words
so the character count may not be exactly as specified.
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$n</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$end_char</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the end character. Usually an ellipsis</td>
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
<summary><small>Source: 28 lines (95 - 122)</small></summary>

```php
function character_limiter(string $str, int $n = 500, string $end_char = '&#8230;'): string
{
	if (mb_strlen($str) < $n)
	{
		return $str;
	}

	// a bit complicated, but faster than preg_replace with \s+
	$str = preg_replace('/ {2,}/', ' ', str_replace(["\r", "\n", "\t", "\x0B", "\x0C"], ' ', $str));

	if (mb_strlen($str) <= $n)
	{
		return $str;
	}

	$out = '';

	foreach (explode(' ', trim($str)) as $val)
	{
		$out .= $val . ' ';
		if (mb_strlen($out) >= $n)
		{
			$out = trim($out);
			break;
		}
	}
	return (mb_strlen($out) === mb_strlen($str)) ? $out : $out . $end_char;
}
```

</details>


<hr>

## ascii_to_entities()

```php
function ascii_to_entities(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
High ASCII to Entities
</td></tr>
</table>

<table>
<tr><td>
Converts high ASCII text and MS Word special characters to character entities
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
<td><code>$str</code></td>
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
<summary><small>Source: 48 lines (138 - 185)</small></summary>

```php
function ascii_to_entities(string $str): string
{
	$out = '';

	for ($i = 0, $s = strlen($str) - 1, $count = 1, $temp = []; $i <= $s; $i ++)
	{
		$ordinal = ord($str[$i]);

		if ($ordinal < 128)
		{
			/*
			  If the $temp array has a value but we have moved on, then it seems only
			  fair that we output that entity and restart $temp before continuing.
			 */
			if (count($temp) === 1)
			{
				$out  .= '&#' . array_shift($temp) . ';';
				$count = 1;
			}

			$out .= $str[$i];
		}
		else
		{
			if (empty($temp))
			{
				$count = ($ordinal < 224) ? 2 : 3;
			}

			$temp[] = $ordinal;

			if (count($temp) === $count)
			{
				$number = ($count === 3) ? (($temp[0] % 16) * 4096) + (($temp[1] % 64) * 64) + ($temp[2] % 64) : (($temp[0] % 32) * 64) + ($temp[1] % 64);
				$out   .= '&#' . $number . ';';
				$count  = 1;
				$temp   = [];
			}
			// If this is the last iteration, just output whatever we have
			elseif ($i === $s)
			{
				$out .= '&#' . implode(';', $temp) . ';';
			}
		}
	}

	return $out;
}
```

</details>


<hr>

## entities_to_ascii()

```php
function entities_to_ascii(string $str, bool $all = true) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Entities to ASCII
</td></tr>
</table>

<table>
<tr><td>
Converts character entities back to ASCII
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$all</code></td>
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
<summary><small>Source: 48 lines (202 - 249)</small></summary>

```php
function entities_to_ascii(string $str, bool $all = true): string
{
	if (preg_match_all('/\&#(\d+)\;/', $str, $matches))
	{
		for ($i = 0, $s = count($matches[0]); $i < $s; $i ++)
		{
			$digits = $matches[1][$i];
			$out    = '';
			if ($digits < 128)
			{
				$out .= chr($digits);
			}
			elseif ($digits < 2048)
			{
				$out .= chr(192 + (($digits - ($digits % 64)) / 64)) . chr(128 + ($digits % 64));
			}
			else
			{
				$out .= chr(224 + (($digits - ($digits % 4096)) / 4096))
						. chr(128 + ((($digits % 4096) - ($digits % 64)) / 64))
						. chr(128 + ($digits % 64));
			}
			$str = str_replace($matches[0][$i], $out, $str);
		}
	}

	if ($all)
	{
		return str_replace([
			'&amp;',
			'&lt;',
			'&gt;',
			'&quot;',
			'&apos;',
			'&#45;',
		], [
			'&',
			'<',
			'>',
			'"',
			"'",
			'-',
		], $str
		);
	}

	return $str;
}
```

</details>


<hr>

## word_censor()

```php
function word_censor(string $str, array $censored, string $replacement = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Word Censoring Function
</td></tr>
</table>

<table>
<tr><td>
Supply a string and an array of disallowed words and any
matched words will be converted to #### or to the replacement
word you've submitted.
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the text string</td>
</tr>

<tr>
<td>2.</td>
<td><code>$censored</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>the array of censored words</td>
</tr>

<tr>
<td>3.</td>
<td><code>$replacement</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the optional replacement value</td>
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
<summary><small>Source: 41 lines (269 - 309)</small></summary>

```php
function word_censor(string $str, array $censored, string $replacement = ''): string
{
	if (empty($censored))
	{
		return $str;
	}

	$str = ' ' . $str . ' ';

	// \w, \b and a few others do not match on a unicode character
	// set for performance reasons. As a result words like über
	// will not match on a word boundary. Instead, we'll assume that
	// a bad word will be bookended by any of these characters.
	$delim = '[-_\'\"`(){}<>\[\]|!?@#%&,.:;^~*+=\/ 0-9\n\r\t]';

	foreach ($censored as $badword)
	{
		$badword = str_replace('\*', '\w*?', preg_quote($badword, '/'));

		if ($replacement !== '')
		{
			$str = preg_replace(
					"/({$delim})(" . $badword . ")({$delim})/i", "\\1{$replacement}\\3", $str
			);
		}
		elseif (preg_match_all("/{$delim}(" . $badword . "){$delim}/i", $str, $matches, PREG_PATTERN_ORDER | PREG_OFFSET_CAPTURE))
		{
			$matches = $matches[1];

			for ($i = count($matches) - 1; $i >= 0; $i --)
			{
				$length = strlen($matches[$i][0]);
				$str    = substr_replace(
						$str, str_repeat('#', $length), $matches[$i][1], $length
				);
			}
		}
	}

	return trim($str);
}
```

</details>


<hr>

## highlight_code()

```php
function highlight_code(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Code Highlighter
</td></tr>
</table>

<table>
<tr><td>
Colorizes code strings
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the text string</td>
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
<summary><small>Source: 64 lines (325 - 388)</small></summary>

```php
function highlight_code(string $str): string
{
	/* The highlight string function encodes and highlights
	 * brackets so we need them to start raw.
	 *
	 * Also replace any existing PHP tags to temporary markers
	 * so they don't accidentally break the string out of PHP,
	 * and thus, thwart the highlighting.
	 */
	$str = str_replace([
		'&lt;',
		'&gt;',
		'<?',
		'?>',
		'<%',
		'%>',
		'\\',
		'</script>',
	], [
		'<',
		'>',
		'phptagopen',
		'phptagclose',
		'asptagopen',
		'asptagclose',
		'backslashtmp',
		'scriptclose',
	], $str
	);

	// The highlight_string function requires that the text be surrounded
	// by PHP tags, which we will remove later
	$str = highlight_string('<?php ' . $str . ' ?>', true);

	// Remove our artificially added PHP, and the syntax highlighting that came with it
	$str = preg_replace([
		'/<span style="color: #([A-Z0-9]+)">&lt;\?php(&nbsp;| )/i',
		'/(<span style="color: #[A-Z0-9]+">.*?)\?&gt;<\/span>\n<\/span>\n<\/code>/is',
		'/<span style="color: #[A-Z0-9]+"\><\/span>/i',
	], [
		'<span style="color: #$1">',
		"$1</span>\n</span>\n</code>",
		'',
	], $str
	);

	// Replace our markers back to PHP tags.
	return str_replace([
		'phptagopen',
		'phptagclose',
		'asptagopen',
		'asptagclose',
		'backslashtmp',
		'scriptclose',
	], [
		'&lt;?',
		'?&gt;',
		'&lt;%',
		'%&gt;',
		'\\',
		'&lt;/script&gt;',
	], $str
	);
}
```

</details>


<hr>

## highlight_phrase()

```php
function highlight_phrase(string $str, string $phrase, string $tag_open = '<mark>', string $tag_close = '</mark>') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Phrase Highlighter
</td></tr>
</table>

<table>
<tr><td>
Highlights a phrase within a text string
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the text string</td>
</tr>

<tr>
<td>2.</td>
<td><code>$phrase</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the phrase you'd like to highlight</td>
</tr>

<tr>
<td>3.</td>
<td><code>$tag_open</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the opening tag to precede the phrase with</td>
</tr>

<tr>
<td>4.</td>
<td><code>$tag_close</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the closing tag to end the phrase with</td>
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
<summary><small>Source: 4 lines (407 - 410)</small></summary>

```php
function highlight_phrase(string $str, string $phrase, string $tag_open = '<mark>', string $tag_close = '</mark>'): string
{
	return ($str !== '' && $phrase !== '') ? preg_replace('/(' . preg_quote($phrase, '/') . ')/i', $tag_open . '\\1' . $tag_close, $str) : $str;
}
```

</details>


<hr>

## convert_accented_characters()

```php
function convert_accented_characters(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Convert Accented Foreign Characters to ASCII
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Input string</td>
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
<summary><small>Source: 23 lines (424 - 446)</small></summary>

```php
function convert_accented_characters(string $str): string
{
	static $array_from, $array_to;

	if (! is_array($array_from))
	{
		$config = new Config\ForeignCharacters();

		if (empty($config->characterList) || ! is_array($config->characterList))
		{
			$array_from = [];
			$array_to   = [];

			return $str;
		}
		$array_from = array_keys($config->characterList);
		$array_to   = array_values($config->characterList);

		unset($config);
	}

	return preg_replace($array_from, $array_to, $str);
}
```

</details>


<hr>

## word_wrap()

```php
function word_wrap(string $str, int $charlim = 76) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Word Wrap
</td></tr>
</table>

<table>
<tr><td>
Wraps text at the specified character. Maintains the integrity of words.
Anything placed between {unwrap}{/unwrap} will not be word wrapped, nor
will URLs.
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the text string</td>
</tr>

<tr>
<td>2.</td>
<td><code>$charlim</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>= 76    the number of characters to wrap at</td>
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
<summary><small>Source: 85 lines (465 - 549)</small></summary>

```php
function word_wrap(string $str, int $charlim = 76): string
{
	// Set the character limit
	is_numeric($charlim) || $charlim = 76;

	// Reduce multiple spaces
	$str = preg_replace('| +|', ' ', $str);

	// Standardize newlines
	if (strpos($str, "\r") !== false)
	{
		$str = str_replace(["\r\n", "\r"], "\n", $str);
	}

	// If the current word is surrounded by {unwrap} tags we'll
	// strip the entire chunk and replace it with a marker.
	$unwrap = [];

	if (preg_match_all('|\{unwrap\}(.+?)\{/unwrap\}|s', $str, $matches))
	{
		for ($i = 0, $c = count($matches[0]); $i < $c; $i ++)
		{
			$unwrap[] = $matches[1][$i];
			$str      = str_replace($matches[0][$i], '{{unwrapped' . $i . '}}', $str);
		}
	}

	// Use PHP's native function to do the initial wordwrap.
	// We set the cut flag to FALSE so that any individual words that are
	// too long get left alone. In the next step we'll deal with them.
	$str = wordwrap($str, $charlim, "\n", false);

	// Split the string into individual lines of text and cycle through them
	$output = '';

	foreach (explode("\n", $str) as $line)
	{
		// Is the line within the allowed character count?
		// If so we'll join it to the output and continue
		if (mb_strlen($line) <= $charlim)
		{
			$output .= $line . "\n";
			continue;
		}

		$temp = '';

		while (mb_strlen($line) > $charlim)
		{
			// If the over-length word is a URL we won't wrap it
			if (preg_match('!\[url.+\]|://|www\.!', $line))
			{
				break;
			}
			// Trim the word down
			$temp .= mb_substr($line, 0, $charlim - 1);
			$line  = mb_substr($line, $charlim - 1);
		}

		// If $temp contains data it means we had to split up an over-length
		// word into smaller chunks so we'll add it back to our current line
		if ($temp !== '')
		{
			$output .= $temp . "\n" . $line . "\n";
		}
		else
		{
			$output .= $line . "\n";
		}
	}

	// Put our markers back
	if (! empty($unwrap))
	{
		foreach ($unwrap as $key => $val)
		{
			$output = str_replace('{{unwrapped' . $key . '}}', $val, $output);
		}
	}

	// remove any trailing newline
	$output = rtrim($output);

	return $output;
}
```

</details>


<hr>

## ellipsize()

```php
function ellipsize(string $str, int $max_length, $position = 1, string $ellipsis = '&hellip;') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ellipsize String
</td></tr>
</table>

<table>
<tr><td>
This function will strip tags from a string, split it at its max_length and ellipsize
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>String to ellipsize</td>
</tr>

<tr>
<td>2.</td>
<td><code>$max_length</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Max length of string</td>
</tr>

<tr>
<td>3.</td>
<td><code>$position</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>int (1|0) or float, .5, .2, etc for position to split</td>
</tr>

<tr>
<td>4.</td>
<td><code>$ellipsis</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>ellipsis ; Default '...'</td>
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
<summary><small>Source: 25 lines (568 - 592)</small></summary>

```php
function ellipsize(string $str, int $max_length, $position = 1, string $ellipsis = '&hellip;'): string
{
	// Strip tags
	$str = trim(strip_tags($str));

	// Is the string long enough to ellipsize?
	if (mb_strlen($str) <= $max_length)
	{
		return $str;
	}

	$beg      = mb_substr($str, 0, floor($max_length * $position));
	$position = ($position > 1) ? 1 : $position;

	if ($position === 1)
	{
		$end = mb_substr($str, 0, -($max_length - mb_strlen($beg)));
	}
	else
	{
		$end = mb_substr($str, -($max_length - mb_strlen($beg)));
	}

	return $beg . $ellipsis . $end;
}
```

</details>


<hr>

## strip_slashes()

```php
function strip_slashes($str)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Strip Slashes
</td></tr>
</table>

<table>
<tr><td>
Removes slashes contained in a string or in an array
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
<td><code>$str</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>string or array</td>
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
<summary><small>Source: 13 lines (608 - 620)</small></summary>

```php
function strip_slashes($str)
{
	if (! is_array($str))
	{
		return stripslashes($str);
	}
	foreach ($str as $key => $val)
	{
		$str[$key] = strip_slashes($val);
	}

	return $str;
}
```

</details>


<hr>

## strip_quotes()

```php
function strip_quotes(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Strip Quotes
</td></tr>
</table>

<table>
<tr><td>
Removes single and double quotes from a string
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (636 - 639)</small></summary>

```php
function strip_quotes(string $str): string
{
	return str_replace(['"', "'"], '', $str);
}
```

</details>


<hr>

## quotes_to_entities()

```php
function quotes_to_entities(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Quotes to Entities
</td></tr>
</table>

<table>
<tr><td>
Converts single and double quotes to entities
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (655 - 658)</small></summary>

```php
function quotes_to_entities(string $str): string
{
	return str_replace(["\'", '"', "'", '"'], ['&#39;', '&quot;', '&#39;', '&quot;'], $str);
}
```

</details>


<hr>

## reduce_double_slashes()

```php
function reduce_double_slashes(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reduce Double Slashes
</td></tr>
</table>

<table>
<tr><td>
Converts double slashes in a string to a single slash,
except those found in http://

<a href="http://www.some-site.com//index.php">http://www.some-site.com//index.php</a>

becomes:

<a href="http://www.some-site.com/index.php">http://www.some-site.com/index.php</a>
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (681 - 684)</small></summary>

```php
function reduce_double_slashes(string $str): string
{
	return preg_replace('#(^|[^:])//+#', '\\1/', $str);
}
```

</details>


<hr>

## reduce_multiples()

```php
function reduce_multiples(string $str, string $character = ',', bool $trim = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reduce Multiples
</td></tr>
</table>

<table>
<tr><td>
Reduces multiple instances of a particular character.  Example:

Fred, Bill,, Joe, Jimmy

becomes:

Fred, Bill, Joe, Jimmy
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$character</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the character you wish to reduce</td>
</tr>

<tr>
<td>3.</td>
<td><code>$trim</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>TRUE/FALSE - whether to trim the character from the beginning/end</td>
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
<summary><small>Source: 6 lines (708 - 713)</small></summary>

```php
function reduce_multiples(string $str, string $character = ',', bool $trim = false): string
{
	$str = preg_replace('#' . preg_quote($character, '#') . '{2,}#', $character, $str);

	return ($trim) ? trim($str, $character) : $str;
}
```

</details>


<hr>

## random_string()

```php
function random_string(string $type = 'alnum', int $len = 8) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create a Random String
</td></tr>
</table>

<table>
<tr><td>
Useful for generating passwords or hashes.
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
<td><code>$type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Type of random string.  basic, alpha, alnum, numeric, nozero, md5, sha1, and crypto</td>
</tr>

<tr>
<td>2.</td>
<td><code>$len</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Number of characters</td>
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
<summary><small>Source: 35 lines (730 - 764)</small></summary>

```php
function random_string(string $type = 'alnum', int $len = 8): string
{
	switch ($type)
	{
		case 'alnum':
		case 'numeric':
		case 'nozero':
		case 'alpha':
			switch ($type)
			{
				case 'alpha':
					$pool = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ';
					break;
				case 'alnum':
					$pool = '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ';
					break;
				case 'numeric':
					$pool = '0123456789';
					break;
				case 'nozero':
					$pool = '123456789';
					break;
			}

			return substr(str_shuffle(str_repeat($pool, ceil($len / strlen($pool)))), 0, $len);
		case 'md5':
			return md5(uniqid(mt_rand(), true));
		case 'sha1':
			return sha1(uniqid(mt_rand(), true));
		case 'crypto':
			return bin2hex(random_bytes($len / 2));
	}
	// 'basic' type treated as default
	return (string) mt_rand();
}
```

</details>


<hr>

## increment_string()

```php
function increment_string(string $str, string $separator = '_', int $first = 1) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add's _1 to a string or increment the ending number to allow _2, _3, etc
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Required</td>
</tr>

<tr>
<td>2.</td>
<td><code>$separator</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>What should the duplicate number be appended with</td>
</tr>

<tr>
<td>3.</td>
<td><code>$first</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Which number should be used for the first dupe increment</td>
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
<summary><small>Source: 6 lines (780 - 785)</small></summary>

```php
function increment_string(string $str, string $separator = '_', int $first = 1): string
{
	preg_match('/(.+)' . preg_quote($separator, '/') . '([0-9]+)$/', $str, $match);

	return isset($match[2]) ? $match[1] . $separator . ($match[2] + 1) : $str . $separator . $first;
}
```

</details>


<hr>

## alternator()

```php
function alternator() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alternator
</td></tr>
</table>

<table>
<tr><td>
Allows strings to be alternated. See docs...
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
<td><code>$</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>(as many parameters as needed)</td>
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
<summary><small>Source: 15 lines (801 - 815)</small></summary>

```php
function alternator(): string
{
	static $i;

	if (func_num_args() === 0)
	{
		$i = 0;

		return '';
	}

	$args = func_get_args();

	return $args[($i++ % count($args))];
}
```

</details>


<hr>

## excerpt()

```php
function excerpt(string $text, string $phrase = null, int $radius = 100, string $ellipsis = '...') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Excerpt.
</td></tr>
</table>

<table>
<tr><td>
Allows to extract a piece of text surrounding a word or phrase.
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
<td><code>$text</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>String to search the phrase</td>
</tr>

<tr>
<td>2.</td>
<td><code>$phrase</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Phrase that will be searched for.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$radius</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The amount of characters returned around the phrase.</td>
</tr>

<tr>
<td>4.</td>
<td><code>$ellipsis</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Ending that will be appended</td>
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
<summary><small>Source: 44 lines (837 - 880)</small></summary>

```php
function excerpt(string $text, string $phrase = null, int $radius = 100, string $ellipsis = '...'): string
{
	if (isset($phrase))
	{
		$phrasePos = stripos($text, $phrase);
		$phraseLen = strlen($phrase);
	}
	elseif (! isset($phrase))
	{
		$phrasePos = $radius / 2;
		$phraseLen = 1;
	}

	$pre = explode(' ', substr($text, 0, $phrasePos));
	$pos = explode(' ', substr($text, $phrasePos + $phraseLen));

	$prev  = ' ';
	$post  = ' ';
	$count = 0;

	foreach (array_reverse($pre) as $e)
	{
		if ((strlen($e) + $count + 1) < $radius)
		{
			$prev = ' ' . $e . $prev;
		}
		$count = ++ $count + strlen($e);
	}

	$count = 0;

	foreach ($pos as $s)
	{
		if ((strlen($s) + $count + 1) < $radius)
		{
			$post .= $s . ' ';
		}
		$count = ++ $count + strlen($s);
	}

	$ellPre = $phrase ? $ellipsis : '';

	return str_replace('  ', ' ', $ellPre . $prev . $phrase . $post . $ellipsis);
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/text_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/html_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/xml_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:06**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>