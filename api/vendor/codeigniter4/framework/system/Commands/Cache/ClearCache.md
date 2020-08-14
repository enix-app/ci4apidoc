


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Commands/Cache/ClearCache.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/CodeIgniter.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Database/CreateMigration.md">next</a></td>
</tr>
</table>







# CodeIgniter\Commands\Cache 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Commands\Cache</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Cache/ClearCache.md">CodeIgniter\Commands\Cache\ClearCache</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheFactory.md"><strong>CodeIgniter\Cache\CacheFactory</strong></a>
</td>
<td>CacheFactory</td>
</tr>
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



 
## CodeIgniter\Commands\Cache\ClearCache

<table style="text-align:left">
<tr><th>Class</th><td>ClearCache</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Commands\Cache\ClearCache</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">CodeIgniter\CLI\BaseCommand</a></td></tr>
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
<td>Command grouping.</td>
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
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Clears the cache</td>
</tr>

</table>





### Properties


<hr>

#### $group

```php
protected $group = 'Cache';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Command grouping.
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
protected $name = 'cache:clear';
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
protected $description = 'Clears the current system caches.';
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
protected $usage = 'cache:clear [driver]';
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
protected $arguments = [
	'driver' => 'The cache driver to use',
];
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
Clears the cache
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
<summary><small>Source: 22 lines (51 - 72)</small></summary>

```php
public function run(array $params)
{
	$config = config('Cache');

	$handler = $params[0] ?? $config->handler;
	if (! array_key_exists($handler, $config->validHandlers))
	{
		CLI::error($handler . ' is not a valid cache handler.');
		return;
	}

	$config->handler = $handler;
	$cache           = CacheFactory::getHandler($config);

	if (! $cache->clean())
	{
		CLI::error('Error while clearing the cache.');
		return;
	}

	CLI::write(CLI::color('Done', 'green'));
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Commands/Cache/ClearCache.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/CodeIgniter.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Database/CreateMigration.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>