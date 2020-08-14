


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/url_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/date_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/url_helper.md">next</a></td>
</tr>
</table>




 



# URL Helper


<hr>

## site_url()

```php
function site_url($uri = '', string $protocol = null, \Config\App $altConfig = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return a site URL to use in views
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
<td><code>$uri</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>URI string or array of URI segments</td>
</tr>

<tr>
<td>2.</td>
<td><code>$protocol</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$altConfig</code></td>
<td><em>\Config\App<br>null
</em></td>
<td>false</td>
<td>Alternate configuration to use</td>
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
<summary><small>Source: 33 lines (57 - 89)</small></summary>

```php
function site_url($uri = '', string $protocol = null, \Config\App $altConfig = null): string
{
	// convert segment array to string
	if (is_array($uri))
	{
		$uri = implode('/', $uri);
	}

	// use alternate config if provided, else default one
	$config = $altConfig ?? config(\Config\App::class);

	$fullPath = rtrim(base_url(), '/') . '/';

	// Add index page, if so configured
	if (! empty($config->indexPage))
	{
		$fullPath .= rtrim($config->indexPage, '/');
	}
	if (! empty($uri))
	{
		$fullPath .= '/' . $uri;
	}

	$url = new \CodeIgniter\HTTP\URI($fullPath);

	// allow the scheme to be over-ridden; else, use default
	if (! empty($protocol))
	{
		$url->setScheme($protocol);
	}

	return (string) $url;
}
```

</details>


<hr>

## base_url()

```php
function base_url($uri = '', string $protocol = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the base URL to use in views
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
<td><code>$uri</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>URI string or array of URI segments</td>
</tr>

<tr>
<td>2.</td>
<td><code>$protocol</code></td>
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
<summary><small>Source: 43 lines (103 - 145)</small></summary>

```php
function base_url($uri = '', string $protocol = null): string
{
	// convert segment array to string
	if (is_array($uri))
	{
		$uri = implode('/', $uri);
	}
	$uri = trim($uri, '/');

	// We should be using the configured baseURL that the user set;
	// otherwise get rid of the path, because we have
	// no way of knowing the intent...
	$config = \Config\Services::request()->config;

	// If baseUrl does not have a trailing slash it won't resolve
	// correctly for users hosting in a subfolder.
	$baseUrl = ! empty($config->baseURL) && $config->baseURL !== '/'
		? rtrim($config->baseURL, '/ ') . '/'
		: $config->baseURL;

	$url = new \CodeIgniter\HTTP\URI($baseUrl);
	unset($config);

	// Merge in the path set by the user, if any
	if (! empty($uri))
	{
		$url = $url->resolveRelativeURI($uri);
	}

	// If the scheme wasn't provided, check to
	// see if it was a secure request
	if (empty($protocol) && \Config\Services::request()->isSecure())
	{
		$protocol = 'https';
	}

	if (! empty($protocol))
	{
		$url->setScheme($protocol);
	}

	return rtrim((string) $url, '/ ');
}
```

</details>


<hr>

## current_url()

```php
function current_url(bool $returnObject = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Current URL
</td></tr>
</table>

<table>
<tr><td>
Returns the full URL (including segments) of the page where this
function is placed
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
<td><code>$returnObject</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>True to return an object instead of a strong</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>\CodeIgniter\HTTP\URI
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (162 - 179)</small></summary>

```php
function current_url(bool $returnObject = false)
{
	$uri = clone \Config\Services::request()->uri;

	// If hosted in a sub-folder, we will have additional
	// segments that show up prior to the URI path we just
	// grabbed from the request, so add it on if necessary.
	$baseUri = new \CodeIgniter\HTTP\URI(config(\Config\App::class)->baseURL);

	if (! empty($baseUri->getPath()))
	{
		$uri->setPath(rtrim($baseUri->getPath(), '/ ') . '/' . $uri->getPath());
	}

	// Since we're basing off of the IncomingRequest URI,
	// we are guaranteed to have a host based on our own configs.
	return $returnObject ? $uri : (string) $uri->setQuery('');
}
```

</details>


<hr>

## previous_url()

```php
function previous_url(bool $returnObject = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the previous URL the current visitor was on. For security reasons
we first check in a saved session variable, if it exists, and use that.
</td></tr>
</table>

<table>
<tr><td>
If that's not available, however, we'll use a sanitized url from $_SERVER['HTTP_REFERER']
which can be set by the user so is untrusted and not set by certain browsers/servers.
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
<td><code>$returnObject</code></td>
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
<td>\CodeIgniter\HTTP\URI<br>mixed<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (196 - 206)</small></summary>

```php
function previous_url(bool $returnObject = false)
{
	// Grab from the session first, if we have it,
	// since it's more reliable and safer.
	// Otherwise, grab a sanitized version from $_SERVER.
	$referer = $_SESSION['_ci_previous_url'] ?? \Config\Services::request()->getServer('HTTP_REFERER', FILTER_SANITIZE_URL);

	$referer = $referer ?? site_url('/');

	return $returnObject ? new \CodeIgniter\HTTP\URI($referer) : $referer;
}
```

</details>


<hr>

## uri_string()

```php
function uri_string() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
URL String
</td></tr>
</table>

<table>
<tr><td>
Returns the path part of the current URL
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
<summary><small>Source: 4 lines (220 - 223)</small></summary>

```php
function uri_string(): string
{
	return \Config\Services::request()->uri->getPath();
}
```

</details>


<hr>

## index_page()

```php
function index_page(\Config\App $altConfig = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Index page
</td></tr>
</table>

<table>
<tr><td>
Returns the "index_page" from your config file
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
<td><code>$altConfig</code></td>
<td><em>\Config\App<br>null
</em></td>
<td>false</td>
<td>Alternate configuration to use</td>
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
<summary><small>Source: 7 lines (238 - 244)</small></summary>

```php
function index_page(\Config\App $altConfig = null): string
{
	// use alternate config if provided, else default one
	$config = $altConfig ?? config(\Config\App::class);

	return $config->indexPage;
}
```

</details>


<hr>

## anchor()

```php
function anchor($uri = '', string $title = '', $attributes = '', \Config\App $altConfig = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Anchor Link
</td></tr>
</table>

<table>
<tr><td>
Creates an anchor based on the local URL.
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
<td><code>$uri</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>URI string or array of URI segments</td>
</tr>

<tr>
<td>2.</td>
<td><code>$title</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The link title</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Any attributes</td>
</tr>

<tr>
<td>4.</td>
<td><code>$altConfig</code></td>
<td><em>\Config\App<br>null
</em></td>
<td>false</td>
<td>Alternate configuration to use</td>
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
<summary><small>Source: 21 lines (263 - 283)</small></summary>

```php
function anchor($uri = '', string $title = '', $attributes = '', \Config\App $altConfig = null): string
{
	// use alternate config if provided, else default one
	$config = $altConfig ?? config(\Config\App::class);

	$site_url = is_array($uri) ? site_url($uri, null, $config) : (preg_match('#^(\w+:)?//#i', $uri) ? $uri : site_url($uri, null, $config));
	// eliminate trailing slash
	$site_url = rtrim($site_url, '/');

	if ($title === '')
	{
		$title = $site_url;
	}

	if ($attributes !== '')
	{
		$attributes = stringify_attributes($attributes);
	}

	return '<a href="' . $site_url . '"' . $attributes . '>' . $title . '</a>';
}
```

</details>


<hr>

## anchor_popup()

```php
function anchor_popup($uri = '', string $title = '', $attributes = false, \Config\App $altConfig = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Anchor Link - Pop-up version
</td></tr>
</table>

<table>
<tr><td>
Creates an anchor based on the local URL. The link
opens a new window based on the attributes specified.
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
<td><code>$uri</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the URL</td>
</tr>

<tr>
<td>2.</td>
<td><code>$title</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the link title</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>any attributes</td>
</tr>

<tr>
<td>4.</td>
<td><code>$altConfig</code></td>
<td><em>\Config\App<br>null
</em></td>
<td>false</td>
<td>Alternate configuration to use</td>
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
<summary><small>Source: 47 lines (303 - 349)</small></summary>

```php
function anchor_popup($uri = '', string $title = '', $attributes = false, \Config\App $altConfig = null): string
{
	// use alternate config if provided, else default one
	$config = $altConfig ?? config(\Config\App::class);

	$site_url = preg_match('#^(\w+:)?//#i', $uri) ? $uri : site_url($uri, '', $config);
	$site_url = rtrim($site_url, '/');

	if ($title === '')
	{
		$title = $site_url;
	}

	if ($attributes === false)
	{
		return '<a href="' . $site_url . '" onclick="window.open(\'' . $site_url . "', '_blank'); return false;\">" . $title . '</a>';
	}

	if (! is_array($attributes))
	{
		$attributes = [$attributes];

		// Ref: http://www.w3schools.com/jsref/met_win_open.asp
		$window_name = '_blank';
	}
	elseif (! empty($attributes['window_name']))
	{
		$window_name = $attributes['window_name'];
		unset($attributes['window_name']);
	}
	else
	{
		$window_name = '_blank';
	}

	foreach (['width' => '800', 'height' => '600', 'scrollbars' => 'yes', 'menubar' => 'no', 'status' => 'yes', 'resizable' => 'yes', 'screenx' => '0', 'screeny' => '0'] as $key => $val)
	{
		$atts[$key] = $attributes[$key] ?? $val;
		unset($attributes[$key]);
	}

	$attributes = stringify_attributes($attributes);

	return '<a href="' . $site_url
			. '" onclick="window.open(\'' . $site_url . "', '" . $window_name . "', '" . stringify_attributes($atts, true) . "'); return false;\""
			. $attributes . '>' . $title . '</a>';
}
```

</details>


<hr>

## mailto()

```php
function mailto(string $email, string $title = '', $attributes = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Mailto Link
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
<td><code>$email</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the email address</td>
</tr>

<tr>
<td>2.</td>
<td><code>$title</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the link title</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>any attributes</td>
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
<summary><small>Source: 9 lines (365 - 373)</small></summary>

```php
function mailto(string $email, string $title = '', $attributes = ''): string
{
	if (trim($title) === '')
	{
		$title = $email;
	}

	return '<a href="mailto:' . $email . '"' . stringify_attributes($attributes) . '>' . $title . '</a>';
}
```

</details>


<hr>

## safe_mailto()

```php
function safe_mailto(string $email, string $title = '', $attributes = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Encoded Mailto Link
</td></tr>
</table>

<table>
<tr><td>
Create a spam-protected mailto link written in Javascript
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
<td><code>$email</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the email address</td>
</tr>

<tr>
<td>2.</td>
<td><code>$title</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the link title</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>any attributes</td>
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
<summary><small>Source: 90 lines (391 - 480)</small></summary>

```php
function safe_mailto(string $email, string $title = '', $attributes = ''): string
{
	if (trim($title) === '')
	{
		$title = $email;
	}

	$x = str_split('<a href="mailto:', 1);

	for ($i = 0, $l = strlen($email); $i < $l; $i ++)
	{
		$x[] = '|' . ord($email[$i]);
	}

	$x[] = '"';

	if ($attributes !== '')
	{
		if (is_array($attributes))
		{
			foreach ($attributes as $key => $val)
			{
				$x[] = ' ' . $key . '="';
				for ($i = 0, $l = strlen($val); $i < $l; $i ++)
				{
					$x[] = '|' . ord($val[$i]);
				}
				$x[] = '"';
			}
		}
		else
		{
			for ($i = 0, $l = mb_strlen($attributes); $i < $l; $i ++)
			{
				$x[] = mb_substr($attributes, $i, 1);
			}
		}
	}

	$x[] = '>';

	$temp = [];
	for ($i = 0, $l = strlen($title); $i < $l; $i ++)
	{
		$ordinal = ord($title[$i]);

		if ($ordinal < 128)
		{
			$x[] = '|' . $ordinal;
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
				$x[]    = '|' . $number;
				$count  = 1;
				$temp   = [];
			}
		}
	}

	$x[] = '<';
	$x[] = '/';
	$x[] = 'a';
	$x[] = '>';

	$x = array_reverse($x);

	// improve obfuscation by eliminating newlines & whitespace
	$output = '<script type="text/javascript">'
			. 'var l=new Array();';

	for ($i = 0, $c = count($x); $i < $c; $i ++)
	{
		$output .= 'l[' . $i . "] = '" . $x[$i] . "';";
	}

	return $output . ('for (var i = l.length-1; i >= 0; i=i-1) {'
			. "if (l[i].substring(0, 1) === '|') document.write(\"&#\"+unescape(l[i].substring(1))+\";\");"
			. 'else document.write(unescape(l[i]));'
			. '}'
			. '</script>');
}
```

</details>


<hr>

## auto_link()

```php
function auto_link(string $str, string $type = 'both', bool $popup = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Auto-linker
</td></tr>
</table>

<table>
<tr><td>
Automatically links URL and Email addresses.
Note: There's a bit of extra code here to deal with
URLs or emails that end in a period. We'll strip these
off and add them after the link.
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
<td>the string</td>
</tr>

<tr>
<td>2.</td>
<td><code>$type</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the type: email, url, or both</td>
</tr>

<tr>
<td>3.</td>
<td><code>$popup</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>whether to create pop-up links</td>
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
<summary><small>Source: 37 lines (501 - 537)</small></summary>

```php
function auto_link(string $str, string $type = 'both', bool $popup = false): string
{
	// Find and replace any URLs.
	if ($type !== 'email' && preg_match_all('#(\w*://|www\.)[^\s()<>;]+\w#i', $str, $matches, PREG_OFFSET_CAPTURE | PREG_SET_ORDER))
	{
		// Set our target HTML if using popup links.
		$target = ($popup) ? ' target="_blank"' : '';

		// We process the links in reverse order (last -> first) so that
		// the returned string offsets from preg_match_all() are not
		// moved as we add more HTML.
		foreach (array_reverse($matches) as $match)
		{
			// $match[0] is the matched string/link
			// $match[1] is either a protocol prefix or 'www.'
			//
			// With PREG_OFFSET_CAPTURE, both of the above is an array,
			// where the actual value is held in [0] and its offset at the [1] index.
			$a   = '<a href="' . (strpos($match[1][0], '/') ? '' : 'http://') . $match[0][0] . '"' . $target . '>' . $match[0][0] . '</a>';
			$str = substr_replace($str, $a, $match[0][1], strlen($match[0][0]));
		}
	}

	// Find and replace any emails.
	if ($type !== 'url' && preg_match_all('#([\w\.\-\+]+@[a-z0-9\-]+\.[a-z0-9\-\.]+[^[:punct:]\s])#i', $str, $matches, PREG_OFFSET_CAPTURE))
	{
		foreach (array_reverse($matches[0]) as $match)
		{
			if (filter_var($match[0], FILTER_VALIDATE_EMAIL) !== false)
			{
				$str = substr_replace($str, safe_mailto($match[0]), $match[1], strlen($match[0]));
			}
		}
	}

	return $str;
}
```

</details>


<hr>

## prep_url()

```php
function prep_url(string $str = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prep URL - Simply adds the http:// part if no scheme is included.
</td></tr>
</table>

<table>
<tr><td>
Formerly used URI, but that does not play nicely with URIs missing
the scheme.
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
<td>the URL</td>
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
<summary><small>Source: 16 lines (553 - 568)</small></summary>

```php
function prep_url(string $str = ''): string
{
	if ($str === 'http://' || $str === '')
	{
		return '';
	}

	$url = parse_url($str);

	if (! $url || ! isset($url['scheme']))
	{
		return 'http://' . $str;
	}

	return $str;
}
```

</details>


<hr>

## url_title()

```php
function url_title(string $str, string $separator = '-', bool $lowercase = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create URL Title
</td></tr>
</table>

<table>
<tr><td>
Takes a "title" string as input and creates a
human-friendly URL string with a "separator" string
as the word separator.
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

<tr>
<td>2.</td>
<td><code>$separator</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Word separator (usually '-' or '_')</td>
</tr>

<tr>
<td>3.</td>
<td><code>$lowercase</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to transform the output string to lowercase</td>
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
<summary><small>Source: 24 lines (587 - 610)</small></summary>

```php
function url_title(string $str, string $separator = '-', bool $lowercase = false): string
{
	$q_separator = preg_quote($separator, '#');

	$trans = [
		'&.+?;'                   => '',
		'[^\w\d\pL\pM _-]'              => '',
		'\s+'                     => $separator,
		'(' . $q_separator . ')+' => $separator,
	];

	$str = strip_tags($str);
	foreach ($trans as $key => $val)
	{
		$str = preg_replace('#' . $key . '#iu', $val, $str);
	}

	if ($lowercase === true)
	{
		$str = mb_strtolower($str);
	}

	return trim(trim($str, $separator));
}
```

</details>


<hr>

## mb_url_title()

```php
function mb_url_title(string $str, string $separator = '-', bool $lowercase = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create URL Title that takes into account accented characters
</td></tr>
</table>

<table>
<tr><td>
Takes a "title" string as input and creates a
human-friendly URL string with a "separator" string
as the word separator.
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

<tr>
<td>2.</td>
<td><code>$separator</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Word separator (usually '-' or '_')</td>
</tr>

<tr>
<td>3.</td>
<td><code>$lowercase</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to transform the output string to lowercase</td>
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
<summary><small>Source: 6 lines (629 - 634)</small></summary>

```php
function mb_url_title(string $str, string $separator = '-', bool $lowercase = false): string
{
	helper('text');

	return url_title(convert_accented_characters($str), $separator, $lowercase);
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/url_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/date_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/url_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:07**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>