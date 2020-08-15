


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/CacheFactory.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Exceptions/CLIException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md">next</a></td>
</tr>
</table>







# CodeIgniter\Cache 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Cache</td></tr>
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
<td>framework/system/Cache/CacheFactory.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheFactory.md">CodeIgniter\Cache\CacheFactory</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md">CodeIgniter\Cache\CacheInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/CacheException.md">CodeIgniter\Cache\Exceptions\CacheException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/ExceptionInterface.md">CodeIgniter\Cache\Exceptions\ExceptionInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/DummyHandler.md">CodeIgniter\Cache\Handlers\DummyHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/FileHandler.md">CodeIgniter\Cache\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/MemcachedHandler.md">CodeIgniter\Cache\Handlers\MemcachedHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/PredisHandler.md">CodeIgniter\Cache\Handlers\PredisHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/RedisHandler.md">CodeIgniter\Cache\Handlers\RedisHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Handlers/WincacheHandler.md">CodeIgniter\Cache\Handlers\WincacheHandler</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/Exceptions/CacheException.md"><strong>CodeIgniter\Cache\Exceptions\CacheException</strong></a>
</td>
<td>CacheException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CriticalError.md"><strong>CodeIgniter\Exceptions\CriticalError</strong></a>
</td>
<td>CriticalError</td>
</tr>
</table>



 
## CodeIgniter\Cache\CacheFactory

<table style="text-align:left">
<tr><th>Class</th><td>CacheFactory</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Cache\CacheFactory</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Cache
</td></tr>
</table>

<table>
<tr><td>
A factory for loading the desired
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Cache
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
<th><a href="#getHandler"><strong>getHandler</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Attempts to create the desired cache handler, based upon the</td>
</tr>

</table>






### Methods


<hr>

#### getHandler()

```php
public static function getHandler($config, string $handler = null, string $backup = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to create the desired cache handler, based upon the
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
<td><em>\Config\Cache
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$handler</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$backup</code></td>
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
<td>\CodeIgniter\Cache\CacheInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: 52 lines (63 - 114)</small></summary>

```php
public static function getHandler($config, string $handler = null, string $backup = null)
{
	if (! isset($config->validHandlers) || ! is_array($config->validHandlers))
	{
		throw CacheException::forInvalidHandlers();
	}

	if (! isset($config->handler) || ! isset($config->backupHandler))
	{
		throw CacheException::forNoBackup();
	}

	$handler = ! empty($handler) ? $handler : $config->handler;
	$backup  = ! empty($backup) ? $backup : $config->backupHandler;

	if (! array_key_exists($handler, $config->validHandlers) || ! array_key_exists($backup, $config->validHandlers))
	{
		throw CacheException::forHandlerNotFound();
	}

	// Get an instance of our handler.
	$adapter = new $config->validHandlers[$handler]($config);

	if (! $adapter->isSupported())
	{
		$adapter = new $config->validHandlers[$backup]($config);

		if (! $adapter->isSupported())
		{
			// Log stuff here, don't throw exception. No need to raise a fuss.
			// Fall back to the dummy adapter.
			$adapter = new $config->validHandlers['dummy']();
		}
	}

	// If $adapter->initialization throws a CriticalError exception, we will attempt to
	// use the $backup handler, if that also fails, we resort to the dummy handler.
	try
	{
		$adapter->initialize();
	}
	catch (CriticalError $e)
	{
		// log the fact that an exception occurred as well what handler we are resorting to
		log_message('critical', $e->getMessage() . ' Resorting to using ' . $backup . ' handler.');

		// get the next best cache handler (or dummy if the $backup also fails)
		$adapter = self::getHandler($config, $backup, 'dummy');
	}

	return $adapter;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Cache/CacheFactory.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Exceptions/CLIException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Cache/CacheInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:09**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>