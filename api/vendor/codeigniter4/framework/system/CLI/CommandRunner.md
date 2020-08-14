


 



<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/CommandRunner.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CLI.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Commands.md">next</a></td>
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
<td>framework/system/CLI/CommandRunner.php
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
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Controller.md"><strong>CodeIgniter\Controller</strong></a>
</td>
<td>Controller</td>
</tr>
</table>



 
## CodeIgniter\CLI\CommandRunner

<table style="text-align:left">
<tr><th>Class</th><td>CommandRunner</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\CLI\CommandRunner</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Controller.md">CodeIgniter\Controller</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Command runner
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
<th><a href="#commands"><strong>commands</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Command Manager</td>
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
<th><a href="#_remap"><strong>_remap</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>We map all un-routed CLI methods through this function
so we have the chance to look for a Command first.</td>
</tr>
<tr>
<th><a href="#index"><strong>index</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Default command.</td>
</tr>
<tr>
<th><a href="#getCommands"><strong>getCommands</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows access to the current commands that have been found.</td>
</tr>

</table>





### Properties


<hr>

#### $commands

```php
protected $commands;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Command Manager
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Commands
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct()
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










<details>
<summary><small>Source: 4 lines (62 - 65)</small></summary>

```php
public function __construct()
{
	$this->commands = service('commands');
}
```

</details>


<hr>

#### _remap()

```php
public function _remap($method, ...$params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
We map all un-routed CLI methods through this function
so we have the chance to look for a Command first.
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
<summary><small>Source: 10 lines (77 - 86)</small></summary>

```php
public function _remap($method, ...$params)
{
	// The first param is usually empty, so scrap it.
	if (empty($params[0]))
	{
		array_shift($params);
	}

	return $this->index($params);
}
```

</details>


<hr>

#### index()

```php
public function index(array $params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Default command.
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
<summary><small>Source: 11 lines (98 - 108)</small></summary>

```php
public function index(array $params)
{
	$command = array_shift($params);

	if (is_null($command))
	{
		$command = 'list';
	}

	return service('commands')->run($command, $params);
}
```

</details>


<hr>

#### getCommands()

```php
public function getCommands() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows access to the current commands that have been found.
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
<summary><small>Source: 4 lines (115 - 118)</small></summary>

```php
public function getCommands(): array
{
	return $this->commands->getCommands();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/CommandRunner.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CLI.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Commands.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:07**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>