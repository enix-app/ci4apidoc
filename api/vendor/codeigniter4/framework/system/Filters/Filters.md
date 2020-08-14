


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Filters/Filters.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/FilterInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Honeypot.md">next</a></td>
</tr>
</table>







# CodeIgniter\Filters 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Filters</td></tr>
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
<td>framework/system/Filters/Filters.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/CSRF.md">CodeIgniter\Filters\CSRF</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/DebugToolbar.md">CodeIgniter\Filters\DebugToolbar</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Exceptions/FilterException.md">CodeIgniter\Filters\Exceptions\FilterException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/FilterInterface.md">CodeIgniter\Filters\FilterInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Filters.md">CodeIgniter\Filters\Filters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Honeypot.md">CodeIgniter\Filters\Honeypot</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Exceptions/FilterException.md"><strong>CodeIgniter\Filters\Exceptions\FilterException</strong></a>
</td>
<td>FilterException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md"><strong>CodeIgniter\HTTP\RequestInterface</strong></a>
</td>
<td>RequestInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/ResponseInterface.md"><strong>CodeIgniter\HTTP\ResponseInterface</strong></a>
</td>
<td>ResponseInterface</td>
</tr>
</table>



 
## CodeIgniter\Filters\Filters

<table style="text-align:left">
<tr><th>Class</th><td>Filters</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Filters\Filters</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Filters
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
<th><a href="#filters"><strong>filters</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The processed filters that will
be used to check against.</td>
</tr>
<tr>
<th><a href="#config"><strong>config</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The original config file</td>
</tr>
<tr>
<th><a href="#request"><strong>request</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The active IncomingRequest or CLIRequest</td>
</tr>
<tr>
<th><a href="#response"><strong>response</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The active Response instance</td>
</tr>
<tr>
<th><a href="#initialized"><strong>initialized</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether we&#039;ve done initial processing
on the filter lists.</td>
</tr>
<tr>
<th><a href="#arguments"><strong>arguments</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Any arguments to be passed to filters.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor.</td>
</tr>
<tr>
<th><a href="#setResponse"><strong>setResponse</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set the response explicity.</td>
</tr>
<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runs through all of the filters for the specified
uri and position.</td>
</tr>
<tr>
<th><a href="#initialize"><strong>initialize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runs through our list of filters provided by the configuration
object to get them ready for use, including getting uri masks
to proper regex, removing those we can from the possibilities
based on HTTP method, etc.</td>
</tr>
<tr>
<th><a href="#getFilters"><strong>getFilters</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the processed filters array.</td>
</tr>
<tr>
<th><a href="#addFilter"><strong>addFilter</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Adds a new alias to the config file.</td>
</tr>
<tr>
<th><a href="#enableFilter"><strong>enableFilter</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Ensures that a specific filter is on and enabled for the current request.</td>
</tr>
<tr>
<th><a href="#getArguments"><strong>getArguments</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the arguments for a specified key, or all.</td>
</tr>
<tr>
<th><a href="#processGlobals"><strong>processGlobals</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Add any applicable (not excluded) global filter settings to the mix.</td>
</tr>
<tr>
<th><a href="#processMethods"><strong>processMethods</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Add any method-specific flters to the mix.</td>
</tr>
<tr>
<th><a href="#processFilters"><strong>processFilters</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Add any applicable configured filters to the mix.</td>
</tr>
<tr>
<th><a href="#pathApplies"><strong>pathApplies</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Check paths for match for URI</td>
</tr>

</table>





### Properties


<hr>

#### $filters

```php
protected $filters = [
	'before' => [],
	'after'  => [],
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The processed filters that will
be used to check against.
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

<table>
<tr><td>
The original config file
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Config\Filters
</td>
</tr>
</table>


<hr>

#### $request

```php
protected $request;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The active IncomingRequest or CLIRequest
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\RequestInterface
</td>
</tr>
</table>


<hr>

#### $response

```php
protected $response;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The active Response instance
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\ResponseInterface
</td>
</tr>
</table>


<hr>

#### $initialized

```php
protected $initialized = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether we've done initial processing
on the filter lists.
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

#### $arguments

```php
protected $arguments = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Any arguments to be passed to filters.
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
public function __construct($config, RequestInterface $request, ResponseInterface $response)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor.
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
<td><em>\Config\Filters
</em></td>
<td>false</td>
<td></td>
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








<details>
<summary><small>Source: 6 lines (108 - 113)</small></summary>

```php
public function __construct($config, RequestInterface $request, ResponseInterface $response)
{
	$this->config  = $config;
	$this->request = &$request;
	$this->setResponse($response);
}
```

</details>


<hr>

#### setResponse()

```php
public function setResponse(ResponseInterface $response)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the response explicity.
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
<td><code>$response</code></td>
<td><em>\ResponseInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (120 - 123)</small></summary>

