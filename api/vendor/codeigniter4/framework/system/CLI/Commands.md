


 



<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/Commands.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CommandRunner.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Console.md">next</a></td>
</tr>
</table>







# CodeIgniter\CLI 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\CLI</td></tr>
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
<td>framework/system/CLI/Commands.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">CodeIgniter\CLI\BaseCommand</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CLI.md">CodeIgniter\CLI\CLI</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CommandRunner.md">CodeIgniter\CLI\CommandRunner</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Commands.md">CodeIgniter\CLI\Commands</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Console.md">CodeIgniter\CLI\Console</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Exceptions/CLIException.md">CodeIgniter\CLI\Exceptions\CLIException</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Log/Logger.md"><strong>CodeIgniter\Log\Logger</strong></a>
</td>
<td>Logger</td>
</tr>
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
</table>



 
## CodeIgniter\CLI\Commands

<table style="text-align:left">
<tr><th>Class</th><td>Commands</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\CLI\Commands</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Commands
</td></tr>
</table>

<table>
<tr><td>
Core functionality for running, listing, etc commands.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\CLI
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
<th><a href="#commands"><strong>commands</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The found commands.</td>
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
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor</td>
</tr>
<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runs a command given</td>
</tr>
<tr>
<th><a href="#getCommands"><strong>getCommands</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Provide access to the list of commands.</td>
</tr>
<tr>
<th><a href="#discoverCommands"><strong>discoverCommands</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Discovers all commands in the framework and within user code,
and collects instances of them to work with.</td>
</tr>
<tr>
<th><a href="#getCommandAlternatives"><strong>getCommandAlternatives</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Finds alternative of `$name` among collection
of commands.</td>
</tr>

</table>





### Properties


<hr>

#### $commands

```php
protected $commands = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The found commands.
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
<td>\Logger
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct($logger = null)
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
<td><code>$logger</code></td>
<td><em>\CodeIgniter\Log\Logger<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (73 - 76)</small></summary>

```php
public function __construct($logger = null)
{
	$this->logger = $logger ?? service('logger');
}
```

</details>


<hr>

#### run()

```php
public function run(string $command, array $params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs a command given
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

<tr>
<td>2.</td>
<td><code>$params</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 34 lines (84 - 117)</small></summary>

```php
public function run(string $command, array $params)
{
	$this->discoverCommands();

	if (! isset($this->commands[$command]))
	{
		$message = lang('CLI.commandNotFound', [$command]);

		if ($alternatives = $this->getCommandAlternatives($command, $this->commands))
		{
			if (count($alternatives) === 1)
			{
				$message .= "\n\n" . lang('CLI.altCommandSingular') . "\n    ";
			}
			else
			{
				$message .= "\n\n" . lang('CLI.altCommandPlural') . "\n    ";
			}

			$message .= implode("\n    ", $alternatives);
		}

		CLI::error($message);
		CLI::newLine();
		return;
	}

	// The file would have already been loaded during the
	// createCommandList function...
	$className = $this->commands[$command]['class'];
	$class     = new $className($this->logger, $this);

	return $class->run($params);
}
```

</details>


<hr>

#### getCommands()

```php
public function getCommands()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provide access to the list of commands.
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
<summary><small>Source: 6 lines (124 - 129)</small></summary>

```php
public function getCommands()
{
	$this->discoverCommands();

	return $this->commands;
}
```

</details>


<hr>

#### discoverCommands()

```php
public function discoverCommands()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Discovers all commands in the framework and within user code,
and collects instances of them to work with.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 62 lines (135 - 196)</small></summary>

```php
public function discoverCommands()
{
	if (! empty($this->commands))
	{
		return;
	}

	$files = service('locator')->listFiles('Commands/');

	// If no matching command files were found, bail
	if (empty($files))
	{
		// This should never happen in unit testing.
		// if it does, we have far bigger problems!
		// @codeCoverageIgnoreStart
		return;
		// @codeCoverageIgnoreEnd
	}

	// Loop over each file checking to see if a command with that
	// alias exists in the class. If so, return it. Otherwise, try the next.
	foreach ($files as $file)
	{
		$className = Services::locator()->findQualifiedNameFromPath($file);
		if (empty($className) || ! class_exists($className))
		{
			continue;
		}

		try
		{
			$class = new \ReflectionClass($className);

			if (! $class->isInstantiable() || ! $class->isSubclassOf(BaseCommand::class))
			{
				continue;
			}

			$class = new $className($this->logger, $this);

			// Store it!
			if ($class->group !== null)
			{
				$this->commands[$class->name] = [
					'class'       => $className,
					'file'        => $file,
					'group'       => $class->group,
					'description' => $class->description,
				];
			}

			$class = null;
			unset($class);
		}
		catch (\ReflectionException $e)
		{
			$this->logger->error($e->getMessage());
		}
	}

	asort($this->commands);
}
```

</details>


<hr>

#### getCommandAlternatives()

```php
protected function getCommandAlternatives(string $name, array $collection) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Finds alternative of `$name` among collection
of commands.
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
<td><code>$collection</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (207 - 224)</small></summary>

```php
protected function getCommandAlternatives(string $name, array $collection): array
{
	$alternatives = [];

	foreach ($collection as $commandName => $attributes)
	{
		$lev = levenshtein($name, $commandName);

		if ($lev <= strlen($commandName) / 3 || strpos($commandName, $name) !== false)
		{
			$alternatives[$commandName] = $lev;
		}
	}

	ksort($alternatives, SORT_NATURAL | SORT_FLAG_CASE);

	return array_keys($alternatives);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/Commands.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CommandRunner.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Console.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:09**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>