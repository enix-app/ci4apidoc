


 



<table>
<tr>
<td style="width:100%"><em>framework/system/View/View.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Table.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Common.md">next</a></td>
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
<td>framework/system/View/View.php
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
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
<tr>
<td>
<strong>Psr\Log\LoggerInterface</strong>
</td>
<td>LoggerInterface</td>
</tr>
</table>



 
## CodeIgniter\View\View

<table style="text-align:left">
<tr><th>Class</th><td>View</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\View\View</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md">CodeIgniter\View\RendererInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class View
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
<th><a href="#data"><strong>data</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Data that is made available to the Views.</td>
</tr>
<tr>
<th><a href="#tempData"><strong>tempData</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Merge savedData and userData</td>
</tr>
<tr>
<th><a href="#viewPath"><strong>viewPath</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The base directory to look in for our Views.</td>
</tr>
<tr>
<th><a href="#renderVars"><strong>renderVars</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The render variables</td>
</tr>
<tr>
<th><a href="#loader"><strong>loader</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Instance of FileLocator for when
we need to attempt to find a view
that&#039;s not in standard place.</td>
</tr>
<tr>
<th><a href="#logger"><strong>logger</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Logger instance.</td>
</tr>
<tr>
<th><a href="#debug"><strong>debug</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Should we store performance info?</td>
</tr>
<tr>
<th><a href="#performanceData"><strong>performanceData</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Cache stats about our performance here,
when CI_DEBUG = true</td>
</tr>
<tr>
<th><a href="#config"><strong>config</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#saveData"><strong>saveData</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether data should be saved between renders.</td>
</tr>
<tr>
<th><a href="#viewsCount"><strong>viewsCount</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Number of loaded views</td>
</tr>
<tr>
<th><a href="#layout"><strong>layout</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the layout being used, if any.</td>
</tr>
<tr>
<th><a href="#sections"><strong>sections</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Holds the sections and their data.</td>
</tr>
<tr>
<th><a href="#currentSection"><strong>currentSection</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The name of the current section being rendered,
if any.</td>
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
<td>Builds the output based upon a file name and any
data that has already been set.</td>
</tr>
<tr>
<th><a href="#renderString"><strong>renderString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Builds the output based upon a string and any
data that has already been set.</td>
</tr>
<tr>
<th><a href="#excerpt"><strong>excerpt</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Extract first bit of a long string and add ellipsis</td>
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
<th><a href="#setVar"><strong>setVar</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets a single piece of view data.</td>
</tr>
<tr>
<th><a href="#resetData"><strong>resetData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Removes all of the view data from the system.</td>
</tr>
<tr>
<th><a href="#getData"><strong>getData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the current data that will be displayed in the view.</td>
</tr>
<tr>
<th><a href="#extend"><strong>extend</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specifies that the current view should extend an existing layout.</td>
</tr>
<tr>
<th><a href="#section"><strong>section</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Starts holds content for a section within the layout.</td>
</tr>
<tr>
<th><a href="#endSection"><strong>endSection</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#renderSection"><strong>renderSection</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Renders a section&#039;s contents.</td>
</tr>
<tr>
<th><a href="#include"><strong>include</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Used within layout views to include additional views.</td>
</tr>
<tr>
<th><a href="#getPerformanceData"><strong>getPerformanceData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the performance data that might have been collected
during the execution. Used primarily in the Debug Toolbar.</td>
</tr>
<tr>
<th><a href="#logPerformance"><strong>logPerformance</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Logs performance data for rendering a view.</td>
</tr>

</table>





### Properties


<hr>

#### $data

```php
protected $data = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Data that is made available to the Views.
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

#### $tempData

```php
protected $tempData = null;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Merge savedData and userData
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>






<hr>

#### $viewPath

```php
protected $viewPath;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The base directory to look in for our Views.
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

#### $renderVars

```php
protected $renderVars = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The render variables
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

