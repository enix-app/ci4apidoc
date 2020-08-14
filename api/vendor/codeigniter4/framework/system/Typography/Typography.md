


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Typography/Typography.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/ThrottlerInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/CreditCardRules.md">next</a></td>
</tr>
</table>







# CodeIgniter\Typography 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Typography</td></tr>
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
<td>framework/system/Typography/Typography.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Typography/Typography.md">CodeIgniter\Typography\Typography</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Typography\Typography

<table style="text-align:left">
<tr><th>Class</th><td>Typography</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Typography\Typography</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Typography Class
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
<th><a href="#blockElements"><strong>blockElements</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Block level elements that should not be wrapped inside &lt;p&gt; tags</td>
</tr>
<tr>
<th><a href="#skipElements"><strong>skipElements</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Elements that should not have &lt;p&gt; and &lt;br /&gt; tags within them.</td>
</tr>
<tr>
<th><a href="#inlineElements"><strong>inlineElements</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Tags we want the parser to completely ignore when splitting the string.</td>
</tr>
<tr>
<th><a href="#innerBlockRequired"><strong>innerBlockRequired</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>array of block level elements that require inner content to be within another block level element</td>
</tr>
<tr>
<th><a href="#lastBlockElement"><strong>lastBlockElement</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>the last block element parsed</td>
</tr>
<tr>
<th><a href="#protectBracedQuotes"><strong>protectBracedQuotes</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>whether or not to protect quotes within { curly braces }</td>
</tr>

<tr>
<th><a href="#autoTypography"><strong>autoTypography</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Auto Typography</td>
</tr>
<tr>
<th><a href="#formatCharacters"><strong>formatCharacters</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Format Characters</td>
</tr>
<tr>
<th><a href="#formatNewLines"><strong>formatNewLines</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Format Newlines</td>
</tr>
<tr>
<th><a href="#protectCharacters"><strong>protectCharacters</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Protect Characters</td>
</tr>
<tr>
<th><a href="#nl2brExceptPre"><strong>nl2brExceptPre</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Convert newlines to HTML line breaks except within PRE tags</td>
</tr>

</table>





### Properties


<hr>

#### $blockElements

```php
public $blockElements = 'address|blockquote|div|dl|fieldset|form|h\d|hr|noscript|object|ol|p|pre|script|table|ul';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Block level elements that should not be wrapped inside <p> tags
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

#### $skipElements

```php
public $skipElements = 'p|pre|ol|ul|dl|object|table|h\d';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Elements that should not have <p> and <br /> tags within them.
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

#### $inlineElements

```php
public $inlineElements = 'a|abbr|acronym|b|bdo|big|br|button|cite|code|del|dfn|em|i|img|ins|input|label|map|kbd|q|samp|select|small|span|strong|sub|sup|textarea|tt|var';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Tags we want the parser to completely ignore when splitting the string.
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

#### $innerBlockRequired

```php
public $innerBlockRequired = ['blockquote'];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
array of block level elements that require inner content to be within another block level element
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

#### $lastBlockElement

```php
public $lastBlockElement = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
the last block element parsed
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

#### $protectBracedQuotes

```php
public $protectBracedQuotes = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
whether or not to protect quotes within { curly braces }
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







### Methods


<hr>

#### autoTypography()

