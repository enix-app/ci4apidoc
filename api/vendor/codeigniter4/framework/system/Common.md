


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Common.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/View/View.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Helpers/test_helper.md">next</a></td>
</tr>
</table>




 



# Common


<hr>

## app_timezone()

```php
function app_timezone() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the timezone the application has been set to display
dates in. This might be different than the timezone set
at the server level, as you often want to stores dates in UTC
and convert them on the fly for the user.
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
<summary><small>Source: 6 lines (77 - 82)</small></summary>

```php
function app_timezone(): string
{
	$config = config(App::class);

	return $config->appTimezone;
}
```

</details>


<hr>

## cache()

```php
function cache(string $key = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A convenience method that provides access to the Cache
object. If no parameter is provided, will return the object,
otherwise, will attempt to return the cached value.
</td></tr>
</table>

<table>
<tr><td>
Examples:
cache()->save('foo', 'bar');
$foo = cache('bar');
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
<td><code>$key</code></td>
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
<td>\CodeIgniter\Cache\CacheInterface<br>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 13 lines (100 - 112)</small></summary>

```php
function cache(string $key = null)
{
	$cache = Services::cache();

	// No params - return cache object
	if (is_null($key))
	{
		return $cache;
	}

	// Still here? Retrieve the value.
	return $cache->get($key);
}
```

</details>


<hr>

## clean_path()

```php
function clean_path(string $path) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A convenience method to clean paths for
a nicer looking output. Useful for exception
handling, error logging, etc.
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
<td><code>$path</code></td>
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
<summary><small>Source: 21 lines (126 - 146)</small></summary>

```php
function clean_path(string $path): string
{
	// Resolve relative paths
	$path = realpath($path) ?: $path;

	switch (true)
	{
		case strpos($path, APPPATH) === 0:
			return 'APPPATH' . DIRECTORY_SEPARATOR . substr($path, strlen(APPPATH));
		case strpos($path, SYSTEMPATH) === 0:
			return 'SYSTEMPATH' . DIRECTORY_SEPARATOR . substr($path, strlen(SYSTEMPATH));
		case strpos($path, FCPATH) === 0:
			return 'FCPATH' . DIRECTORY_SEPARATOR . substr($path, strlen(FCPATH));
		case defined('VENDORPATH') && strpos($path, VENDORPATH) === 0:
			return 'VENDORPATH' . DIRECTORY_SEPARATOR . substr($path, strlen(VENDORPATH));
		case strpos($path, ROOTPATH) === 0:
			return 'ROOTPATH' . DIRECTORY_SEPARATOR . substr($path, strlen(ROOTPATH));
		default:
			return $path;
	}
}
```

</details>


<hr>

## command()

```php
function command(string $command)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs a single command.
</td></tr>
</table>

<table>
<tr><td>
Input expected in a single string as would
be used on the command line itself:

 > command('migrate:create SomeMigration');
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
<td><code>$command</code></td>
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
<td>false<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 47 lines (162 - 208)</small></summary>

```php
function command(string $command)
{
	$runner = service('commands');

	$args    = explode(' ', $command);
	$command = array_shift($args);

	$params      = [];
	$optionValue = false;

	foreach ($args as $i => $arg)
	{
		// add to segments if not starting with '-'
		// and not an option value
		if (mb_strpos($arg, '-') !== 0 && ! $optionValue)
		{
			$params[] = $arg;
			continue;
		}

		// if this was an option value, it was already
		// included in the previous iteration, so
		// reset the process
		if (mb_strpos($arg, '-') !== 0)
		{
			$optionValue = false;
			continue;
		}

		$arg   = ltrim($arg, '-');
		$value = null;

		if (isset($args[$i + 1]) && mb_strpos($args[$i + 1], '-') !== 0)
		{
			$value       = $args[$i + 1];
			$optionValue = true;
		}

		$params[$arg] = $value;
	}

	ob_start();
	$runner->run($command, $params);
	$output = ob_get_clean();

	return $output;
}
```

</details>


<hr>

## config()

```php
function config(string $name, bool $getShared = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
More simple way of getting config instances
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
<td><code>$getShared</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (221 - 224)</small></summary>

```php
function config(string $name, bool $getShared = true)
{
	return Config::get($name, $getShared);
}
```

</details>


<hr>

## csrf_token()

```php
function csrf_token() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the CSRF token name.
</td></tr>
</table>

<table>
<tr><td>
Can be used in Views when building hidden inputs manually,
or used in javascript vars when using APIs.
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
<summary><small>Source: 6 lines (236 - 241)</small></summary>

```php
function csrf_token(): string
{
	$config = config(App::class);

	return $config->CSRFTokenName;
}
```

</details>


<hr>

## csrf_header()

```php
function csrf_header() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the CSRF header name.
</td></tr>
</table>

<table>
<tr><td>
Can be used in Views by adding it to the meta tag
or used in javascript to define a header name when using APIs.
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
<summary><small>Source: 6 lines (253 - 258)</small></summary>

```php
function csrf_header(): string
{
	$config = config(App::class);

	return $config->CSRFHeaderName;
}
```

</details>


<hr>

## csrf_hash()

```php
function csrf_hash() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the current hash value for the CSRF protection.
</td></tr>
</table>

<table>
<tr><td>
Can be used in Views when building hidden inputs manually,
or used in javascript vars for API usage.
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
<summary><small>Source: 6 lines (270 - 275)</small></summary>

```php
function csrf_hash(): string
{
	$security = Services::security(null, true);

	return $security->getCSRFHash();
}
```

</details>


<hr>

## csrf_field()

```php
function csrf_field(string $id = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates a hidden input field for use within manually generated forms.
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
<td><code>$id</code></td>
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
<summary><small>Source: 4 lines (287 - 290)</small></summary>

```php
function csrf_field(string $id = null): string
{
	return '<input type="hidden"' . (! empty($id) ? ' id="' . esc($id, 'attr') . '"' : '') . ' name="' . csrf_token() . '" value="' . csrf_hash() . '" />';
}
```

</details>


<hr>

## csrf_meta()

```php
function csrf_meta(string $id = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates a meta tag for use within javascript calls.
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
<td><code>$id</code></td>
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
<summary><small>Source: 4 lines (302 - 305)</small></summary>

```php
function csrf_meta(string $id = null): string
{
	return '<meta' . (! empty($id) ? ' id="' . esc($id, 'attr') . '"' : '') . ' name="' . csrf_header() . '" content="' . csrf_hash() . '" />';
}
```

</details>


<hr>

## db_connect()

```php
function db_connect($db = null, bool $getShared = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Grabs a database connection and returns it to the user.
</td></tr>
</table>

<table>
<tr><td>
This is a convenience wrapper for \Config\Database::connect()
and supports the same parameters. Namely:

When passing in $db, you may pass any of the following to connect:
- group name
- existing connection instance
- array of database configuration values

If $getShared === false then a new connection instance will be provided,
otherwise it will all calls will return the same instance.
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
<td><code>$db</code></td>
<td><em>\CodeIgniter\Database\ConnectionInterface<br>array<br>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$getShared</code></td>
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
<td>\CodeIgniter\Database\BaseConnection
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (329 - 332)</small></summary>

```php
function db_connect($db = null, bool $getShared = true)
{
	return Database::connect($db, $getShared);
}
```

</details>


<hr>

## dd()

```php
function dd(...$vars)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prints a Kint debug report and exits.
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>Can't be tested ... exits
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
<td><code>$vars</code></td>
<td><em>array
</em></td>
<td>true</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 8 lines (344 - 351)</small></summary>

```php
function dd(...$vars)
{
	// @codeCoverageIgnoreStart
	Kint::$aliases[] = 'dd';
	Kint::dump(...$vars);
	exit;
	// @codeCoverageIgnoreEnd
}
```

</details>


<hr>

## env()

```php
function env(string $key, $default = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows user to retrieve values from the environment
variables that have been set. Especially useful for
retrieving values set from the .env file for
use in config files.
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
<td><code>$key</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$default</code></td>
<td><em>null
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
<summary><small>Source: 25 lines (367 - 391)</small></summary>

```php
function env(string $key, $default = null)
{
	$value = $_ENV[$key] ?? $_SERVER[$key] ?? getenv($key);

	// Not found? Return the default value
	if ($value === false)
	{
		return $default;
	}

	// Handle any boolean values
	switch (strtolower($value))
	{
		case 'true':
			return true;
		case 'false':
			return false;
		case 'empty':
			return '';
		case 'null':
			return null;
	}

	return $value;
}
```

</details>


<hr>

## esc()

```php
function esc($data, string $context = 'html', string $encoding = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Performs simple auto-escaping of data for security reasons.
</td></tr>
</table>

<table>
<tr><td>
Might consider making this more complex at a later date.

If $data is a string, then it simply escapes and returns it.
If $data is an array, then it loops over it, escaping each
'value' of the key/value pairs.

Valid context values: html, js, css, url, attr, raw, null
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
<td><em>string<br>array
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

<tr>
<td>3.</td>
<td><code>$encoding</code></td>
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
<td>string<br>array
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\InvalidArgumentException
</td>
</tr>
</table>



<details>
<summary><small>Source: 52 lines (413 - 464)</small></summary>

```php
function esc($data, string $context = 'html', string $encoding = null)
{
	if (is_array($data))
	{
		foreach ($data as &$value)
		{
			$value = esc($value, $context);
		}
	}

	if (is_string($data))
	{
		$context = strtolower($context);

		// Provide a way to NOT escape data since
		// this could be called automatically by
		// the View library.
		if (empty($context) || $context === 'raw')
		{
			return $data;
		}

		if (! in_array($context, ['html', 'js', 'css', 'url', 'attr']))
		{
			throw new InvalidArgumentException('Invalid escape context provided.');
		}

		if ($context === 'attr')
		{
			$method = 'escapeHtmlAttr';
		}
		else
		{
			$method = 'escape' . ucfirst($context);
		}

		static $escaper;
		if (! $escaper)
		{
			$escaper = new Escaper($encoding);
		}

		if ($encoding && $escaper->getEncoding() !== $encoding)
		{
			$escaper = new Escaper($encoding);
		}

		$data = $escaper->$method($data);
	}

	return $data;
}
```

</details>


<hr>

## force_https()

```php
function force_https(int $duration = 31536000, RequestInterface $request = null, ResponseInterface $response = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used to force a page to be accessed in via HTTPS.
</td></tr>
</table>

<table>
<tr><td>
Uses a standard redirect, plus will set the HSTS header
for modern browsers that support, which gives best
protection against man-in-the-middle attacks.
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
<td><code>$duration</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>How long should the SSL header be set for? (in seconds)
Defaults to 1 year.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$request</code></td>
<td><em>\RequestInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$response</code></td>
<td><em>\ResponseInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\HTTP\Exceptions\HTTPException
</td>
</tr>
</table>



<details>
<summary><small>Source: 56 lines (484 - 539)</small></summary>

```php
function force_https(int $duration = 31536000, RequestInterface $request = null, ResponseInterface $response = null)
{
	if (is_null($request))
	{
		$request = Services::request(null, true);
	}
	if (is_null($response))
	{
		$response = Services::response(null, true);
	}

	if ((ENVIRONMENT !== 'testing' && (is_cli() || $request->isSecure())) || (isset($_SERVER['HTTPS']) && $_SERVER['HTTPS'] === 'test'))
	{
		// @codeCoverageIgnoreStart
		return;
		// @codeCoverageIgnoreEnd
	}

	// If the session status is active, we should regenerate
	// the session ID for safety sake.
	if (ENVIRONMENT !== 'testing' && session_status() === PHP_SESSION_ACTIVE)
	{
		// @codeCoverageIgnoreStart
		Services::session(null, true)
			->regenerate();
		// @codeCoverageIgnoreEnd
	}

	$baseURL = config(App::class)->baseURL;

	if (strpos($baseURL, 'https://') === 0)
	{
		$baseURL = (string) substr($baseURL, strlen('https://'));
	}
	elseif (strpos($baseURL, 'http://') === 0)
	{
		$baseURL = (string) substr($baseURL, strlen('http://'));
	}

	$uri = URI::createURIString(
		'https', $baseURL, $request->uri->getPath(), // Absolute URIs should use a "/" for an empty path
		$request->uri->getQuery(), $request->uri->getFragment()
	);

	// Set an HSTS header
	$response->setHeader('Strict-Transport-Security', 'max-age=' . $duration);
	$response->redirect($uri);
	$response->sendHeaders();

	if (ENVIRONMENT !== 'testing')
	{
		// @codeCoverageIgnoreStart
		exit();
		// @codeCoverageIgnoreEnd
	}
}
```

</details>


<hr>

## function_usable()

```php
function function_usable(string $function_name) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Function usable
</td></tr>
</table>

<table>
<tr><td>
Executes a function_exists() check, and if the Suhosin PHP
extension is loaded - checks whether the function that is
checked might be disabled in there as well.

This is useful as function_exists() will return FALSE for
functions disabled via the *disable_functions* php.ini
setting, but not for *suhosin.executor.func.blacklist* and
*suhosin.executor.disable_eval*. These settings will just
terminate script execution if a disabled function is executed.

The above described behavior turned out to be a bug in Suhosin,
but even though a fix was committed for 0.9.34 on 2012-02-12,
that version is yet to be released. This function will therefore
be just temporary, but would probably be kept for a few years.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="http://www.hardened-php.net/suhosin/">http://www.hardened-php.net/suhosin/</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>This is too exotic
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
<td><code>$function_name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Function to check for</td>
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
<summary><small>Source: 16 lines (569 - 584)</small></summary>

```php
function function_usable(string $function_name): bool
{
	static $_suhosin_func_blacklist;

	if (function_exists($function_name))
	{
		if (! isset($_suhosin_func_blacklist))
		{
			$_suhosin_func_blacklist = extension_loaded('suhosin') ? explode(',', trim(ini_get('suhosin.executor.func.blacklist'))) : [];
		}

		return ! in_array($function_name, $_suhosin_func_blacklist, true);
	}

	return false;
}
```

</details>


<hr>

## helper()

```php
function helper($filenames)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Loads a helper file into memory. Supports namespaced helpers,
both in and out of the 'helpers' directory of a namespaced directory.
</td></tr>
</table>

<table>
<tr><td>
Will load ALL helpers of the matching name, in the following order:
1. app/Helpers
2. {namespace}/Helpers
3. system/Helpers
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
<td><code>$filenames</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Files\Exceptions\FileNotFoundException
</td>
</tr>
</table>



<details>
<summary><small>Source: 93 lines (601 - 693)</small></summary>

```php
function helper($filenames)
{
	$loader = Services::locator(true);

	if (! is_array($filenames))
	{
		$filenames = [$filenames];
	}

	// Store a list of all files to include...
	$includes = [];

	foreach ($filenames as $filename)
	{
		// Store our system and application helper
		// versions so that we can control the load ordering.
		$systemHelper  = null;
		$appHelper     = null;
		$localIncludes = [];

		if (strpos($filename, '_helper') === false)
		{
			$filename .= '_helper';
		}

		// If the file is namespaced, we'll just grab that
		// file and not search for any others
		if (strpos($filename, '\\') !== false)
		{
			$path = $loader->locateFile($filename, 'Helpers');

			if (empty($path))
			{
				throw FileNotFoundException::forFileNotFound($filename);
			}

			$includes[] = $path;
		}

		// No namespaces, so search in all available locations
		else
		{
			$paths = $loader->search('Helpers/' . $filename);

			if (! empty($paths))
			{
				foreach ($paths as $path)
				{
					if (strpos($path, APPPATH) === 0)
					{
						// @codeCoverageIgnoreStart
						$appHelper = $path;
						// @codeCoverageIgnoreEnd
					}
					elseif (strpos($path, SYSTEMPATH) === 0)
					{
						$systemHelper = $path;
					}
					else
					{
						$localIncludes[] = $path;
					}
				}
			}

			// App-level helpers should override all others
			if (! empty($appHelper))
			{
				// @codeCoverageIgnoreStart
				$includes[] = $appHelper;
				// @codeCoverageIgnoreEnd
			}

			// All namespaced files get added in next
			$includes = array_merge($includes, $localIncludes);

			// And the system default one should be added in last.
			if (! empty($systemHelper))
			{
				$includes[] = $systemHelper;
			}
		}
	}

	// Now actually include all of the files
	if (! empty($includes))
	{
		foreach ($includes as $path)
		{
			include_once($path);
		}
	}
}
```

</details>


<hr>

## is_cli()

```php
function is_cli() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Is CLI?
</td></tr>
</table>

<table>
<tr><td>
Test to see if a request was made from the command line.
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
<summary><small>Source: 4 lines (705 - 708)</small></summary>

```php
function is_cli(): bool
{
	return (PHP_SAPI === 'cli' || defined('STDIN'));
}
```

</details>


<hr>

## is_really_writable()

```php
function is_really_writable(string $file) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Tests for file writability
</td></tr>
</table>

<table>
<tr><td>
is_writable() returns TRUE on Windows servers when you really can't write to
the file, based on the read-only attribute. is_writable() is also unreliable
on Unix servers if safe_mode is on.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://bugs.php.net/bug.php?id=54709">https://bugs.php.net/bug.php?id=54709</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>Not practical to test, as travis runs on linux
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
<td><code>$file</code></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 34 lines (729 - 762)</small></summary>

```php
function is_really_writable(string $file): bool
{
	// If we're on a Unix server with safe_mode off we call is_writable
	if (DIRECTORY_SEPARATOR === '/' || ! ini_get('safe_mode'))
	{
		return is_writable($file);
	}

	/* For Windows servers and safe_mode "on" installations we'll actually
	 * write a file then read it. Bah...
	 */
	if (is_dir($file))
	{
		$file = rtrim($file, '/') . '/' . bin2hex(random_bytes(16));
		if (($fp = @fopen($file, 'ab')) === false)
		{
			return false;
		}

		fclose($fp);
		@chmod($file, 0777);
		@unlink($file);

		return true;
	}
	elseif (! is_file($file) || ( $fp = @fopen($file, 'ab')) === false)
	{
		return false;
	}

	fclose($fp);

	return true;
}
```

</details>


<hr>

## lang()

```php
function lang(string $line, array $args = array(), string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A convenience method to translate a string or array of them and format
the result with the intl extension's MessageFormatter.
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
<td><code>$line</code></td>
<td><em>string[]
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$args</code></td>
<td><em>array
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (777 - 781)</small></summary>

```php
function lang(string $line, array $args = [], string $locale = null)
{
	return Services::language($locale)
		->getLine($line, $args);
}
```

</details>


<hr>

## log_message()

```php
function log_message(string $level, string $message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A convenience/compatibility method for logging events through
the Log system.
</td></tr>
</table>

<table>
<tr><td>
Allowed log levels are:
- emergency
- alert
- critical
- error
- warning
- notice
- info
- debug
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
<td><code>$level</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$context</code></td>
<td><em>array<br>null
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
<summary><small>Source: 17 lines (806 - 822)</small></summary>

```php
function log_message(string $level, string $message, array $context = [])
{
	// When running tests, we want to always ensure that the
	// TestLogger is running, which provides utilities for
	// for asserting that logs were called in the test code.
	if (ENVIRONMENT === 'testing')
	{
		$logger = new TestLogger(new Logger());

		return $logger->log($level, $message, $context);
	}

	// @codeCoverageIgnoreStart
	return Services::logger(true)
		->log($level, $message, $context);
	// @codeCoverageIgnoreEnd
}
```

</details>


<hr>

## model()

```php
function model(string $name, bool $getShared = true, ConnectionInterface &$conn = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
More simple way of getting model instances
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
<td><code>$getShared</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$conn</code></td>
<td><em>\ConnectionInterface<br>null
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
<summary><small>Source: 4 lines (836 - 839)</small></summary>

```php
function model(string $name, bool $getShared = true, ConnectionInterface &$conn = null)
{
	return \CodeIgniter\Database\ModelFactory::get($name, $getShared, $conn);
}
```

</details>


<hr>

## old()

```php
function old(string $key, $default = null, $escape = 'html')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides access to "old input" that was set in the session
during a redirect()->withInput().
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
<td><code>$key</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$default</code></td>
<td><em>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$escape</code></td>
<td><em>string<br>bool
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 32 lines (854 - 885)</small></summary>

```php
function old(string $key, $default = null, $escape = 'html')
{
	// Ensure the session is loaded
	if (session_status() === PHP_SESSION_NONE && ENVIRONMENT !== 'testing')
	{
		// @codeCoverageIgnoreStart
		session();
		// @codeCoverageIgnoreEnd
	}

	$request = Services::request();

	$value = $request->getOldInput($key);

	// Return the default value if nothing
	// found in the old input.
	if (is_null($value))
	{
		return $default;
	}

	// If the result was serialized array or string, then unserialize it for use...
	if (is_string($value))
	{
		if (strpos($value, 'a:') === 0 || strpos($value, 's:') === 0)
		{
			$value = unserialize($value);
		}
	}

	return $escape === false ? $value : esc($value, $escape);
}
```

</details>


<hr>

## redirect()

```php
function redirect(string $uri = null) : RedirectResponse
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Convenience method that works with the current global $request and
$router instances to redirect using named/reverse-routed routes
to determine the URL to go to. If nothing is found, will treat
as a traditional redirect and pass the string in, letting
$response->redirect() determine the correct method and code.
</td></tr>
</table>

<table>
<tr><td>
If more control is needed, you must use $response->redirect explicitly.
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
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\HTTP\RedirectResponse
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (903 - 913)</small></summary>

```php
function redirect(string $uri = null): RedirectResponse
{
	$response = Services::redirectResponse(null, true);

	if (! empty($uri))
	{
		return $response->route($uri);
	}

	return $response;
}
```

</details>


<hr>

## remove_invisible_characters()

```php
function remove_invisible_characters(string $str, bool $urlEncoded = true) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Remove Invisible Characters
</td></tr>
</table>

<table>
<tr><td>
This prevents sandwiching null characters
between ascii characters, like Java\0script.
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
<td><code>$urlEncoded</code></td>
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
<summary><small>Source: 22 lines (929 - 950)</small></summary>

```php
function remove_invisible_characters(string $str, bool $urlEncoded = true): string
{
	$nonDisplayables = [];

	// every control character except newline (dec 10),
	// carriage return (dec 13) and horizontal tab (dec 09)
	if ($urlEncoded)
	{
		$nonDisplayables[] = '/%0[0-8bcef]/';  // url encoded 00-08, 11, 12, 14, 15
		$nonDisplayables[] = '/%1[0-9a-f]/';   // url encoded 16-31
	}

	$nonDisplayables[] = '/[\x00-\x08\x0B\x0C\x0E-\x1F\x7F]+/S';   // 00-08, 11, 12, 14-31, 127

	do
	{
		$str = preg_replace($nonDisplayables, '', $str, -1, $count);
	}
	while ($count);

	return $str;
}
```

</details>


<hr>

## route_to()

```php
function route_to(string $method, ...$params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Given a controller/method string and any params,
will attempt to build the relative URL to the
matching route.
</td></tr>
</table>

<table>
<tr><td>
NOTE: This requires the controller/method to
have a route defined in the routes Config file.
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
<td><code>$method</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
<td><em>array
</em></td>
<td>true</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>false<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (968 - 971)</small></summary>

```php
function route_to(string $method, ...$params)
{
	return Services::routes()->reverseRoute($method, ...$params);
}
```

</details>


<hr>

## session()

```php
function session(string $val = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A convenience method for accessing the session instance,
or an item that has been set in the session.
</td></tr>
</table>

<table>
<tr><td>
Examples:
session()->set('foo', 'bar');
$foo = session('bar');
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
<td><code>$val</code></td>
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
<td>\CodeIgniter\Session\Session<br>mixed<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 12 lines (988 - 999)</small></summary>

```php
function session(string $val = null)
{
	$session = Services::session();

	// Returning a single item?
	if (is_string($val))
	{
		return $session->get($val);
	}

	return $session;
}
```

</details>


<hr>

## service()

```php
function service(string $name, ...$params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows cleaner access to the Services Config file.
</td></tr>
</table>

<table>
<tr><td>
Always returns a SHARED instance of the class, so
calling the function multiple times should always
return the same instance.

These are equal:
 - $timer = service('timer')
 - $timer = \CodeIgniter\Config\Services::timer();
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
<td><code>$params</code></td>
<td><em>array
</em></td>
<td>true</td>
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
<summary><small>Source: 4 lines (1019 - 1022)</small></summary>

```php
function service(string $name, ...$params)
{
	return Services::$name(...$params);
}
```

</details>


<hr>

## single_service()

```php
function single_service(string $name, ...$params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allow cleaner access to a Service.
</td></tr>
</table>

<table>
<tr><td>
Always returns a new instance of the class.
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
<td><code>$params</code></td>
<td><em>array<br>null
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
<summary><small>Source: 7 lines (1036 - 1042)</small></summary>

```php
function single_service(string $name, ...$params)
{
	// Ensure it's NOT a shared instance
	array_push($params, false);

	return Services::$name(...$params);
}
```

</details>


<hr>

## slash_item()

```php
function slash_item(string $item) : ?string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetch a config file item with slash appended (if not empty)
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
<td><code>$item</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Config item name</td>
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
<summary><small>Source: 12 lines (1057 - 1068)</small></summary>

```php
function slash_item(string $item): ?string
{
	$config     = config(App::class);
	$configItem = $config->{$item};

	if (! isset($configItem) || empty(trim($configItem)))
	{
		return $configItem;
	}

	return rtrim($configItem, '/') . '/';
}
```

</details>


<hr>

## stringify_attributes()

```php
function stringify_attributes($attributes, bool $js = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stringify attributes for use in HTML tags.
</td></tr>
</table>

<table>
<tr><td>
Helper function used to convert a string, array, or object
of attributes to a string.
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
<td><code>$attributes</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>string, array, object</td>
</tr>

<tr>
<td>2.</td>
<td><code>$js</code></td>
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
<summary><small>Source: 23 lines (1084 - 1106)</small></summary>

```php
function stringify_attributes($attributes, bool $js = false): string
{
	$atts = '';

	if (empty($attributes))
	{
		return $atts;
	}

	if (is_string($attributes))
	{
		return ' ' . $attributes;
	}

	$attributes = (array) $attributes;

	foreach ($attributes as $key => $val)
	{
		$atts .= ($js) ? $key . '=' . esc($val, 'js') . ',' : ' ' . $key . '="' . esc($val, 'attr') . '"';
	}

	return rtrim($atts, ',');
}
```

</details>


<hr>

## timer()

```php
function timer(string $name = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A convenience method for working with the timer.
</td></tr>
</table>

<table>
<tr><td>
If no parameter is passed, it will return the timer instance,
otherwise will start or stop the timer intelligently.
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
<td>\CodeIgniter\Debug\Timer<br>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 16 lines (1120 - 1135)</small></summary>

```php
function timer(string $name = null)
{
	$timer = Services::timer();

	if (empty($name))
	{
		return $timer;
	}

	if ($timer->has($name))
	{
		return $timer->stop($name);
	}

	return $timer->start($name);
}
```

</details>


<hr>

## trace()

```php
function trace()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides a backtrace to the current execution point, from Kint.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 5 lines (1143 - 1147)</small></summary>

```php
function trace()
{
	Kint::$aliases[] = 'trace';
	Kint::trace();
}
```

</details>


<hr>

## view()

```php
function view(string $name, array $data = array(), array $options = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Grabs the current RendererInterface-compatible class
and tells it to render the specified view. Simply provides
a convenience method that can be used in Controllers,
libraries, and routed closures.
</td></tr>
</table>

<table>
<tr><td>
NOTE: Does not provide any escaping of the data, so that must
all be handled manually by the developer.
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
<td><code>$data</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Unused - reserved for third-party extensions.</td>
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
<summary><small>Source: 18 lines (1167 - 1184)</small></summary>

```php
function view(string $name, array $data = [], array $options = []): string
{
	/**
	 * @var CodeIgniter\View\View $renderer
	 */
	$renderer = Services::renderer();

	$saveData = config(View::class)->saveData;

	if (array_key_exists('saveData', $options))
	{
		$saveData = (bool) $options['saveData'];
		unset($options['saveData']);
	}

	return $renderer->setData($data, 'raw')
					->render($name, $options, $saveData);
}
```

</details>


<hr>

## view_cell()

```php
function view_cell(string $library, $params = null, int $ttl = 0, string $cacheName = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
View cells are used within views to insert HTML chunks that are managed
by other classes.
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
<td><code>$library</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
<td><em>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$ttl</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$cacheName</code></td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 5 lines (1201 - 1205)</small></summary>

```php
function view_cell(string $library, $params = null, int $ttl = 0, string $cacheName = null): string
{
	return Services::viewcell()
		->render($library, $params, $ttl, $cacheName);
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Common.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/View/View.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Helpers/test_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:26**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>