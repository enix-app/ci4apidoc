


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Config/DotEnv.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Config.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/ForeignCharacters.md">next</a></td>
</tr>
</table>







# CodeIgniter\Config 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Config</td></tr>
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
<td>framework/system/Config/DotEnv.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/AutoloadConfig.md">CodeIgniter\Config\AutoloadConfig</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">CodeIgniter\Config\BaseConfig</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseService.md">CodeIgniter\Config\BaseService</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Config.md">CodeIgniter\Config\Config</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md">CodeIgniter\Config\DotEnv</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/ForeignCharacters.md">CodeIgniter\Config\ForeignCharacters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Services.md">CodeIgniter\Config\Services</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/View.md">CodeIgniter\Config\View</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Config\DotEnv

<table style="text-align:left">
<tr><th>Class</th><td>DotEnv</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Config\DotEnv</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Environment-specific configuration
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
<th><a href="#path"><strong>path</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The directory where the .env file can be located.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Builds the path to our file.</td>
</tr>
<tr>
<th><a href="#load"><strong>load</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>The main entry point, will load the .env file and process it
so that we end up with all settings in the PHP environment vars
(i.e. getenv(), $_ENV, and $_SERVER)</td>
</tr>
<tr>
<th><a href="#parse"><strong>parse</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Parse the .env file into an array of key =&gt; value</td>
</tr>
<tr>
<th><a href="#setVariable"><strong>setVariable</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Sets the variable into the environment. Will parse the string
first to look for {name}={value} pattern, ensure that nested
variables are handled, and strip it of single and double quotes.</td>
</tr>
<tr>
<th><a href="#normaliseVariable"><strong>normaliseVariable</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Parses for assignment, cleans the $name and $value, and ensures
that nested variables are handled.</td>
</tr>
<tr>
<th><a href="#sanitizeValue"><strong>sanitizeValue</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Strips quotes from the environment variable value.</td>
</tr>
<tr>
<th><a href="#resolveNestedVariables"><strong>resolveNestedVariables</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Resolve the nested variables.</td>
</tr>
<tr>
<th><a href="#getVariable"><strong>getVariable</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Search the different places for environment variables and return first value found.</td>
</tr>

</table>





### Properties


<hr>

#### $path

```php
protected $path;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The directory where the .env file can be located.
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







### Methods


<hr>

#### __construct()

```php
public function __construct(string $path, string $file = '.env')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Builds the path to our file.
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

<tr>
<td>2.</td>
<td><code>$file</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (63 - 66)</small></summary>

```php
public function __construct(string $path, string $file = '.env')
{
	$this->path = rtrim($path, DIRECTORY_SEPARATOR) . DIRECTORY_SEPARATOR . $file;
}
```

</details>


<hr>

#### load()

```php
public function load() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The main entry point, will load the .env file and process it
so that we end up with all settings in the PHP environment vars
(i.e. getenv(), $_ENV, and $_SERVER)
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
<summary><small>Source: 6 lines (77 - 82)</small></summary>

```php
public function load(): bool
{
	$vars = $this->parse();

	return ($vars === null ? false : true);
}
```

</details>


<hr>

#### parse()

```php
public function parse() : ?array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parse the .env file into an array of key => value
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 37 lines (91 - 127)</small></summary>

```php
public function parse(): ?array
{
	// We don't want to enforce the presence of a .env file, they should be optional.
	if (! is_file($this->path))
	{
		return null;
	}

	// Ensure the file is readable
	if (! is_readable($this->path))
	{
		throw new \InvalidArgumentException("The .env file is not readable: {$this->path}");
	}

	$vars = [];

	$lines = file($this->path, FILE_IGNORE_NEW_LINES | FILE_SKIP_EMPTY_LINES);

	foreach ($lines as $line)
	{
		// Is it a comment?
		if (strpos(trim($line), '#') === 0)
		{
			continue;
		}

		// If there is an equal sign, then we know we are assigning a variable.
		if (strpos($line, '=') !== false)
		{
			list($name, $value) = $this->normaliseVariable($line);
			$vars[$name]        = $value;
			$this->setVariable($name, $value);
		}
	}

	return $vars;
}
```

</details>


<hr>

#### setVariable()

