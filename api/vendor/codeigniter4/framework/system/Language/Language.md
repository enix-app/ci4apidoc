


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Language/Language.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/ImageHandlerInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Exceptions/LogException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Language 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Language</td></tr>
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
<td>framework/system/Language/Language.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Language/Language.md">CodeIgniter\Language\Language</a></td></tr>
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
</table>



 
## CodeIgniter\Language\Language

<table style="text-align:left">
<tr><th>Class</th><td>Language</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Language\Language</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handle system messages and localization.
</td></tr>
</table>

<table>
<tr><td>
Locale-based, built on top of PHP internationalization.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Language
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
<th><a href="#language"><strong>language</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores the retrieved language lines
from files for faster retrieval on
second use.</td>
</tr>
<tr>
<th><a href="#locale"><strong>locale</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The current language/locale to work with.</td>
</tr>
<tr>
<th><a href="#intlSupport"><strong>intlSupport</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Boolean value whether the intl
libraries exist on the system.</td>
</tr>
<tr>
<th><a href="#loadedFiles"><strong>loadedFiles</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores filenames that have been
loaded so that we don&#039;t load them again.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#setLocale"><strong>setLocale</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the current locale to use when performing string lookups.</td>
</tr>
<tr>
<th><a href="#getLocale"><strong>getLocale</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#getLine"><strong>getLine</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Parses the language string for a file, loads the file, if necessary,
getting the line.</td>
</tr>
<tr>
<th><a href="#getTranslationOutput"><strong>getTranslationOutput</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td></td>
</tr>
<tr>
<th><a href="#parseLine"><strong>parseLine</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Parses the language string which should include the
filename as the first segment (separated by period).</td>
</tr>
<tr>
<th><a href="#formatMessage"><strong>formatMessage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Advanced message formatting.</td>
</tr>
<tr>
<th><a href="#load"><strong>load</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Loads a language file in the current locale. If $return is true,
will return the file&#039;s contents, otherwise will merge with
the existing language lines.</td>
</tr>
<tr>
<th><a href="#requireFile"><strong>requireFile</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A simple method for including files that can be
overridden during testing.</td>
</tr>

</table>





### Properties


<hr>

#### $language

```php
protected $language = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the retrieved language lines
from files for faster retrieval on
second use.
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

#### $locale

```php
protected $locale;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The current language/locale to work with.
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

#### $intlSupport

```php
protected $intlSupport = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Boolean value whether the intl
libraries exist on the system.
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


<hr>

#### $loadedFiles

```php
protected $loadedFiles = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores filenames that have been
loaded so that we don't load them again.
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







### Methods


<hr>

#### __construct()

