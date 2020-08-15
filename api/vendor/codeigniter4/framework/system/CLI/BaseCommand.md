


 



<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/BaseCommand.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/FileLocator.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CLI.md">next</a></td>
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
<td>framework/system/CLI/BaseCommand.php
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
<strong>Psr\Log\LoggerInterface</strong>
</td>
<td>LoggerInterface</td>
</tr>
</table>



 
## CodeIgniter\CLI\BaseCommand

<table style="text-align:left">
<tr><th>Abstract</th><td>BaseCommand</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\CLI\BaseCommand</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class BaseCommand
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
<th><a href="#group"><strong>group</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The group the command is lumped under
when listing commands.</td>
</tr>
<tr>
<th><a href="#name"><strong>name</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Command&#039;s name</td>
</tr>
<tr>
<th><a href="#usage"><strong>usage</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>the Command&#039;s usage description</td>
</tr>
<tr>
<th><a href="#description"><strong>description</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>the Command&#039;s short description</td>
</tr>
<tr>
<th><a href="#options"><strong>options</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>the Command&#039;s options description</td>
</tr>
<tr>
<th><a href="#arguments"><strong>arguments</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>the Command&#039;s Arguments description</td>
</tr>
<tr>
<th><a href="#logger"><strong>logger</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Logger to use for a command</td>
</tr>
<tr>
<th><a href="#commands"><strong>commands</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Instance of the CommandRunner controller
so commands can call other commands.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>BaseCommand constructor.</td>
</tr>
<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public<br>abstract

</td>
<td>Actually execute a command.</td>
</tr>
<tr>
<th><a href="#call"><strong>call</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Can be used by a command to run other commands.</td>
</tr>
<tr>
<th><a href="#showError"><strong>showError</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A simple method to display an error with line/file,
in child commands.</td>
</tr>
<tr>
<th><a href="#__get"><strong>__get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Makes it simple to access our protected properties.</td>
</tr>
<tr>
<th><a href="#__isset"><strong>__isset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Makes it simple to check our protected properties.</td>
</tr>
<tr>
<th><a href="#showHelp"><strong>showHelp</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>show Help include (usage,arguments,description,options)</td>
</tr>
<tr>
<th><a href="#getPad"><strong>getPad</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get pad for $key =&gt; $value array output</td>
</tr>

</table>





### Properties


<hr>

#### $group

```php
protected $group;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The group the command is lumped under
when listing commands.
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

#### $name

```php
protected $name;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Command's name
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

#### $usage

```php
protected $usage;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
the Command's usage description
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

#### $description

```php
protected $description;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
the Command's short description
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

#### $options

```php
protected $options = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
the Command's options description
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

#### $arguments

```php
protected $arguments = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
the Command's Arguments description
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
The Logger to use for a command
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Psr\Log\LoggerInterface
</td>
</tr>
</table>


<hr>

#### $commands

```php
protected $commands;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Instance of the CommandRunner controller
so commands can call other commands.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\CLI\Commands
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(LoggerInterface $logger, Commands $commands)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
BaseCommand constructor.
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
<td><em>\Psr\Log\LoggerInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$commands</code></td>
<td><em>\CodeIgniter\CLI\Commands
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 5 lines (122 - 126)</small></summary>

```php
public function __construct(LoggerInterface $logger, Commands $commands)
{
	$this->logger   = $logger;
	$this->commands = $commands;
}
```

</details>


<hr>

#### run()

```php
public abstract function run(array $params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Actually execute a command.
</td></tr>
</table>

<table>
<tr><td>
This has to be over-ridden in any concrete implementation.
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
<td><code>$params</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 136</small></summary>

```php
abstract public function run(array $params);
```

</details>


<hr>

#### call()

```php
protected function call(string $command, array $params = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Can be used by a command to run other commands.
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



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
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
<summary><small>Source: 8 lines (149 - 156)</small></summary>

```php
protected function call(string $command, array $params = [])
{
	// The CommandRunner will grab the first element
	// for the command name.
	array_unshift($params, $command);

	return $this->commands->run($command, $params);
}
```

</details>


<hr>

#### showError()

```php
protected function showError(\Exception $e)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A simple method to display an error with line/file,
in child commands.
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
<td><code>$e</code></td>
<td><em>\Exception
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 7 lines (166 - 172)</small></summary>

```php
protected function showError(\Exception $e)
{
	CLI::newLine();
	CLI::error($e->getMessage());
	CLI::write($e->getFile() . ' - ' . $e->getLine());
	CLI::newLine();
}
```

</details>


<hr>

#### __get()

```php
public function __get(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Makes it simple to access our protected properties.
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (183 - 191)</small></summary>

```php
public function __get(string $key)
{
	if (isset($this->$key))
	{
		return $this->$key;
	}

	return null;
}
```

</details>


<hr>

#### __isset()

```php
public function __isset(string $key) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Makes it simple to check our protected properties.
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (202 - 205)</small></summary>

```php
public function __isset(string $key): bool
{
	return isset($this->$key);
}
```

</details>


<hr>

#### showHelp()

```php
public function showHelp()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
show Help include (usage,arguments,description,options)
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 35 lines (212 - 246)</small></summary>

```php
public function showHelp()
{
	// 4 spaces instead of tab
	$tab = '   ';
	CLI::write(lang('CLI.helpDescription'), 'yellow');
	CLI::write($tab . $this->description);
	CLI::newLine();

	CLI::write(lang('CLI.helpUsage'), 'yellow');
	$usage = empty($this->usage) ? $this->name . ' [arguments]' : $this->usage;
	CLI::write($tab . $usage);
	CLI::newLine();

	$pad = max($this->getPad($this->options, 6), $this->getPad($this->arguments, 6));

	if (! empty($this->arguments))
	{
		CLI::write(lang('CLI.helpArguments'), 'yellow');
		foreach ($this->arguments as $argument => $description)
		{
			CLI::write($tab . CLI::color(str_pad($argument, $pad), 'green') . $description, 'yellow');
		}
		CLI::newLine();
	}

	if (! empty($this->options))
	{
		CLI::write(lang('CLI.helpOptions'), 'yellow');
		foreach ($this->options as $option => $description)
		{
			CLI::write($tab . CLI::color(str_pad($option, $pad), 'green') . $description, 'yellow');
		}
		CLI::newLine();
	}
}
```

</details>


<hr>

#### getPad()

```php
public function getPad(array $array, int $pad) : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get pad for $key => $value array output
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
<td><code>$array</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$pad</code></td>
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
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (258 - 266)</small></summary>

```php
public function getPad(array $array, int $pad): int
{
	$max = 0;
	foreach ($array as $key => $value)
	{
		$max = max($max, strlen($key));
	}
	return $max + $pad;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/BaseCommand.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Autoloader/FileLocator.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CLI.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>