```php
public function setResponse(ResponseInterface $response)
{
	$this->response = &$response;
}
```

</details>


<hr>

#### run()

```php
public function run(string $uri, string $position = 'before')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs through all of the filters for the specified
uri and position.
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

<tr>
<td>2.</td>
<td><code>$position</code></td>
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
<td>\CodeIgniter\HTTP\RequestInterface<br>\CodeIgniter\HTTP\ResponseInterface<br>mixed
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Filters\Exceptions\FilterException
</td>
</tr>
</table>



<details>
<summary><small>Source: 75 lines (137 - 211)</small></summary>

```php
public function run(string $uri, string $position = 'before')
{
	$this->initialize(strtolower($uri));

	foreach ($this->filters[$position] as $alias => $rules)
	{
		if (is_numeric($alias) && is_string($rules))
		{
			$alias = $rules;
		}

		if (! array_key_exists($alias, $this->config->aliases))
		{
			throw FilterException::forNoAlias($alias);
		}

		if (is_array($this->config->aliases[$alias]))
		{
			$classNames = $this->config->aliases[$alias];
		}
		else
		{
			$classNames = [$this->config->aliases[$alias]];
		}

		foreach ($classNames as $className)
		{
			$class = new $className();

			if (! $class instanceof FilterInterface)
			{
				throw FilterException::forIncorrectInterface(get_class($class));
			}

			if ($position === 'before')
			{
				$result = $class->before($this->request, $this->arguments[$alias] ?? null);

				if ($result instanceof RequestInterface)
				{
					$this->request = $result;
					continue;
				}

				// If the response object was sent back,
				// then send it and quit.
				if ($result instanceof ResponseInterface)
				{
					// short circuit - bypass any other filters
					return $result;
				}

				// Ignore an empty result
				if (empty($result))
				{
					continue;
				}

				return $result;
			}
			elseif ($position === 'after')
			{
				$result = $class->after($this->request, $this->response, $this->arguments[$alias] ?? null);

				if ($result instanceof ResponseInterface)
				{
					$this->response = $result;
					continue;
				}
			}
		}
	}

	return $position === 'before' ? $this->request : $this->response;
}
```

</details>


<hr>

#### initialize()

```php
public function initialize(string $uri = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs through our list of filters provided by the configuration
object to get them ready for use, including getting uri masks
to proper regex, removing those we can from the possibilities
based on HTTP method, etc.
</td></tr>
</table>

<table>
<tr><td>
The resulting $this->filters is an array of only filters
that should be applied to this request.

We go ahead an process the entire tree because we'll need to
run through both a before and after and don't want to double
process the rows.
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
<td>\Filters
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (232 - 246)</small></summary>

```php
public function initialize(string $uri = null)
{
	if ($this->initialized === true)
	{
		return $this;
	}

	$this->processGlobals($uri);
	$this->processMethods();
	$this->processFilters($uri);

	$this->initialized = true;

	return $this;
}
```

</details>


<hr>

#### getFilters()

```php
public function getFilters() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the processed filters array.
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
<summary><small>Source: 4 lines (255 - 258)</small></summary>

```php
public function getFilters(): array
{
	return $this->filters;
}
```

</details>


<hr>

#### addFilter()

```php
public function addFilter(string $class, string $alias = null, string $when = 'before', string $section = 'globals')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Adds a new alias to the config file.
</td></tr>
</table>

<table>
<tr><td>
MUST be called prior to initialize();
Intended for use within routes files.
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
<td><code>$class</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$alias</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$when</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$section</code></td>
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
<summary><small>Source: 20 lines (272 - 291)</small></summary>

```php
public function addFilter(string $class, string $alias = null, string $when = 'before', string $section = 'globals')
{
	$alias = $alias ?? md5($class);

	if (! isset($this->config->{$section}))
	{
		$this->config->{$section} = [];
	}

	if (! isset($this->config->{$section}[$when]))
	{
		$this->config->{$section}[$when] = [];
	}

	$this->config->aliases[$alias] = $class;

	$this->config->{$section}[$when][] = $alias;

	return $this;
}
```

</details>


<hr>

#### enableFilter()

```php
public function enableFilter(string $name, string $when = 'before')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ensures that a specific filter is on and enabled for the current request.
</td></tr>
</table>

<table>
<tr><td>
Filters can have "arguments". This is done by placing a colon immediately
after the filter name, followed by a comma-separated list of arguments that
are passed to the filter when executed.
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
<td><code>$when</code></td>
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
<td>\CodeIgniter\Filters\Filters
</td>
</tr>
</table>





<details>
<summary><small>Source: 27 lines (307 - 333)</small></summary>

```php
public function enableFilter(string $name, string $when = 'before')
{
	// Get parameters and clean name
	if (strpos($name, ':') !== false)
	{
		list($name, $params) = explode(':', $name);

		$params = explode(',', $params);
		array_walk($params, function (&$item) {
			$item = trim($item);
		});

		$this->arguments[$name] = $params;
	}

	if (! array_key_exists($name, $this->config->aliases))
	{
		throw FilterException::forNoAlias($name);
	}

	if (! isset($this->filters[$when][$name]))
	{
		$this->filters[$when][] = $name;
	}

	return $this;
}
```

</details>


<hr>

#### getArguments()

```php
public function getArguments(string $key = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the arguments for a specified key, or all.
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (344 - 347)</small></summary>

```php
public function getArguments(string $key = null)
{
	return is_null($key) ? $this->arguments : $this->arguments[$key];
}
```

</details>


<hr>

#### processGlobals()

```php
protected function processGlobals(string $uri = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add any applicable (not excluded) global filter settings to the mix.
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 49 lines (361 - 409)</small></summary>

```php
protected function processGlobals(string $uri = null)
{
	if (! isset($this->config->globals) || ! is_array($this->config->globals))
	{
		return;
	}

	$uri = strtolower(trim($uri, '/ '));

	// Add any global filters, unless they are excluded for this URI
	$sets = [
		'before',
		'after',
	];

	foreach ($sets as $set)
	{
		if (isset($this->config->globals[$set]))
		{
			// look at each alias in the group
			foreach ($this->config->globals[$set] as $alias => $rules)
			{
				$keep = true;
				if (is_array($rules))
				{
					// see if it should be excluded
					if (isset($rules['except']))
					{
						// grab the exclusion rules
						$check = $rules['except'];
						if ($this->pathApplies($uri, $check))
						{
							$keep = false;
						}
					}
				}
				else
				{
					$alias = $rules; // simple name of filter to apply
				}

				if ($keep)
				{
					$this->filters[$set][] = $alias;
				}
			}
		}
	}
}
```

</details>


<hr>

#### processMethods()

```php
protected function processMethods()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add any method-specific flters to the mix.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 16 lines (418 - 433)</small></summary>

```php
protected function processMethods()
{
	if (! isset($this->config->methods) || ! is_array($this->config->methods))
	{
		return;
	}

	// Request method won't be set for CLI-based requests
	$method = strtolower($_SERVER['REQUEST_METHOD'] ?? 'cli');

	if (array_key_exists($method, $this->config->methods))
	{
		$this->filters['before'] = array_merge($this->filters['before'], $this->config->methods[$method]);
		return;
	}
}
```

</details>


<hr>

#### processFilters()

```php
protected function processFilters(string $uri = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add any applicable configured filters to the mix.
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 32 lines (444 - 475)</small></summary>

```php
protected function processFilters(string $uri = null)
{
	if (! isset($this->config->filters) || ! $this->config->filters)
	{
		return;
	}

	$uri = strtolower(trim($uri, '/ '));

	// Add any filters that apply to this URI
	foreach ($this->config->filters as $alias => $settings)
	{
		// Look for inclusion rules
		if (isset($settings['before']))
		{
			$path = $settings['before'];
			if ($this->pathApplies($uri, $path))
			{
				$this->filters['before'][] = $alias;
			}
		}

		if (isset($settings['after']))
		{
			$path = $settings['after'];
			if ($this->pathApplies($uri, $path))
			{
				$this->filters['after'][] = $alias;
			}
		}
	}
}
```

</details>


<hr>

#### pathApplies()

```php
private function pathApplies(string $uri, $paths)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Check paths for match for URI
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
<td>URI to test against</td>
</tr>

<tr>
<td>2.</td>
<td><code>$paths</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>The path patterns to test</td>
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
<summary><small>Source: 30 lines (485 - 514)</small></summary>

```php
private function pathApplies(string $uri, $paths)
{
	// empty path matches all
	if (empty($paths))
	{
		return true;
	}

	// make sure the paths are iterable
	if (is_string($paths))
	{
		$paths = [$paths];
	}

	// treat each paths as pseudo-regex
	foreach ($paths as $path)
	{
		// need to escape path separators
		$path = str_replace('/', '\/', trim($path, '/ '));
		// need to make pseudo wildcard real
		$path = strtolower(str_replace('*', '.*', $path));
		// Does this rule apply here?
		if (preg_match('#^' . $path . '$#', $uri, $match) === 1)
		{
			return true;
		}
	}

	return false;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Filters/Filters.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/FilterInterface.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/Honeypot.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>