


 



<table>
<tr>
<td style="width:100%"><em>framework/system/View/Parser.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Filters.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Plugins.md">next</a></td>
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
<td>framework/system/View/Parser.php
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
<a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Exceptions/ViewException.md"><strong>CodeIgniter\View\Exceptions\ViewException</strong></a>
</td>
<td>ViewException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerInterface.md"><strong>Psr\Log\LoggerInterface</strong></a>
</td>
<td>LoggerInterface</td>
</tr>
</table>



 
## CodeIgniter\View\Parser

<table style="text-align:left">
<tr><th>Class</th><td>Parser</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\View\Parser</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/View.md">CodeIgniter\View\View</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Parser
</td></tr>
</table>

<table>
<tr><td>
ClassFormerlyKnownAsTemplateParser
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\View
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
<th><a href="#leftDelimiter"><strong>leftDelimiter</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Left delimiter character for pseudo vars</td>
</tr>
<tr>
<th><a href="#rightDelimiter"><strong>rightDelimiter</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Right delimiter character for pseudo vars</td>
</tr>
<tr>
<th><a href="#noparseBlocks"><strong>noparseBlocks</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores extracted noparse blocks.</td>
</tr>
<tr>
<th><a href="#plugins"><strong>plugins</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores any plugins registered at run-time.</td>
</tr>
<tr>
<th><a href="#dataContexts"><strong>dataContexts</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores the context for each data element
when set by `setData` so the context is respected.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor</td>
</tr>
<tr>
<th><a href="#render"><strong>render</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Parse a template</td>
</tr>
<tr>
<th><a href="#renderString"><strong>renderString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Parse a String</td>
</tr>
<tr>
<th><a href="#setData"><strong>setData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets several pieces of view data at once.</td>
</tr>
<tr>
<th><a href="#parse"><strong>parse</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Parse a template</td>
</tr>
<tr>
<th><a href="#parseSingle"><strong>parseSingle</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Parse a single key/value, extracting it</td>
</tr>
<tr>
<th><a href="#parsePair"><strong>parsePair</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Parse a tag pair</td>
</tr>
<tr>
<th><a href="#parseComments"><strong>parseComments</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Removes any comments from the file. Comments are wrapped in {# #} symbols:</td>
</tr>
<tr>
<th><a href="#extractNoparse"><strong>extractNoparse</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Extracts noparse blocks, inserting a hash in its place so that
those blocks of the page are not touched by parsing.</td>
</tr>
<tr>
<th><a href="#insertNoparse"><strong>insertNoparse</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Re-inserts the noparsed contents back into the template.</td>
</tr>
<tr>
<th><a href="#parseConditionals"><strong>parseConditionals</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Parses any conditionals in the code, removing blocks that don&#039;t
pass so we don&#039;t try to parse it later.</td>
</tr>
<tr>
<th><a href="#setDelimiters"><strong>setDelimiters</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Over-ride the substitution field delimiters.</td>
</tr>
<tr>
<th><a href="#replaceSingle"><strong>replaceSingle</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Handles replacing a pseudo-variable with the actual content. Will double-check
for escaping brackets.</td>
</tr>
<tr>
<th><a href="#prepareReplacement"><strong>prepareReplacement</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Callback used during parse() to apply any filters to the value.</td>
</tr>
<tr>
<th><a href="#shouldAddEscaping"><strong>shouldAddEscaping</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks the placeholder the view provided to see if we need to provide any autoescaping.</td>
</tr>
<tr>
<th><a href="#applyFilters"><strong>applyFilters</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Given a set of filters, will apply each of the filters in turn
to $replace, and return the modified string.</td>
</tr>
<tr>
<th><a href="#parsePlugins"><strong>parsePlugins</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Scans the template for any parser plugins, and attempts to execute them.</td>
</tr>
<tr>
<th><a href="#addPlugin"><strong>addPlugin</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Makes a new plugin available during the parsing of the template.</td>
</tr>
<tr>
<th><a href="#removePlugin"><strong>removePlugin</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Removes a plugin from the available plugins.</td>
</tr>
<tr>
<th><a href="#objectToArray"><strong>objectToArray</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Converts an object to an array, respecting any
toArray() methods on an object.</td>
</tr>

</table>





### Properties


<hr>

#### $leftDelimiter

```php
public $leftDelimiter = '{';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Left delimiter character for pseudo vars
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

#### $rightDelimiter

```php
public $rightDelimiter = '}';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Right delimiter character for pseudo vars
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

#### $noparseBlocks

```php
protected $noparseBlocks = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores extracted noparse blocks.
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

#### $plugins

```php
protected $plugins = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores any plugins registered at run-time.
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

#### $dataContexts

```php
protected $dataContexts = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the context for each data element
when set by `setData` so the context is respected.
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
public function __construct($config, string $viewPath = null, $loader = null, bool $debug = null, LoggerInterface $logger = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor
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
<td><code>$config</code></td>
<td><em>\Config\View
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$viewPath</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$loader</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$debug</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$logger</code></td>
<td><em>\LoggerInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 7 lines (102 - 108)</small></summary>

```php
public function __construct($config, string $viewPath = null, $loader = null, bool $debug = null, LoggerInterface $logger = null)
{
	// Ensure user plugins override core plugins.
	$this->plugins = $config->plugins ?? [];

	parent::__construct($config, $viewPath, $loader, $debug, $logger);
}
```

</details>


<hr>

#### render()

```php
public function render(string $view, array $options = null, bool $saveData = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parse a template
</td></tr>
</table>

<table>
<tr><td>
Parses pseudo-variables contained in the specified template view,
replacing them with any data that has already been set.
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
<td><code>$view</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$saveData</code></td>
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
<summary><small>Source: 57 lines (124 - 180)</small></summary>

```php
public function render(string $view, array $options = null, bool $saveData = null): string
{
	$start = microtime(true);
	if (is_null($saveData))
	{
		$saveData = $this->config->saveData;
	}

	$fileExt = pathinfo($view, PATHINFO_EXTENSION);
	$view    = empty($fileExt) ? $view . '.php' : $view; // allow Views as .html, .tpl, etc (from CI3)

	// Was it cached?
	if (isset($options['cache']))
	{
		$cacheName = $options['cache_name'] ?? str_replace('.php', '', $view);

		if ($output = cache($cacheName))
		{
			$this->logPerformance($start, microtime(true), $view);
			return $output;
		}
	}

	$file = $this->viewPath . $view;

	if (! is_file($file))
	{
		$file = $this->loader->locateFile($view, 'Views');
	}

	// locateFile will return an empty string if the file cannot be found.
	if (empty($file))
	{
		throw ViewException::forInvalidFile($file);
	}

	if (is_null($this->tempData))
	{
		$this->tempData = $this->data;
	}

	$template = file_get_contents($file);
	$output   = $this->parse($template, $this->tempData, $options);
	$this->logPerformance($start, microtime(true), $view);

	if ($saveData)
	{
		$this->data = $this->tempData;
	}
	// Should we cache?
	if (isset($options['cache']))
	{
		cache()->save($cacheName, $output, (int) $options['cache']);
	}
	$this->tempData = null;
	return $output;
}
```

</details>


<hr>

#### renderString()

```php
public function renderString(string $template, array $options = null, bool $saveData = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parse a String
</td></tr>
</table>

<table>
<tr><td>
Parses pseudo-variables contained in the specified string,
replacing them with any data that has already been set.
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
<td><code>$template</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$saveData</code></td>
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
<summary><small>Source: 26 lines (196 - 221)</small></summary>

```php
public function renderString(string $template, array $options = null, bool $saveData = null): string
{
	$start = microtime(true);
	if (is_null($saveData))
	{
		$saveData = $this->config->saveData;
	}

	if (is_null($this->tempData))
	{
		$this->tempData = $this->data;
	}

	$output = $this->parse($template, $this->tempData, $options);

	$this->logPerformance($start, microtime(true), $this->excerpt($template));

	if ($saveData)
	{
		$this->data = $this->tempData;
	}

	$this->tempData = null;

	return $output;
}
```

</details>


<hr>

#### setData()

```php
public function setData(array $data = array(), string $context = null) : RendererInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets several pieces of view data at once.
</td></tr>
</table>

<table>
<tr><td>
In the Parser, we need to store the context here
so that the variable is correctly handled within the
parsing itself, and contexts (including raw) are respected.
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
<td><em>array
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
<td>The context to escape it for: html, css, js, url, raw
If 'raw', no escaping will happen</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\RendererInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 27 lines (237 - 263)</small></summary>

```php
public function setData(array $data = [], string $context = null): RendererInterface
{
	if (! empty($context))
	{
		foreach ($data as $key => &$value)
		{
			if (is_array($value))
			{
				foreach ($value as &$obj)
				{
					$obj = $this->objectToArray($obj);
				}
			}
			else
			{
				$value = $this->objectToArray($value);
			}

			$this->dataContexts[$key] = $context;
		}
	}

	$this->tempData = $this->tempData ?? $this->data;
	$this->tempData = array_merge($this->tempData, $data);

	return $this;
}
```

</details>


<hr>

#### parse()

```php
protected function parse(string $template, array $data = array(), array $options = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parse a template
</td></tr>
</table>

<table>
<tr><td>
Parses pseudo-variables contained in the specified template,
replacing them with the data in the second param
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
<td><code>$template</code></td>
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
<td>Future options</td>
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
<summary><small>Source: 45 lines (279 - 323)</small></summary>

```php
protected function parse(string $template, array $data = [], array $options = null): string
{
	if ($template === '')
	{
		return '';
	}

	// Remove any possible PHP tags since we don't support it
	// and parseConditionals needs it clean anyway...
	$template = str_replace(['<?', '?>'], ['&lt;?', '?&gt;'], $template);

	$template = $this->parseComments($template);
	$template = $this->extractNoparse($template);

	// Replace any conditional code here so we don't have to parse as much
	$template = $this->parseConditionals($template);

	// Handle any plugins before normal data, so that
	// it can potentially modify any template between its tags.
	$template = $this->parsePlugins($template);

	// loop over the data variables, replacing
	// the content as we go.
	foreach ($data as $key => $val)
	{
		$escape = true;

		if (is_array($val))
		{
			$escape  = false;
			$replace = $this->parsePair($key, $val, $template);
		}
		else
		{
			$replace = $this->parseSingle($key, (string) $val);
		}

		foreach ($replace as $pattern => $content)
		{
			$template = $this->replaceSingle($pattern, $content, $template, $escape);
		}
	}

	return $this->insertNoparse($template);
}
```

</details>


<hr>

#### parseSingle()

```php
protected function parseSingle(string $key, string $val) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parse a single key/value, extracting it
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (334 - 339)</small></summary>

```php
protected function parseSingle(string $key, string $val): array
{
	$pattern = '#' . $this->leftDelimiter . '!?\s*' . preg_quote($key) . '\s*\|*\s*([|\w<>=\(\),:.\-\s\+\\\\/]+)*\s*!?' . $this->rightDelimiter . '#ms';

	return [$pattern => $val];
}
```

</details>


<hr>

#### parsePair()

```php
protected function parsePair(string $variable, array $data, string $template) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parse a tag pair
</td></tr>
</table>

<table>
<tr><td>
Parses tag pairs: {some_tag} string... {/some_tag}
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
<td><code>$variable</code></td>
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
<td><code>$template</code></td>
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
<summary><small>Source: 85 lines (353 - 437)</small></summary>

```php
protected function parsePair(string $variable, array $data, string $template): array
{
	// Holds the replacement patterns and contents
	// that will be used within a preg_replace in parse()
	$replace = [];

	// Find all matches of space-flexible versions of {tag}{/tag} so we
	// have something to loop over.
	preg_match_all(
			'#' . $this->leftDelimiter . '\s*' . preg_quote($variable) . '\s*' . $this->rightDelimiter . '(.+?)' .
			$this->leftDelimiter . '\s*' . '/' . preg_quote($variable) . '\s*' . $this->rightDelimiter . '#s', $template, $matches, PREG_SET_ORDER
	);

	/*
	 * Each match looks like:
	 *
	 * $match[0] {tag}...{/tag}
	 * $match[1] Contents inside the tag
	 */
	foreach ($matches as $match)
	{
		// Loop over each piece of $data, replacing
		// it's contents so that we know what to replace in parse()
		$str = '';  // holds the new contents for this tag pair.
		foreach ($data as $row)
		{
			// Objects that have a `toArray()` method should be
			// converted with that method (i.e. Entities)
			if (is_object($row) && method_exists($row, 'toArray'))
			{
				$row = $row->toArray();
			}
			// Otherwise, cast as an array and it will grab public properties.
			else if (is_object($row))
			{
				$row = (array)$row;
			}

			$temp  = [];
			$pairs = [];
			$out   = $match[1];
			foreach ($row as $key => $val)
			{
				// For nested data, send us back through this method...
				if (is_array($val))
				{
					$pair = $this->parsePair($key, $val, $match[1]);

					if (! empty($pair))
					{
						$pairs[array_keys( $pair )[0]] = true;
						$temp                          = array_merge($temp, $pair);
					}

					continue;
				}
				else if (is_object($val))
				{
					$val = 'Class: ' . get_class($val);
				}
				else if (is_resource($val))
				{
					$val = 'Resource';
				}

				$temp['#' . $this->leftDelimiter . '!?\s*' . preg_quote($key) . '\s*\|*\s*([|\w<>=\(\),:.\-\s\+\\\\/]+)*\s*!?' . $this->rightDelimiter . '#s'] = $val;
			}

			// Now replace our placeholders with the new content.
			foreach ($temp as $pattern => $content)
			{
				$out = $this->replaceSingle($pattern, $content, $out, ! isset( $pairs[$pattern] ) );
			}

			$str .= $out;
		}

		//Escape | character from filters as it's handled as OR in regex
		$escaped_match = preg_replace('/(?<!\\\\)\\|/', '\\|', $match[0]);

		$replace['#' . $escaped_match . '#s'] = $str;
	}

	return $replace;
}
```

</details>


<hr>

#### parseComments()

```php
protected function parseComments(string $template) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes any comments from the file. Comments are wrapped in {# #} symbols:
</td></tr>
</table>

<table>
<tr><td>
{# This is a comment #}
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
<td><code>$template</code></td>
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
<summary><small>Source: 4 lines (450 - 453)</small></summary>

```php
protected function parseComments(string $template): string
{
	return preg_replace('/\{#.*?#\}/s', '', $template);
}
```

</details>


<hr>

#### extractNoparse()

```php
protected function extractNoparse(string $template) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Extracts noparse blocks, inserting a hash in its place so that
those blocks of the page are not touched by parsing.
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
<td><code>$template</code></td>
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
<summary><small>Source: 21 lines (465 - 485)</small></summary>

```php
protected function extractNoparse(string $template): string
{
	$pattern = '/\{\s*noparse\s*\}(.*?)\{\s*\/noparse\s*\}/ms';

	/*
	 * $matches[][0] is the raw match
	 * $matches[][1] is the contents
	 */
	if (preg_match_all($pattern, $template, $matches, PREG_SET_ORDER))
	{
		foreach ($matches as $match)
		{
			// Create a hash of the contents to insert in its place.
			$hash                       = md5($match[1]);
			$this->noparseBlocks[$hash] = $match[1];
			$template                   = str_replace($match[0], "noparse_{$hash}", $template);
		}
	}

	return $template;
}
```

</details>


<hr>

#### insertNoparse()

```php
public function insertNoparse(string $template) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Re-inserts the noparsed contents back into the template.
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
<td><code>$template</code></td>
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
<summary><small>Source: 10 lines (496 - 505)</small></summary>

```php
public function insertNoparse(string $template): string
{
	foreach ($this->noparseBlocks as $hash => $replace)
	{
		$template = str_replace("noparse_{$hash}", $replace, $template);
		unset($this->noparseBlocks[$hash]);
	}

	return $template;
}
```

</details>


<hr>

#### parseConditionals()

```php
protected function parseConditionals(string $template) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses any conditionals in the code, removing blocks that don't
pass so we don't try to parse it later.
</td></tr>
</table>

<table>
<tr><td>
Valid conditionals:
- if
- elseif
- else
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
<td><code>$template</code></td>
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
<summary><small>Source: 47 lines (522 - 568)</small></summary>

```php
protected function parseConditionals(string $template): string
{
	$pattern = '/\{\s*(if|elseif)\s*((?:\()?(.*?)(?:\))?)\s*\}/ms';

	/**
	 * For each match:
	 * [0] = raw match `{if var}`
	 * [1] = conditional `if`
	 * [2] = condition `do === true`
	 * [3] = same as [2]
	 */
	preg_match_all($pattern, $template, $matches, PREG_SET_ORDER);

	foreach ($matches as $match)
	{
		// Build the string to replace the `if` statement with.
		$condition = $match[2];

		$statement = $match[1] === 'elseif' ? '<?php elseif (' . $condition . '): ?>' : '<?php if (' . $condition . '): ?>';
		$template  = str_replace($match[0], $statement, $template);
	}

	$template = preg_replace('/\{\s*else\s*\}/ms', '<?php else: ?>', $template);
	$template = preg_replace('/\{\s*endif\s*\}/ms', '<?php endif; ?>', $template);

	// Parse the PHP itself, or insert an error so they can debug
	ob_start();

	if (is_null($this->tempData))
	{
		$this->tempData = $this->data;
	}

	extract($this->tempData);

	try
	{
		eval('?>' . $template . '<?php ');
	}
	catch (\ParseError $e)
	{
		ob_end_clean();
		throw ViewException::forTagSyntaxError(str_replace(['?>', '<?php '], '', $template));
	}

	return ob_get_clean();
}
```

</details>


<hr>

#### setDelimiters()

```php
public function setDelimiters($leftDelimiter = '{', $rightDelimiter = '}') : RendererInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Over-ride the substitution field delimiters.
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
<td><code>$leftDelimiter</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$rightDelimiter</code></td>
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
<td>\RendererInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (579 - 584)</small></summary>

```php
public function setDelimiters($leftDelimiter = '{', $rightDelimiter = '}'): RendererInterface
{
	$this->leftDelimiter  = $leftDelimiter;
	$this->rightDelimiter = $rightDelimiter;
	return $this;
}
```

</details>


<hr>

#### replaceSingle()

```php
protected function replaceSingle($pattern, $content, $template, bool $escape = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles replacing a pseudo-variable with the actual content. Will double-check
for escaping brackets.
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
<td><code>$pattern</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$content</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$template</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$escape</code></td>
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
<summary><small>Source: 18 lines (599 - 616)</small></summary>

```php
protected function replaceSingle($pattern, $content, $template, bool $escape = false): string
{
	// Any dollar signs in the pattern will be mis-interpreted, so slash them
	$pattern = addcslashes($pattern, '$');

	// Replace the content in the template
	$template = preg_replace_callback($pattern, function ($matches) use ($content, $escape) {
		// Check for {! !} syntax to not-escape this one.
		if (strpos($matches[0], '{!') === 0 && substr($matches[0], -2) === '!}')
		{
			$escape = false;
		}

		return $this->prepareReplacement($matches, $content, $escape);
	}, $template);

	return $template;
}
```

</details>


<hr>

#### prepareReplacement()

```php
protected function prepareReplacement(array $matches, string $replace, bool $escape = true) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callback used during parse() to apply any filters to the value.
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
<td><code>$matches</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$replace</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$escape</code></td>
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
<summary><small>Source: 18 lines (629 - 646)</small></summary>

```php
protected function prepareReplacement(array $matches, string $replace, bool $escape = true): string
{
	$orig = array_shift($matches);

	// Our regex earlier will leave all chained values on a single line
	// so we need to break them apart so we can apply them all.
	$filters = isset($matches[0]) ? explode('|', $matches[0]) : [];

	if ($escape && ! isset($matches[0]))
	{
		if ($context = $this->shouldAddEscaping($orig))
		{
			$filters[] = "esc({$context})";
		}
	}

	return $this->applyFilters($replace, $filters);
}
```

</details>


<hr>

#### shouldAddEscaping()

```php
public function shouldAddEscaping(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks the placeholder the view provided to see if we need to provide any autoescaping.
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
<summary><small>Source: 33 lines (657 - 689)</small></summary>

```php
public function shouldAddEscaping(string $key)
{
	$escape = false;

	$key = trim(str_replace(['{', '}'], '', $key));

	// If the key has a context stored (from setData)
	// we need to respect that.
	if (array_key_exists($key, $this->dataContexts))
	{
		if ($this->dataContexts[$key] !== 'raw')
		{
			return $this->dataContexts[$key];
		}
	}
	// No pipes, then we know we need to escape
	elseif (strpos($key, '|') === false)
	{
		$escape = 'html';
	}
	// If there's a `noescape` then we're definitely false.
	elseif (strpos($key, 'noescape') !== false)
	{
		$escape = false;
	}
	// If no `esc` filter is found, then we'll need to add one.
	elseif (! preg_match('/\s+esc/', $key))
	{
		$escape = 'html';
	}

	return $escape;
}
```

</details>


<hr>

#### applyFilters()

```php
protected function applyFilters(string $replace, array $filters) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Given a set of filters, will apply each of the filters in turn
to $replace, and return the modified string.
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
<td><code>$replace</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$filters</code></td>
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
<summary><small>Source: 41 lines (702 - 742)</small></summary>

```php
protected function applyFilters(string $replace, array $filters): string
{
	// Determine the requested filters
	foreach ($filters as $filter)
	{
		// Grab any parameter we might need to send
		preg_match('/\([\w<>=\/\\\,:.\-\s\+]+\)/', $filter, $param);

		// Remove the () and spaces to we have just the parameter left
		$param = ! empty($param) ? trim($param[0], '() ') : null;

		// Params can be separated by commas to allow multiple parameters for the filter
		if (! empty($param))
		{
			$param = explode(',', $param);

			// Clean it up
			foreach ($param as &$p)
			{
				$p = trim($p, ' "');
			}
		}
		else
		{
			$param = [];
		}

		// Get our filter name
		$filter = ! empty($param) ? trim(strtolower(substr($filter, 0, strpos($filter, '(')))) : trim($filter);

		if (! array_key_exists($filter, $this->config->filters))
		{
			continue;
		}

		// Filter it....
		$replace = $this->config->filters[$filter]($replace, ...$param);
	}

	return $replace;
}
```

</details>


<hr>

#### parsePlugins()

```php
protected function parsePlugins(string $template)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Scans the template for any parser plugins, and attempts to execute them.
</td></tr>
</table>

<table>
<tr><td>
Plugins are notated based on {+ +} opening and closing braces.

When encountered,
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
<td><code>$template</code></td>
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
<summary><small>Source: 49 lines (758 - 806)</small></summary>

```php
protected function parsePlugins(string $template)
{
	foreach ($this->plugins as $plugin => $callable)
	{
		// Paired tags are enclosed in an array in the config array.
		$isPair   = is_array($callable);
		$callable = $isPair ? array_shift($callable) : $callable;

		$pattern = $isPair ? '#{\+\s*' . $plugin . '([\w\d=-_:\+\s()/\"@.]*)?\s*\+}(.+?){\+\s*/' . $plugin . '\s*\+}#ims' : '#{\+\s*' . $plugin . '([\w\d=-_:\+\s()/\"@.]*)?\s*\+}#ims';

		/**
		 * Match tag pairs
		 *
		 * Each match is an array:
		 *   $matches[0] = entire matched string
		 *   $matches[1] = all parameters string in opening tag
		 *   $matches[2] = content between the tags to send to the plugin.
		 */
		preg_match_all($pattern, $template, $matches, PREG_SET_ORDER);

		if (empty($matches))
		{
			continue;
		}

		foreach ($matches as $match)
		{
			$params = [];

			preg_match_all('/([\w-]+=\"[^"]+\")|([\w-]+=[^\"\s=]+)|(\"[^"]+\")|(\S+)/', trim($match[1]), $matchesParams);
			foreach ($matchesParams[0] as $item)
			{
				$keyVal = explode('=', $item);
				if (count($keyVal) === 2)
				{
					$params[$keyVal[0]] = str_replace('"', '', $keyVal[1]);
				}
				else
				{
					$params[] = str_replace('"', '', $item);
				}
			}

			$template = $isPair ? str_replace($match[0], $callable($match[2], $params), $template) : str_replace($match[0], $callable($params), $template);
		}
	}

	return $template;
}
```

</details>


<hr>

#### addPlugin()

```php
public function addPlugin(string $alias, callable $callback, bool $isPair = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Makes a new plugin available during the parsing of the template.
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
<td><code>$alias</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$callback</code></td>
<td><em>callable
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$isPair</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (818 - 823)</small></summary>

```php
public function addPlugin(string $alias, callable $callback, bool $isPair = false)
{
	$this->plugins[$alias] = $isPair ? [$callback] : $callback;

	return $this;
}
```

</details>


<hr>

#### removePlugin()

```php
public function removePlugin(string $alias)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes a plugin from the available plugins.
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
<td><code>$alias</code></td>
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
<summary><small>Source: 6 lines (834 - 839)</small></summary>

```php
public function removePlugin(string $alias)
{
	unset($this->plugins[$alias]);

	return $this;
}
```

</details>


<hr>

#### objectToArray()

```php
protected function objectToArray($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts an object to an array, respecting any
toArray() methods on an object.
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 16 lines (849 - 864)</small></summary>

```php
protected function objectToArray($value)
{
	// Objects that have a `toArray()` method should be
	// converted with that method (i.e. Entities)
	if (is_object($value) && method_exists($value, 'toArray'))
	{
		$value = $value->toArray();
	}
	// Otherwise, cast as an array and it will grab public properties.
	else if (is_object($value))
	{
		$value = (array)$value;
	}

	return $value;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/View/Parser.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Filters.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Plugins.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>