```php
public function __construct(string $locale)
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
<td><code>$locale</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (87 - 95)</small></summary>

```php
public function __construct(string $locale)
{
	$this->locale = $locale;

	if (class_exists('\MessageFormatter'))
	{
		$this->intlSupport = true;
	};
}
```

</details>


<hr>

#### setLocale()

```php
public function setLocale(string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the current locale to use when performing string lookups.
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (106 - 114)</small></summary>

```php
public function setLocale(string $locale = null)
{
	if (! is_null($locale))
	{
		$this->locale = $locale;
	}

	return $this;
}
```

</details>


<hr>

#### getLocale()

```php
public function getLocale() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<summary><small>Source: 4 lines (121 - 124)</small></summary>

```php
public function getLocale(): string
{
	return $this->locale;
}
```

</details>


<hr>

#### getLine()

```php
public function getLine(string $line, array $args = [])
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses the language string for a file, loads the file, if necessary,
getting the line.
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
<td><em>string
</em></td>
<td>false</td>
<td>Line.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$args</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Arguments.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>string[]
</td>
</tr>
</table>





<details>
<summary><small>Source: 48 lines (137 - 184)</small></summary>

```php
public function getLine(string $line, array $args = [])
{
	// ignore requests with no file specified
	if (! strpos($line, '.'))
	{
		return $line;
	}

	// Parse out the file name and the actual alias.
	// Will load the language file and strings.
	[
		$file,
		$parsedLine,
	] = $this->parseLine($line, $this->locale);

	$output = $this->getTranslationOutput($this->locale, $file, $parsedLine);

	if ($output === null && strpos($this->locale, '-'))
	{
		[$locale] = explode('-', $this->locale, 2);

		[
			$file,
			$parsedLine,
		] = $this->parseLine($line, $locale);

		$output = $this->getTranslationOutput($locale, $file, $parsedLine);
	}

	// if still not found, try English
	if ($output === null)
	{
		[
			$file,
			$parsedLine,
		]       = $this->parseLine($line, 'en');
		$output = $this->getTranslationOutput('en', $file, $parsedLine);
	}

	$output = $output ?? $line;

	if (! empty($args))
	{
		$output = $this->formatMessage($output, $args);
	}

	return $output;
}
```

</details>


<hr>

#### getTranslationOutput()

```php
private function getTranslationOutput(string $locale, string $file, string $parsedLine)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 32 lines (191 - 222)</small></summary>

```php
private function getTranslationOutput(string $locale, string $file, string $parsedLine)
{
	$output = $this->language[$locale][$file][$parsedLine] ?? null;
	if ($output !== null)
	{
		return $output;
	}

	foreach (explode('.', $parsedLine) as $row)
	{
		if (! isset($current))
		{
			$current = $this->language[$locale][$file] ?? null;
		}

		$output = $current[$row] ?? null;
		if (is_array($output))
		{
			$current = $output;
		}
	}

	if ($output !== null)
	{
		return $output;
	}

	$row = current(explode('.', $parsedLine));
	$key = substr($parsedLine, strlen($row) + 1);

	return $this->language[$locale][$file][$row][$key] ?? null;
}
```

</details>


<hr>

#### parseLine()

```php
protected function parseLine(string $line, string $locale) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses the language string which should include the
filename as the first segment (separated by period).
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
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (233 - 247)</small></summary>

```php
protected function parseLine(string $line, string $locale): array
{
	$file = substr($line, 0, strpos($line, '.'));
	$line = substr($line, strlen($file) + 1);

	if (! isset($this->language[$locale][$file]) || ! array_key_exists($line, $this->language[$locale][$file]))
	{
		$this->load($file, $locale);
	}

	return [
		$file,
		$line,
	];
}
```

</details>


<hr>

#### formatMessage()

```php
protected function formatMessage($message, array $args = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Advanced message formatting.
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
<td><code>$message</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Message.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$args</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Arguments.</td>
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





<details>
<summary><small>Source: 18 lines (259 - 276)</small></summary>

```php
protected function formatMessage($message, array $args = [])
{
	if (! $this->intlSupport || ! $args)
	{
		return $message;
	}

	if (is_array($message))
	{
		foreach ($message as $index => $value)
		{
			$message[$index] = $this->formatMessage($value, $args);
		}
		return $message;
	}

	return \MessageFormatter::formatMessage($this->locale, $message, $args);
}
```

</details>


<hr>

#### load()

```php
protected function load(string $file, string $locale, bool $return = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Loads a language file in the current locale. If $return is true,
will return the file's contents, otherwise will merge with
the existing language lines.
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
<td><code>$file</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$locale</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$return</code></td>
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
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 37 lines (291 - 327)</small></summary>

```php
protected function load(string $file, string $locale, bool $return = false)
{
	if (! array_key_exists($locale, $this->loadedFiles))
	{
		$this->loadedFiles[$locale] = [];
	}

	if (in_array($file, $this->loadedFiles[$locale]))
	{
		// Don't load it more than once.
		return [];
	}

	if (! array_key_exists($locale, $this->language))
	{
		$this->language[$locale] = [];
	}

	if (! array_key_exists($file, $this->language[$locale]))
	{
		$this->language[$locale][$file] = [];
	}

	$path = "Language/{$locale}/{$file}.php";

	$lang = $this->requireFile($path);

	if ($return)
	{
		return $lang;
	}

	$this->loadedFiles[$locale][] = $file;

	// Merge our string
	$this->language[$locale][$file] = $lang;
}
```

</details>


<hr>

#### requireFile()

```php
protected function requireFile(string $path) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A simple method for including files that can be
overridden during testing.
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 28 lines (339 - 366)</small></summary>

```php
protected function requireFile(string $path): array
{
	$files   = Services::locator()->search($path, 'php', false);
	$strings = [];

	foreach ($files as $file)
	{
		// On some OS's we were seeing failures
		// on this command returning boolean instead
		// of array during testing, so we've removed
		// the require_once for now.
		if (is_file($file))
		{
			$strings[] = require $file;
		}
	}

	if (isset($strings[1]))
	{
		$strings = array_replace_recursive(...$strings);
	}
	elseif (isset($strings[0]))
	{
		$strings = $strings[0];
	}

	return $strings;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Language/Language.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/ImageHandlerInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Exceptions/LogException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:17**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>