```php
protected function setVariable(string $name, string $value = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the variable into the environment. Will parse the string
first to look for {name}={value} pattern, ensure that nested
variables are handled, and strip it of single and double quotes.
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
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 17 lines (139 - 155)</small></summary>

```php
protected function setVariable(string $name, string $value = '')
{
	if (! getenv($name, true))
	{
		putenv("$name=$value");
	}

	if (empty($_ENV[$name]))
	{
		$_ENV[$name] = $value;
	}

	if (empty($_SERVER[$name]))
	{
		$_SERVER[$name] = $value;
	}
}
```

</details>


<hr>

#### normaliseVariable()

```php
public function normaliseVariable(string $name, string $value = '') : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses for assignment, cleans the $name and $value, and ensures
that nested variables are handled.
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 24 lines (168 - 191)</small></summary>

```php
public function normaliseVariable(string $name, string $value = ''): array
{
	// Split our compound string into its parts.
	if (strpos($name, '=') !== false)
	{
		list($name, $value) = explode('=', $name, 2);
	}

	$name  = trim($name);
	$value = trim($value);

	// Sanitize the name
	$name = str_replace(['export', '\'', '"'], '', $name);

	// Sanitize the value
	$value = $this->sanitizeValue($value);

	$value = $this->resolveNestedVariables($value);

	return [
		$name,
		$value,
	];
}
```

</details>


<hr>

#### sanitizeValue()

```php
protected function sanitizeValue(string $value) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Strips quotes from the environment variable value.
</td></tr>
</table>

<table>
<tr><td>
This was borrowed from the excellent phpdotenv with very few changes.
<a href="https://github.com/vlucas/phpdotenv">https://github.com/vlucas/phpdotenv</a>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\InvalidArgumentException
</td>
</tr>
</table>



<details>
<summary><small>Source: 45 lines (206 - 250)</small></summary>

```php
protected function sanitizeValue(string $value): string
{
	if (! $value)
	{
		return $value;
	}

	// Does it begin with a quote?
	if (strpbrk($value[0], '"\'') !== false)
	{
		// value starts with a quote
		$quote        = $value[0];
		$regexPattern = sprintf(
				'/^
				%1$s          # match a quote at the start of the value
				(             # capturing sub-pattern used
							  (?:          # we do not need to capture this
							   [^%1$s\\\\] # any character other than a quote or backslash
							   |\\\\\\\\   # or two backslashes together
							   |\\\\%1$s   # or an escaped quote e.g \"
							  )*           # as many characters that match the previous rules
				)             # end of the capturing sub-pattern
				%1$s          # and the closing quote
				.*$           # and discard any string after the closing quote
				/mx', $quote
		);
		$value        = preg_replace($regexPattern, '$1', $value);
		$value        = str_replace("\\$quote", $quote, $value);
		$value        = str_replace('\\\\', '\\', $value);
	}
	else
	{
		$parts = explode(' #', $value, 2);

		$value = trim($parts[0]);

		// Unquoted values cannot contain whitespace
		if (preg_match('/\s+/', $value) > 0)
		{
			throw new \InvalidArgumentException('.env values containing spaces must be surrounded by quotes.');
		}
	}

	return $value;
}
```

</details>


<hr>

#### resolveNestedVariables()

```php
protected function resolveNestedVariables(string $value) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Resolve the nested variables.
</td></tr>
</table>

<table>
<tr><td>
Look for ${varname} patterns in the variable value and replace with an existing
environment variable.

This was borrowed from the excellent phpdotenv with very few changes.
<a href="https://github.com/vlucas/phpdotenv">https://github.com/vlucas/phpdotenv</a>
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
<summary><small>Source: 24 lines (267 - 290)</small></summary>

```php
protected function resolveNestedVariables(string $value): string
{
	if (strpos($value, '$') !== false)
	{
		$loader = $this;

		$value = preg_replace_callback(
			'/\${([a-zA-Z0-9_]+)}/',
			function ($matchedPatterns) use ($loader) {
				$nestedVariable = $loader->getVariable($matchedPatterns[1]);

				if (is_null($nestedVariable))
				{
					return $matchedPatterns[0];
				}

				return $nestedVariable;
			},
			$value
		);
	}

	return $value;
}
```

</details>


<hr>

#### getVariable()

```php
protected function getVariable(string $name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Search the different places for environment variables and return first value found.
</td></tr>
</table>

<table>
<tr><td>
This was borrowed from the excellent phpdotenv with very few changes.
<a href="https://github.com/vlucas/phpdotenv">https://github.com/vlucas/phpdotenv</a>
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
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (304 - 318)</small></summary>

```php
protected function getVariable(string $name)
{
	switch (true)
	{
		case array_key_exists($name, $_ENV):
			return $_ENV[$name];
		case array_key_exists($name, $_SERVER):
			return $_SERVER[$name];
		default:
			$value = getenv($name);

			// switch getenv default to null
			return $value === false ? null : $value;
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Config/DotEnv.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Config.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/ForeignCharacters.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>