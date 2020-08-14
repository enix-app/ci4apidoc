


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Commands/Server/Serve.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/ListCommands.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Sessions/CreateMigration.md">next</a></td>
</tr>
</table>







# CodeIgniter\Commands\Server 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Commands\Server</td></tr>
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
<td>framework/system/Commands/Server/Serve.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Server/Serve.md">CodeIgniter\Commands\Server\Serve</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md"><strong>CodeIgniter\CLI\BaseCommand</strong></a>
</td>
<td>BaseCommand</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/CLI/CLI.md"><strong>CodeIgniter\CLI\CLI</strong></a>
</td>
<td>CLI</td>
</tr>
</table>



 
## CodeIgniter\Commands\Server\Serve

<table style="text-align:left">
<tr><th>Class</th><td>Serve</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Commands\Server\Serve</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">CodeIgniter\CLI\BaseCommand</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Launch the PHP development server
</td></tr>
</table>

<table>
<tr><td>
Not testable, as it throws phpunit for a loop :-/
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Commands\Server
</td>
</tr>
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
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
<th><a href="#minPHPVersion"><strong>minPHPVersion</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Minimum PHP version</td>
</tr>
<tr>
<th><a href="#group"><strong>group</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Group</td>
</tr>
<tr>
<th><a href="#name"><strong>name</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Name</td>
</tr>
<tr>
<th><a href="#description"><strong>description</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Description</td>
</tr>
<tr>
<th><a href="#usage"><strong>usage</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Usage</td>
</tr>
<tr>
<th><a href="#arguments"><strong>arguments</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Arguments</td>
</tr>
<tr>
<th><a href="#portOffset"><strong>portOffset</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The current port offset.</td>
</tr>
<tr>
<th><a href="#tries"><strong>tries</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The max number of ports to attempt to serve from</td>
</tr>
<tr>
<th><a href="#options"><strong>options</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Options</td>
</tr>

<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Run the server</td>
</tr>

</table>





### Properties


<hr>

#### $minPHPVersion

```php
protected $minPHPVersion = '7.2';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Minimum PHP version
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

#### $group

```php
protected $group = 'CodeIgniter';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Group
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
protected $name = 'serve';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Name
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
protected $description = 'Launches the CodeIgniter PHP-Development Server.';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Description
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
protected $usage = 'serve';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Usage
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

#### $arguments

```php
protected $arguments = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Arguments
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

#### $portOffset

```php
protected $portOffset = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The current port offset.
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

#### $tries

```php
protected $tries = 10;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The max number of ports to attempt to serve from
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

#### $options

```php
protected $options = [
	'-php'  => 'The PHP Binary [default: "PHP_BINARY"]',
	'-host' => 'The HTTP Host [default: "localhost"]',
	'-port' => 'The HTTP Host Port [default: "8080"]',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Options
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

#### run()

```php
public function run(array $params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Run the server
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
<td>Parameters</td>
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
<summary><small>Source: 38 lines (129 - 166)</small></summary>

```php
public function run(array $params)
{
	// Valid PHP Version?
	if (phpversion() < $this->minPHPVersion)
	{
		// @codeCoverageIgnoreStart
		die('Your PHP version must be ' . $this->minPHPVersion .
			' or higher to run CodeIgniter. Current version: ' . phpversion());
		// @codeCoverageIgnoreEnd
	}

	// Collect any user-supplied options and apply them.
	$php  = escapeshellarg(CLI::getOption('php') ?? PHP_BINARY);
	$host = CLI::getOption('host') ?? 'localhost';
	$port = (int) (CLI::getOption('port') ?? '8080') + $this->portOffset;

	// Get the party started.
	CLI::write('CodeIgniter development server started on http://' . $host . ':' . $port, 'green');
	CLI::write('Press Control-C to stop.');

	// Set the Front Controller path as Document Root.
	$docroot = escapeshellarg(FCPATH);

	// Mimic Apache's mod_rewrite functionality with user settings.
	$rewrite = escapeshellarg(__DIR__ . '/rewrite.php');

	// Call PHP's built-in webserver, making sure to set our
	// base path to the public folder, and to use the rewrite file
	// to ensure our environment is set and it simulates basic mod_rewrite.
	passthru($php . ' -S ' . $host . ':' . $port . ' -t ' . $docroot . ' ' . $rewrite, $status);

	if ($status && $this->portOffset < $this->tries)
	{
		$this->portOffset += 1;

		$this->run($params);
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Commands/Server/Serve.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/ListCommands.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Sessions/CreateMigration.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>