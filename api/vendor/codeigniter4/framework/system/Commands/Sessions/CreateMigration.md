


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Commands/Sessions/CreateMigration.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Server/Serve.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Utilities/Namespaces.md">next</a></td>
</tr>
</table>







# CodeIgniter\Commands\Sessions 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Commands\Sessions</td></tr>
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
<td>framework/system/Commands/Sessions/CreateMigration.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Sessions/CreateMigration.md">CodeIgniter\Commands\Sessions\CreateMigration</a></td></tr>
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
<tr>
<td>
<strong>Config\App</strong>
</td>
<td>App</td>
</tr>
</table>



 
## CodeIgniter\Commands\Sessions\CreateMigration

<table style="text-align:left">
<tr><th>Class</th><td>CreateMigration</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Commands\Sessions\CreateMigration</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">CodeIgniter\CLI\BaseCommand</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Creates a migration file for database sessions.
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Commands
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
<th><a href="#description"><strong>description</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>the Command&#039;s short description</td>
</tr>
<tr>
<th><a href="#usage"><strong>usage</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>the Command&#039;s usage</td>
</tr>
<tr>
<th><a href="#arguments"><strong>arguments</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>the Command&#039;s Arguments</td>
</tr>
<tr>
<th><a href="#options"><strong>options</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>the Command&#039;s Options</td>
</tr>

<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Creates a new migration file with the current timestamp.</td>
</tr>

</table>





### Properties


<hr>

#### $group

```php
protected $group = 'CodeIgniter';
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
protected $name = 'session:migration';
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

#### $description

```php
protected $description = 'Generates the migration file for database sessions.';
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

#### $usage

```php
protected $usage = 'session:migration';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
the Command's usage
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
the Command's Arguments
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

#### $options

```php
protected $options = [
	'-n' => 'Set migration namespace',
	'-g' => 'Set database group',
	'-t' => 'Set table name',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
the Command's Options
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
Creates a new migration file with the current timestamp.
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
<summary><small>Source: 28 lines (107 - 134)</small></summary>

```php
public function run(array $params)
{
	$config = new App();

	$tableName = CLI::getOption('t') ?? 'ci_sessions';

	$path = APPPATH . 'Database/Migrations/' . date('YmdHis_') . 'create_' . $tableName . '_table' . '.php';

	$data = [
		'namespace' => CLI::getOption('n') ?? APP_NAMESPACE ?? 'App',
		'DBGroup'   => CLI::getOption('g'),
		'tableName' => $tableName,
		'matchIP'   => $config->sessionMatchIP ?? false,
	];

	$template = view('\CodeIgniter\Commands\Sessions\Views\migration.tpl.php', $data, ['debug' => false]);
	$template = str_replace('@php', '<?php', $template);

	// Write the file out.
	helper('filesystem');
	if (! write_file($path, $template))
	{
		CLI::error(lang('Migrations.writeError', [$path]));
		return;
	}

	CLI::write('Created file: ' . CLI::color(str_replace(APPPATH, 'APPPATH/', $path), 'green'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Commands/Sessions/CreateMigration.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Server/Serve.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Utilities/Namespaces.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>