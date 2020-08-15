


 



<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/Console.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Commands.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Exceptions/CLIException.md">next</a></td>
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
<td>framework/system/CLI/Console.php
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
<a href="../../../../../../api/vendor/codeigniter4/framework/system/CodeIgniter.md"><strong>CodeIgniter\CodeIgniter</strong></a>
</td>
<td>CodeIgniter</td>
</tr>
</table>



 
## CodeIgniter\CLI\Console

<table style="text-align:left">
<tr><th>Class</th><td>Console</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\CLI\Console</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Console
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
<th><a href="#app"><strong>app</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Main CodeIgniter instance.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Console constructor.</td>
</tr>
<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runs the current command discovered on the CLI.</td>
</tr>
<tr>
<th><a href="#showHeader"><strong>showHeader</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Displays basic information about the Console.</td>
</tr>

</table>





### Properties


<hr>

#### $app

```php
protected $app;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Main CodeIgniter instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(CodeIgniter $app)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Console constructor.
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
<td><code>$app</code></td>
<td><em>\CodeIgniter\CodeIgniter
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (64 - 67)</small></summary>

```php
public function __construct(CodeIgniter $app)
{
	$this->app = $app;
}
```

</details>


<hr>

#### run()

```php
public function run(bool $useSafeOutput = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs the current command discovered on the CLI.
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
<td><code>$useSafeOutput</code></td>
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
<td>\CodeIgniter\HTTP\RequestInterface<br>\CodeIgniter\HTTP\Response<br>\CodeIgniter\HTTP\ResponseInterface<br>mixed
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 9 lines (79 - 87)</small></summary>

```php
public function run(bool $useSafeOutput = false)
{
	$path = CLI::getURI() ?: 'list';

	// Set the path for the application to route to.
	$this->app->setPath("ci{$path}");

	return $this->app->useSafeOutput($useSafeOutput)->run();
}
```

</details>


<hr>

#### showHeader()

```php
public function showHeader()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Displays basic information about the Console.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 10 lines (94 - 103)</small></summary>

```php
public function showHeader()
{
	CLI::newLine();

	CLI::write(CLI::color('CodeIgniter CLI Tool', 'green')
			. ' - Version ' . CodeIgniter::CI_VERSION
			. sprintf(' - Server Time: %s UTC%s', date('Y-m-d H:i:sa'), date('P')));

	CLI::newLine();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/Console.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Commands.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Exceptions/CLIException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:09**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>