```php
public function autoTypography(string $str, bool $reduce_linebreaks = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Auto Typography
</td></tr>
</table>

<table>
<tr><td>
This function converts text, making it typographically correct:
   - Converts double spaces into paragraphs.
   - Converts single line breaks into <br /> tags
   - Converts single and double quotes into correctly facing curly quote entities.
   - Converts three dots into ellipsis.
   - Converts double dashes into em-dashes.
- Converts two spaces into entities
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
<td><code>$reduce_linebreaks</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>whether to reduce more then two consecutive newlines to two</td>
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
<summary><small>Source: 164 lines (106 - 269)</small></summary>

```php
public function autoTypography(string $str, bool $reduce_linebreaks = false): string
{
	if ($str === '')
	{
		return '';
	}

	// Standardize Newlines to make matching easier
	if (strpos($str, "\r") !== false)
	{
		$str = str_replace(["\r\n", "\r"], "\n", $str);
	}

	// Reduce line breaks.  If there are more than two consecutive linebreaks
	// we'll compress them down to a maximum of two since there's no benefit to more.
	if ($reduce_linebreaks === false)
	{
		$str = preg_replace("/\n\n+/", "\n\n", $str);
	}

	// HTML comment tags don't conform to patterns of normal tags, so pull them out separately, only if needed
	$html_comments = [];
	if (strpos($str, '<!--') !== false && preg_match_all('#(<!\-\-.*?\-\->)#s', $str, $matches))
	{
		for ($i = 0, $total = count($matches[0]); $i < $total; $i ++)
		{
			$html_comments[] = $matches[0][$i];
			$str             = str_replace($matches[0][$i], '{@HC' . $i . '}', $str);
		}
	}

	// match and yank <pre> tags if they exist.  It's cheaper to do this separately since most content will
	// not contain <pre> tags, and it keeps the PCRE patterns below simpler and faster
	if (strpos($str, '<pre') !== false)
	{
		$str = preg_replace_callback('#<pre.*?>.*?</pre>#si', [$this, 'protectCharacters'], $str);
	}

	// Convert quotes within tags to temporary markers.
	$str = preg_replace_callback('#<.+?>#si', [$this, 'protectCharacters'], $str);

	// Do the same with braces if necessary
	if ($this->protectBracedQuotes === false)
	{
		$str = preg_replace_callback('#\{.+?\}#si', [$this, 'protectCharacters'], $str);
	}

	// Convert "ignore" tags to temporary marker.  The parser splits out the string at every tag
	// it encounters.  Certain inline tags, like image tags, links, span tags, etc. will be
	// adversely affected if they are split out so we'll convert the opening bracket < temporarily to: {@TAG}
	$str = preg_replace('#<(/*)(' . $this->inlineElements . ')([ >])#i', '{@TAG}\\1\\2\\3', $str);

	/* Split the string at every tag. This expression creates an array with this prototype:
	 *
	 * 	[array]
	 * 	{
	 * 		[0] = <opening tag>
	 * 		[1] = Content...
	 * 		[2] = <closing tag>
	 * 		Etc...
	 * 	}
	 */
	$chunks = preg_split('/(<(?:[^<>]+(?:"[^"]*"|\'[^\']*\')?)+>)/', $str, -1, PREG_SPLIT_DELIM_CAPTURE | PREG_SPLIT_NO_EMPTY);

	// Build our finalized string.  We cycle through the array, skipping tags, and processing the contained text
	$str     = '';
	$process = true;

	for ($i = 0, $c = count($chunks) - 1; $i <= $c; $i ++)
	{
		// Are we dealing with a tag? If so, we'll skip the processing for this cycle.
		// Well also set the "process" flag which allows us to skip <pre> tags and a few other things.
		if (preg_match('#<(/*)(' . $this->blockElements . ').*?>#', $chunks[$i], $match))
		{
			if (preg_match('#' . $this->skipElements . '#', $match[2]))
			{
				$process = ($match[1] === '/');
			}

			if ($match[1] === '')
			{
				$this->lastBlockElement = $match[2];
			}

			$str .= $chunks[$i];
			continue;
		}

		if ($process === false)
		{
			$str .= $chunks[$i];
			continue;
		}

		//  Force a newline to make sure end tags get processed by _format_newlines()
		if ($i === $c)
		{
			$chunks[$i] .= "\n";
		}

		//  Convert Newlines into <p> and <br /> tags
		$str .= $this->formatNewLines($chunks[$i]);
	}

	// No opening block level tag? Add it if needed.
	if (! preg_match('/^\s*<(?:' . $this->blockElements . ')/i', $str))
	{
		$str = preg_replace('/^(.*?)<(' . $this->blockElements . ')/i', '<p>$1</p><$2', $str);
	}

	// Convert quotes, elipsis, em-dashes, non-breaking spaces, and ampersands
	$str = $this->formatCharacters($str);

	// restore HTML comments
	for ($i = 0, $total = count($html_comments); $i < $total; $i ++)
	{
		// remove surrounding paragraph tags, but only if there's an opening paragraph tag
		// otherwise HTML comments at the ends of paragraphs will have the closing tag removed
		// if '<p>{@HC1}' then replace <p>{@HC1}</p> with the comment, else replace only {@HC1} with the comment
		$str = preg_replace('#(?(?=<p>\{@HC' . $i . '\})<p>\{@HC' . $i . '\}(\s*</p>)|\{@HC' . $i . '\})#s', $html_comments[$i], $str);
	}

	// Final clean up
	$table = [
		// If the user submitted their own paragraph tags within the text
		// we will retain them instead of using our tags.
		'/(<p[^>*?]>)<p>/'                              => '$1', // <?php BBEdit syntax coloring bug fix
		// Reduce multiple instances of opening/closing paragraph tags to a single one
		'#(</p>)+#'                                     => '</p>',
		'/(<p>\W*<p>)+/'                                => '<p>',
		// Clean up stray paragraph tags that appear before block level elements
		'#<p></p><(' . $this->blockElements . ')#'      => '<$1',
		// Clean up stray non-breaking spaces preceeding block elements
		'#(&nbsp;\s*)+<(' . $this->blockElements . ')#' => '  <$2',
		// Replace the temporary markers we added earlier
		'/\{@TAG\}/'                                    => '<',
		'/\{@DQ\}/'                                     => '"',
		'/\{@SQ\}/'                                     => "'",
		'/\{@DD\}/'                                     => '--',
		'/\{@NBS\}/'                                    => '  ',
		// An unintended consequence of the _format_newlines function is that
		// some of the newlines get truncated, resulting in <p> tags
		// starting immediately after <block> tags on the same line.
		// This forces a newline after such occurrences, which looks much nicer.
		"/><p>\n/"                                      => ">\n<p>",
		// Similarly, there might be cases where a closing </block> will follow
		// a closing </p> tag, so we'll correct it by adding a newline in between
		'#</p></#'                                      => "</p>\n</",
	];

	// Do we need to reduce empty lines?
	if ($reduce_linebreaks === true)
	{
		$table['#<p>\n*</p>#'] = '';
	}
	else
	{
		// If we have empty paragraph tags we add a non-breaking space
		// otherwise most browsers won't treat them as true paragraphs
		$table['#<p></p>#'] = '<p>&nbsp;</p>';
	}

	return preg_replace(array_keys($table), $table, $str);
}
```

</details>


<hr>

#### formatCharacters()

```php
public function formatCharacters(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Format Characters
</td></tr>
</table>

<table>
<tr><td>
This function mainly converts double and single quotes
to curly entities, but it also converts em-dashes,
double spaces, and ampersands
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
<summary><small>Source: 46 lines (283 - 328)</small></summary>

```php
public function formatCharacters(string $str): string
{
	static $table;

	if (! isset($table))
	{
		$table = [
			// nested smart quotes, opening and closing
			// note that rules for grammar (English) allow only for two levels deep
			// and that single quotes are _supposed_ to always be on the outside
			// but we'll accommodate both
			// Note that in all cases, whitespace is the primary determining factor
			// on which direction to curl, with non-word characters like punctuation
			// being a secondary factor only after whitespace is addressed.
			'/\'"(\s|$)/'               => '&#8217;&#8221;$1',
			'/(^|\s|<p>)\'"/'           => '$1&#8216;&#8220;',
			'/\'"(\W)/'                 => '&#8217;&#8221;$1',
			'/(\W)\'"/'                 => '$1&#8216;&#8220;',
			'/"\'(\s|$)/'               => '&#8221;&#8217;$1',
			'/(^|\s|<p>)"\'/'           => '$1&#8220;&#8216;',
			'/"\'(\W)/'                 => '&#8221;&#8217;$1',
			'/(\W)"\'/'                 => '$1&#8220;&#8216;',
			// single quote smart quotes
			'/\'(\s|$)/'                => '&#8217;$1',
			'/(^|\s|<p>)\'/'            => '$1&#8216;',
			'/\'(\W)/'                  => '&#8217;$1',
			'/(\W)\'/'                  => '$1&#8216;',
			// double quote smart quotes
			'/"(\s|$)/'                 => '&#8221;$1',
			'/(^|\s|<p>)"/'             => '$1&#8220;',
			'/"(\W)/'                   => '&#8221;$1',
			'/(\W)"/'                   => '$1&#8220;',
			// apostrophes
			"/(\w)'(\w)/"               => '$1&#8217;$2',
			// Em dash and ellipses dots
			'/\s?\-\-\s?/'              => '&#8212;',
			'/(\w)\.{3}/'               => '$1&#8230;',
			// double space after sentences
			'/(\W)  /'                  => '$1&nbsp; ',
			// ampersands, if not a character entity
			'/&(?!#?[a-zA-Z0-9]{2,};)/' => '&amp;',
		];
	}

	return preg_replace(array_keys($table), $table, $str);
}
```

</details>


<hr>

#### formatNewLines()

```php
protected function formatNewLines(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Format Newlines
</td></tr>
</table>

<table>
<tr><td>
Converts newline characters into either <p> tags or <br />
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
<summary><small>Source: 26 lines (340 - 365)</small></summary>

```php
protected function formatNewLines(string $str): string
{
	if ($str === '' || ( strpos($str, "\n") === false && ! in_array($this->lastBlockElement, $this->innerBlockRequired)))
	{
		return $str;
	}

	// Convert two consecutive newlines to paragraphs
	$str = str_replace("\n\n", "</p>\n\n<p>", $str);

	// Convert single spaces to <br /> tags
	$str = preg_replace("/([^\n])(\n)([^\n])/", '\\1<br />\\2\\3', $str);

	// Wrap the whole enchilada in enclosing paragraphs
	if ($str !== "\n")
	{
		// We trim off the right-side new line so that the closing </p> tag
		// will be positioned immediately following the string, matching
		// the behavior of the opening <p> tag
		$str = '<p>' . rtrim($str) . '</p>';
	}

	// Remove empty paragraphs if they are on the first line, as this
	// is a potential unintended consequence of the previous code
	return preg_replace('/<p><\/p>(.*)/', '\\1', $str, 1);
}
```

</details>


<hr>

#### protectCharacters()

```php
protected function protectCharacters(array $match) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Protect Characters
</td></tr>
</table>

<table>
<tr><td>
Protects special characters from being formatted later
We don't want quotes converted within tags so we'll temporarily convert them to %1$s and %2$s
and we don't want double dashes converted to emdash entities, so they are marked with %3$s
likewise double spaces are converted to %4$s to prevent entity conversion
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
<td><code>$match</code></td>
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
<summary><small>Source: 4 lines (380 - 383)</small></summary>

```php
protected function protectCharacters(array $match): string
{
	return str_replace(["'", '"', '--', '  '], ['{@SQ}', '{@DQ}', '{@DD}', '{@NBS}'], $match[0]);
}
```

</details>


<hr>

#### nl2brExceptPre()

```php
public function nl2brExceptPre(string $str) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Convert newlines to HTML line breaks except within PRE tags
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
<summary><small>Source: 14 lines (393 - 406)</small></summary>

```php
public function nl2brExceptPre(string $str): string
{
	$newstr = '';
	for ($ex = explode('pre>', $str), $ct = count($ex), $i = 0; $i < $ct; $i ++)
	{
		$newstr .= (($i % 2) === 0) ? nl2br($ex[$i]) : $ex[$i];
		if ($ct - 1 !== $i)
		{
			$newstr .= 'pre>';
		}
	}

	return $newstr;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Typography/Typography.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Throttle/ThrottlerInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/CreditCardRules.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>