#### $loader

```php
protected $loader;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instance of FileLocator for when
we need to attempt to find a view
that's not in standard place.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Autoloader\FileLocator
</td>
</tr>
</table>


<hr>

#### $logger

```php
protected $logger;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Logger instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Log\Logger
</td>
</tr>
</table>


<hr>

#### $debug

```php
protected $debug = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Should we store performance info?
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

#### $performanceData

```php
protected $performanceData = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cache stats about our performance here,
when CI_DEBUG = true
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

#### $config

```php
protected $config;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Config\View
</td>
</tr>
</table>


<hr>

#### $saveData

```php
protected $saveData;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether data should be saved between renders.
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

#### $viewsCount

```php
protected $viewsCount = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Number of loaded views
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $layout

```php
protected $layout;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the layout being used, if any.
</td></tr>
</table>

<table>
<tr><td>
Set by the `extend` method used within views.
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

#### $sections

```php
protected $sections = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Holds the sections and their data.
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

#### $currentSection

```php
protected $currentSection;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The name of the current section being rendered,
if any.
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
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$loader</code></td>
<td><em>\CodeIgniter\Autoloader\FileLocator<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$debug</code></td>
<td><em>bool<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$logger</code></td>
<td><em>\Psr\Log\LoggerInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (164 - 172)</small></summary>

