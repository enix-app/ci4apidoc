


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/html_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/form_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/html_helper.md">next</a></td>
</tr>
</table>




 



# HTML Helper


<hr>

## ul()

```php
function ul(array $list, $attributes = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Unordered List
</td></tr>
</table>

<table>
<tr><td>
Generates an HTML unordered list from an single or
multi-dimensional array.
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
<td><code>$list</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$attributes</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>HTML attributes string, array, object</td>
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
<summary><small>Source: 4 lines (60 - 63)</small></summary>

```php
function ul(array $list, $attributes = ''): string
{
	return _list('ul', $list, $attributes);
}
```

</details>


<hr>

## ol()

```php
function ol(array $list, $attributes = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ordered List
</td></tr>
</table>

<table>
<tr><td>
Generates an HTML ordered list from an single or multi-dimensional array.
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
<td><code>$list</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$attributes</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>HTML attributes string, array, object</td>
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
<summary><small>Source: 4 lines (80 - 83)</small></summary>

```php
function ol(array $list, $attributes = ''): string
{
	return _list('ol', $list, $attributes);
}
```

</details>


<hr>

## _list()

```php
function _list(string $type = 'ul', $list = array(), $attributes = '', int $depth = 0) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates the list
</td></tr>
</table>

<table>
<tr><td>
Generates an HTML ordered list from an single or multi-dimensional array.
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
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$list</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>string, array, object</td>
</tr>

<tr>
<td>4.</td>
<td><code>$depth</code></td>
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
<summary><small>Source: 35 lines (102 - 136)</small></summary>

```php
function _list(string $type = 'ul', $list = [], $attributes = '', int $depth = 0): string
{
	// Set the indentation based on the depth
	$out = str_repeat(' ', $depth)
			// Write the opening list tag
			. '<' . $type . stringify_attributes($attributes) . ">\n";

	// Cycle through the list elements.  If an array is
	// encountered we will recursively call _list()

	static $_last_list_item = '';
	foreach ($list as $key => $val)
	{
		$_last_list_item = $key;

		$out .= str_repeat(' ', $depth + 2) . '<li>';

		if (! is_array($val))
		{
			$out .= $val;
		}
		else
		{
			$out .= $_last_list_item
					. "\n"
					. _list($type, $val, '', $depth + 4)
					. str_repeat(' ', $depth + 2);
		}

		$out .= "</li>\n";
	}

	// Set the indentation for the closing tag and apply it
	return $out . str_repeat(' ', $depth) . '</' . $type . ">\n";
}
```

</details>


<hr>

## img()

```php
function img($src = '', bool $indexPage = false, $attributes = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Image
</td></tr>
</table>

<table>
<tr><td>
Generates an image element
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
<td><code>$src</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$indexPage</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>mixed
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
<summary><small>Source: 42 lines (154 - 195)</small></summary>

```php
function img($src = '', bool $indexPage = false, $attributes = ''): string
{
	if (! is_array($src))
	{
		$src = ['src' => $src];
	}

	if (! isset($src['alt']))
	{
		$src['alt'] = $attributes['alt'] ?? '';
	}

	$img = '<img';

	foreach ($src as $k => $v)
	{
		//Include a protocol if nothing is explicitely defined.
		if ($k === 'src' && ! preg_match('#^([a-z]+:)?//#i', $v))
		{
			if ($indexPage === true)
			{
				$img .= ' src="' . site_url($v) . '"';
			}
			else
			{
				$img .= ' src="' . slash_item('baseURL') . $v . '"';
			}
		}
		else
		{
			$img .= ' ' . $k . '="' . $v . '"';
		}
	}

	// prevent passing "alt" to stringify_attributes
	if (is_array($attributes) && isset($attributes['alt']))
	{
		unset($attributes['alt']);
	}

	return $img . stringify_attributes($attributes) . ' />';
}
```

</details>


<hr>

## doctype()

```php
function doctype(string $type = 'html5') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Doctype
</td></tr>
</table>

<table>
<tr><td>
Generates a page document type declaration

Examples of valid options: html5, xhtml-11, xhtml-strict, xhtml-trans,
xhtml-frame, html4-strict, html4-trans, and html4-frame.
All values are saved in the doctypes config file.
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
<td>The doctype to be generated</td>
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
function doctype(string $type = 'html5'): string
{
	$config   = new \Config\DocTypes();
	$doctypes = $config->list;
	return $doctypes[$type] ?? false;
}
```

</details>


<hr>

## script_tag()

```php
function script_tag($src = '', bool $indexPage = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Script
</td></tr>
</table>

<table>
<tr><td>
Generates link to a JS file
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
<td><code>$src</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Script source or an array</td>
</tr>

<tr>
<td>2.</td>
<td><code>$indexPage</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Should indexPage be added to the JS path</td>
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
<summary><small>Source: 29 lines (237 - 265)</small></summary>

```php
function script_tag($src = '', bool $indexPage = false): string
{
	$script = '<script ';
	if (! is_array($src))
	{
		$src = ['src' => $src];
	}

	foreach ($src as $k => $v)
	{
		if ($k === 'src' && ! preg_match('#^([a-z]+:)?//#i', $v))
		{
			if ($indexPage === true)
			{
				$script .= 'src="' . site_url($v) . '" ';
			}
			else
			{
				$script .= 'src="' . slash_item('baseURL') . $v . '" ';
			}
		}
		else
		{
			$script .= $k . '="' . $v . '" ';
		}
	}

	return $script . 'type="text/javascript"' . '></script>';
}
```

</details>


<hr>

## link_tag()

```php
function link_tag($href = '', string $rel = 'stylesheet', string $type = 'text/css', string $title = '', string $media = '', bool $indexPage = false, string $hreflang = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Link
</td></tr>
</table>

<table>
<tr><td>
Generates link to a CSS file
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
<td><code>$href</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Stylesheet href or an array</td>
</tr>

<tr>
<td>2.</td>
<td><code>$rel</code></td>
<td><em>string
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
<td><code>$title</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$media</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>6.</td>
<td><code>$indexPage</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>should indexPage be added to the CSS path.</td>
</tr>

<tr>
<td>7.</td>
<td><code>$hreflang</code></td>
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
<summary><small>Source: 56 lines (287 - 342)</small></summary>

```php
function link_tag($href = '', string $rel = 'stylesheet', string $type = 'text/css', string $title = '', string $media = '', bool $indexPage = false, string $hreflang = ''): string
{
	$link = '<link ';

	// extract fields if needed
	if (is_array($href))
	{
		$rel       = $href['rel'] ?? $rel;
		$type      = $href['type'] ?? $type;
		$title     = $href['title'] ?? $title;
		$media     = $href['media'] ?? $media;
		$hreflang  = $href['hreflang'] ?? '';
		$indexPage = $href['indexPage'] ?? $indexPage;
		$href      = $href['href'] ?? '';
	}

	if (! preg_match('#^([a-z]+:)?//#i', $href))
	{
		if ($indexPage === true)
		{
			$link .= 'href="' . site_url($href) . '" ';
		}
		else
		{
			$link .= 'href="' . slash_item('baseURL') . $href . '" ';
		}
	}
	else
	{
		$link .= 'href="' . $href . '" ';
	}

	if ($hreflang !== '')
	{
		$link .= 'hreflang="' . $hreflang . '" ';
	}

	$link .= 'rel="' . $rel . '" ';

	if (! in_array($rel, ['alternate', 'canonical']))
	{
		$link .= 'type="' . $type . '" ';
	}

	if ($media !== '')
	{
		$link .= 'media="' . $media . '" ';
	}

	if ($title !== '')
	{
		$link .= 'title="' . $title . '" ';
	}

	return $link . '/>';
}
```

</details>


<hr>

## video()

```php
function video($src, string $unsupportedMessage = '', string $attributes = '', array $tracks = array(), bool $indexPage = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Video
</td></tr>
</table>

<table>
<tr><td>
Generates a video element to embed videos. The video element can
contain one or more video sources
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
<td><code>$src</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Either a source string or an array of sources</td>
</tr>

<tr>
<td>2.</td>
<td><code>$unsupportedMessage</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The message to display if the media tag is not supported by the browser</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>HTML attributes</td>
</tr>

<tr>
<td>4.</td>
<td><code>$tracks</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$indexPage</code></td>
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
<summary><small>Source: 46 lines (363 - 408)</small></summary>

```php
function video($src, string $unsupportedMessage = '', string $attributes = '', array $tracks = [], bool $indexPage = false): string
{
	if (is_array($src))
	{
		return _media('video', $src, $unsupportedMessage, $attributes, $tracks);
	}

	$video = '<video';

	if (_has_protocol($src))
	{
		$video .= ' src="' . $src . '"';
	}
	elseif ($indexPage === true)
	{
		$video .= ' src="' . site_url($src) . '"';
	}
	else
	{
		$video .= ' src="' . slash_item('baseURL') . $src . '"';
	}

	if ($attributes !== '')
	{
		$video .= ' ' . $attributes;
	}

	$video .= ">\n";

	if (! empty($tracks))
	{
		foreach ($tracks as $track)
		{
			$video .= _space_indent() . $track . "\n";
		}
	}

	if (! empty($unsupportedMessage))
	{
		$video .= _space_indent()
				. $unsupportedMessage
				. "\n";
	}

	return $video . "</video>\n";
}
```

</details>


<hr>

## audio()

```php
function audio($src, string $unsupportedMessage = '', string $attributes = '', array $tracks = array(), bool $indexPage = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Audio
</td></tr>
</table>

<table>
<tr><td>
Generates an audio element to embed sounds
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
<td><code>$src</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Either a source string or an array of sources</td>
</tr>

<tr>
<td>2.</td>
<td><code>$unsupportedMessage</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The message to display if the media tag is not supported by the browser.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>HTML attributes</td>
</tr>

<tr>
<td>4.</td>
<td><code>$tracks</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$indexPage</code></td>
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
<summary><small>Source: 44 lines (428 - 471)</small></summary>

```php
function audio($src, string $unsupportedMessage = '', string $attributes = '', array $tracks = [], bool $indexPage = false): string
{
	if (is_array($src))
	{
		return _media('audio', $src, $unsupportedMessage, $attributes, $tracks);
	}

	$audio = '<audio';

	if (_has_protocol($src))
	{
		$audio .= ' src="' . $src . '"';
	}
	elseif ($indexPage === true)
	{
		$audio .= ' src="' . site_url($src) . '"';
	}
	else
	{
		$audio .= ' src="' . slash_item('baseURL') . $src . '"';
	}

	if ($attributes !== '')
	{
		$audio .= ' ' . $attributes;
	}

	$audio .= '>';

	if (! empty($tracks))
	{
		foreach ($tracks as $track)
		{
			$audio .= "\n" . _space_indent() . $track;
		}
	}

	if (! empty($unsupportedMessage))
	{
		$audio .= "\n" . _space_indent() . $unsupportedMessage . "\n";
	}

	return $audio . "</audio>\n";
}
```

</details>


<hr>

## _media()

```php
function _media(string $name, array $types = array(), string $unsupportedMessage = '', string $attributes = '', array $tracks = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generate media based tag
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
<td><code>$types</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$unsupportedMessage</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The message to display if the media tag is not supported by the browser.</td>
</tr>

<tr>
<td>4.</td>
<td><code>$attributes</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$tracks</code></td>
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
<summary><small>Source: 35 lines (489 - 523)</small></summary>

```php
function _media(string $name, array $types = [], string $unsupportedMessage = '', string $attributes = '', array $tracks = []): string
{
	$media = '<' . $name;

	if (empty($attributes))
	{
		$media .= '>';
	}
	else
	{
		$media .= ' ' . $attributes . '>';
	}

	$media .= "\n";

	foreach ($types as $option)
	{
		$media .= _space_indent() . $option . "\n";
	}

	if (! empty($tracks))
	{
		foreach ($tracks as $track)
		{
			$media .= _space_indent() . $track . "\n";
		}
	}

	if (! empty($unsupportedMessage))
	{
		$media .= _space_indent() . $unsupportedMessage . "\n";
	}

	return $media . ('</' . $name . ">\n");
}
```

</details>


<hr>

## source()

```php
function source(string $src, string $type = 'unknown', string $attributes = '', bool $indexPage = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Source
</td></tr>
</table>

<table>
<tr><td>
Generates a source element that specifies multiple media resources
for either audio or video element
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
<td><code>$src</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The path of the media resource</td>
</tr>

<tr>
<td>2.</td>
<td><code>$type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The MIME-type of the resource with optional codecs parameters</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>HTML attributes</td>
</tr>

<tr>
<td>4.</td>
<td><code>$indexPage</code></td>
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
<summary><small>Source: 24 lines (543 - 566)</small></summary>

```php
function source(string $src, string $type = 'unknown', string $attributes = '', bool $indexPage = false): string
{
	if (! _has_protocol($src))
	{
		if ($indexPage === true)
		{
			$src = site_url($src);
		}
		else
		{
			$src = slash_item('baseURL') . $src;
		}
	}

	$source = '<source src="' . $src
			. '" type="' . $type . '"';

	if (! empty($attributes))
	{
		$source .= ' ' . $attributes;
	}

	return $source . ' />';
}
```

</details>


<hr>

## track()

```php
function track(string $src, string $kind, string $srcLanguage, string $label) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Track
</td></tr>
</table>

<table>
<tr><td>
Generates a track element to specify timed tracks. The tracks are
formatted in WebVTT format.
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
<td><code>$src</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The path of the .VTT file</td>
</tr>

<tr>
<td>2.</td>
<td><code>$kind</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$srcLanguage</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$label</code></td>
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
<summary><small>Source: 8 lines (586 - 593)</small></summary>

```php
function track(string $src, string $kind, string $srcLanguage, string $label): string
{
	return '<track src="' . $src
			. '" kind="' . $kind
			. '" srclang="' . $srcLanguage
			. '" label="' . $label
			. '" />';
}
```

</details>


<hr>

## object()

```php
function object(string $data, string $type = 'unknown', string $attributes = '', array $params = array(), bool $indexPage = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Object
</td></tr>
</table>

<table>
<tr><td>
Generates an object element that represents the media
as either image or a resource plugin such as audio, video,
Java applets, ActiveX, PDF and Flash
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
<td><code>$data</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>A resource URL</td>
</tr>

<tr>
<td>2.</td>
<td><code>$type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Content-type of the resource</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>HTML attributes</td>
</tr>

<tr>
<td>4.</td>
<td><code>$params</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$indexPage</code></td>
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
<summary><small>Source: 29 lines (615 - 643)</small></summary>

```php
function object(string $data, string $type = 'unknown', string $attributes = '', array $params = [], bool $indexPage = false): string
{
	if (! _has_protocol($data))
	{
		if ($indexPage === true)
		{
			$data = site_url($data);
		}
		else
		{
			$data = slash_item('baseURL') . $data;
		}
	}

	$object = '<object data="' . $data . '" '
			. $attributes . '>';

	if (! empty($params))
	{
		$object .= "\n";
	}

	foreach ($params as $param)
	{
		$object .= _space_indent() . $param . "\n";
	}

	return $object . "</object>\n";
}
```

</details>


<hr>

## param()

```php
function param(string $name, string $value, string $type = 'ref', string $attributes = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Param
</td></tr>
</table>

<table>
<tr><td>
Generates a param element that defines parameters
for the object element.
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
<td>The name of the parameter</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The value of the parameter</td>
</tr>

<tr>
<td>3.</td>
<td><code>$type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The MIME-type</td>
</tr>

<tr>
<td>4.</td>
<td><code>$attributes</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>HTML attributes</td>
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
<summary><small>Source: 7 lines (663 - 669)</small></summary>

```php
function param(string $name, string $value, string $type = 'ref', string $attributes = ''): string
{
	return '<param name="' . $name
			. '" type="' . $type
			. '" value="' . $value
			. '" ' . $attributes . ' />';
}
```

</details>


<hr>

## embed()

```php
function embed(string $src, string $type = 'unknown', string $attributes = '', bool $indexPage = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Embed
</td></tr>
</table>

<table>
<tr><td>
Generates an embed element
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
<td><code>$src</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The path of the resource to embed</td>
</tr>

<tr>
<td>2.</td>
<td><code>$type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>MIME-type</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>HTML attributes</td>
</tr>

<tr>
<td>4.</td>
<td><code>$indexPage</code></td>
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
<summary><small>Source: 18 lines (688 - 705)</small></summary>

```php
function embed(string $src, string $type = 'unknown', string $attributes = '', bool $indexPage = false): string
{
	if (! _has_protocol($src))
	{
		if ($indexPage === true)
		{
			$src = site_url($src);
		}
		else
		{
			$src = slash_item('baseURL') . $src;
		}
	}

	return '<embed src="' . $src
			. '" type="' . $type . '" '
			. $attributes . " />\n";
}
```

</details>


<hr>

## _has_protocol()

```php
function _has_protocol(string $url)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Test the protocol of a URI.
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
<td><code>$url</code></td>
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
<td>false<br>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (719 - 722)</small></summary>

```php
function _has_protocol(string $url)
{
	return preg_match('#^([a-z]+:)?//#i', $url);
}
```

</details>


<hr>

## _space_indent()

```php
function _space_indent(int $depth = 2) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provide space indenting.
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
<td><code>$depth</code></td>
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
<summary><small>Source: 4 lines (736 - 739)</small></summary>

```php
function _space_indent(int $depth = 2): string
{
	return str_repeat(' ', $depth);
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/html_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/form_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/html_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:04**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>