```php
public function __construct($config, string $viewPath = null, $loader = null, bool $debug = null, LoggerInterface $logger = null)
{
	$this->config   = $config;
	$this->viewPath = rtrim($viewPath, '\\/ ') . DIRECTORY_SEPARATOR;
	$this->loader   = $loader ?? Services::locator();
	$this->logger   = $logger ?? Services::logger();
	$this->debug    = $debug ?? CI_DEBUG;
	$this->saveData = $config->saveData ?? null;
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
Builds the output based upon a file name and any
data that has already been set.
</td></tr>
</table>

<table>
<tr><td>
Valid $options:
   - cache 		number of seconds to cache for
- cache_name	Name to use for cache
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
<summary><small>Source: 99 lines (190 - 288)</small></summary>

```php
public function render(string $view, array $options = null, bool $saveData = null): string
{
	$this->renderVars['start'] = microtime(true);

	// Store the results here so even if
	// multiple views are called in a view, it won't
	// clean it unless we mean it to.
	$saveData                    = $saveData ?? $this->saveData;
	$fileExt                     = pathinfo($view, PATHINFO_EXTENSION);
	$realPath                    = empty($fileExt) ? $view . '.php' : $view; // allow Views as .html, .tpl, etc (from CI3)
	$this->renderVars['view']    = $realPath;
	$this->renderVars['options'] = $options;

	// Was it cached?
	if (isset($this->renderVars['options']['cache']))
	{
		$this->renderVars['cacheName'] = $this->renderVars['options']['cache_name'] ?? str_replace('.php', '', $this->renderVars['view']);

		if ($output = cache($this->renderVars['cacheName']))
		{
			$this->logPerformance($this->renderVars['start'], microtime(true), $this->renderVars['view']);
			return $output;
		}
	}

	$this->renderVars['file'] = $this->viewPath . $this->renderVars['view'];

	if (! is_file($this->renderVars['file']))
	{
		$this->renderVars['file'] = $this->loader->locateFile($this->renderVars['view'], 'Views', empty($fileExt) ? 'php' : $fileExt);
	}

	// locateFile will return an empty string if the file cannot be found.
	if (empty($this->renderVars['file']))
	{
		throw ViewException::forInvalidFile($this->renderVars['view']);
	}

	// Make our view data available to the view.
	$this->tempData = $this->tempData ?? $this->data;
	extract($this->tempData);

	if ($saveData)
	{
		$this->data = $this->tempData;
	}

	// Save current vars
	$renderVars = $this->renderVars;

	ob_start();
	include $this->renderVars['file']; // PHP will be processed
	$output = ob_get_contents();
	@ob_end_clean();

	// Get back current vars
	$this->renderVars = $renderVars;

	// When using layouts, the data has already been stored
	// in $this->sections, and no other valid output
	// is allowed in $output so we'll overwrite it.
	if (! is_null($this->layout) && empty($this->currentSection))
	{
		$layoutView   = $this->layout;
		$this->layout = null;
		// Save current vars
		$renderVars = $this->renderVars;
		$output     = $this->render($layoutView, $options, $saveData);
		// Get back current vars
		$this->renderVars = $renderVars;
	}

	$this->logPerformance($this->renderVars['start'], microtime(true), $this->renderVars['view']);

	if ($this->debug && (! isset($options['debug']) || $options['debug'] === true))
	{
		$toolbarCollectors = config(\Config\Toolbar::class)->collectors;

		if (in_array(\CodeIgniter\Debug\Toolbar\Collectors\Views::class, $toolbarCollectors))
		{
			// Clean up our path names to make them a little cleaner
			$this->renderVars['file'] = clean_path($this->renderVars['file']);
			$this->renderVars['file'] = ++$this->viewsCount . ' ' . $this->renderVars['file'];
			$output                   = '<!-- DEBUG-VIEW START ' . $this->renderVars['file'] . ' -->' . PHP_EOL
				. $output . PHP_EOL
				. '<!-- DEBUG-VIEW ENDED ' . $this->renderVars['file'] . ' -->' . PHP_EOL;
		}
	}

	// Should we cache?
	if (isset($this->renderVars['options']['cache']))
	{
		cache()->save($this->renderVars['cacheName'], $output, (int) $this->renderVars['options']['cache']);
	}

	$this->tempData = null;

	return $output;
}
```

</details>


<hr>

#### renderString()

```php
public function renderString(string $view, array $options = null, bool $saveData = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Builds the output based upon a string and any
data that has already been set.
</td></tr>
</table>

<table>
<tr><td>
Cache does not apply, because there is no "key".
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
<td>The view contents</td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Reserved for 3rd-party uses since
it might be needed to pass additional info
to other template engines.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$saveData</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>If true, will save data for use with any other calls,
if false, will clean the data after displaying the view,
   if not specified, use the config setting.</td>
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
<summary><small>Source: 25 lines (307 - 331)</small></summary>

```php
public function renderString(string $view, array $options = null, bool $saveData = null): string
{
	$start          = microtime(true);
	$saveData       = $saveData ?? $this->saveData;
	$this->tempData = $this->tempData ?? $this->data;

	extract($this->tempData);

	if ($saveData)
	{
		$this->data = $this->tempData;
	}

	ob_start();
	$incoming = '?>' . $view;
	eval($incoming);
	$output = ob_get_contents();
	@ob_end_clean();

	$this->logPerformance($start, microtime(true), $this->excerpt($view));

	$this->tempData = null;

	return $output;
}
```

</details>


<hr>

#### excerpt()

```php
public function excerpt(string $string, int $length = 20) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Extract first bit of a long string and add ellipsis
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
<td><code>$string</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$length</code></td>
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
<summary><small>Source: 4 lines (342 - 345)</small></summary>

```php
public function excerpt(string $string, int $length = 20): string
{
	return (strlen($string) > $length) ? substr($string, 0, $length - 3) . '...' : $string;
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
<td>The context to escape it for: html, css, js, url
If null, no escaping will happen</td>
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
<summary><small>Source: 12 lines (358 - 369)</small></summary>

```php
public function setData(array $data = [], string $context = null): RendererInterface
{
	if ($context)
	{
		$data = \esc($data, $context);
	}

	$this->tempData = $this->tempData ?? $this->data;
	$this->tempData = array_merge($this->tempData, $data);

	return $this;
}
```

</details>


<hr>

#### setVar()

```php
public function setVar(string $name, $value = null, string $context = null) : RendererInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets a single piece of view data.
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$context</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The context to escape it for: html, css, js, url
If null, no escaping will happen</td>
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
<summary><small>Source: 12 lines (383 - 394)</small></summary>

```php
public function setVar(string $name, $value = null, string $context = null): RendererInterface
{
	if ($context)
	{
		$value = \esc($value, $context);
	}

	$this->tempData        = $this->tempData ?? $this->data;
	$this->tempData[$name] = $value;

	return $this;
}
```

</details>


<hr>

#### resetData()

```php
public function resetData() : RendererInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes all of the view data from the system.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\RendererInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (403 - 408)</small></summary>

```php
public function resetData(): RendererInterface
{
	$this->data = [];

	return $this;
}
```

</details>


<hr>

#### getData()

```php
public function getData() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the current data that will be displayed in the view.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (417 - 420)</small></summary>

```php
public function getData(): array
{
	return $this->tempData ?? $this->data;
}
```

</details>


<hr>

#### extend()

```php
public function extend(string $layout)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specifies that the current view should extend an existing layout.
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
<td><code>$layout</code></td>
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (431 - 434)</small></summary>

```php
public function extend(string $layout)
{
	$this->layout = $layout;
}
```

</details>


<hr>

#### section()

```php
public function section(string $name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Starts holds content for a section within the layout.
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








<details>
<summary><small>Source: 6 lines (443 - 448)</small></summary>

```php
public function section(string $name)
{
	$this->currentSection = $name;

	ob_start();
}
```

</details>


<hr>

#### endSection()

```php
public function endSection()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>







<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Laminas\Escaper\Exception\RuntimeException
</td>
</tr>
</table>



<details>
<summary><small>Source: 18 lines (457 - 474)</small></summary>

```php
public function endSection()
{
	$contents = ob_get_clean();

	if (empty($this->currentSection))
	{
		throw new \RuntimeException('View themes, no current section.');
	}

	// Ensure an array exists so we can store multiple entries for this.
	if (! array_key_exists($this->currentSection, $this->sections))
	{
		$this->sections[$this->currentSection] = [];
	}
	$this->sections[$this->currentSection][] = $contents;

	$this->currentSection = null;
}
```

</details>


<hr>

#### renderSection()

```php
public function renderSection(string $sectionName)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Renders a section's contents.
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
<td><code>$sectionName</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 15 lines (483 - 497)</small></summary>

```php
public function renderSection(string $sectionName)
{
	if (! isset($this->sections[$sectionName]))
	{
		echo '';

		return;
	}

	foreach ($this->sections[$sectionName] as $key => $contents)
	{
		echo $contents;
		unset($this->sections[$sectionName][$key]);
	}
}
```

</details>


<hr>

#### include()

```php
public function include(string $view, array $options = null, $saveData = true) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used within layout views to include additional views.
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
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$saveData</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (510 - 513)</small></summary>

```php
public function include(string $view, array $options = null, $saveData = true): string
{
	return $this->render($view, $options, $saveData);
}
```

</details>


<hr>

#### getPerformanceData()

```php
public function getPerformanceData() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the performance data that might have been collected
during the execution. Used primarily in the Debug Toolbar.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (523 - 526)</small></summary>

```php
public function getPerformanceData(): array
{
	return $this->performanceData;
}
```

</details>


<hr>

#### logPerformance()

```php
protected function logPerformance(float $start, float $end, string $view)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Logs performance data for rendering a view.
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
<td><code>$start</code></td>
<td><em>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$end</code></td>
<td><em>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$view</code></td>
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (539 - 549)</small></summary>

```php
protected function logPerformance(float $start, float $end, string $view)
{
	if ($this->debug)
	{
		$this->performanceData[] = [
			'start' => $start,
			'end'   => $end,
			'view'  => $view,
		];
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/View/View.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Table.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Common.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:20**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>