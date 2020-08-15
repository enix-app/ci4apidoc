


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Commands/Encryption/GenerateKey.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Database/Seed.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Help.md">next</a></td>
</tr>
</table>







# CodeIgniter\Commands\Encryption 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Commands\Encryption</td></tr>
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
<td>framework/system/Commands/Encryption/GenerateKey.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Encryption/GenerateKey.md">CodeIgniter\Commands\Encryption\GenerateKey</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md"><strong>CodeIgniter\Config\DotEnv</strong></a>
</td>
<td>DotEnv</td>
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
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Encryption/Encryption.md"><strong>CodeIgniter\Encryption\Encryption</strong></a>
</td>
<td>Encryption</td>
</tr>
</table>



 
## CodeIgniter\Commands\Encryption\GenerateKey

<table style="text-align:left">
<tr><th>Class</th><td>GenerateKey</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Commands\Encryption\GenerateKey</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">CodeIgniter\CLI\BaseCommand</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates a new encryption key.
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
<th><a href="#group"><strong>group</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Command&#039;s group.</td>
</tr>
<tr>
<th><a href="#name"><strong>name</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Command&#039;s name.</td>
</tr>
<tr>
<th><a href="#usage"><strong>usage</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Command&#039;s usage.</td>
</tr>
<tr>
<th><a href="#description"><strong>description</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Command&#039;s short description.</td>
</tr>
<tr>
<th><a href="#options"><strong>options</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The command&#039;s options</td>
</tr>

<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Actually execute the command.</td>
</tr>
<tr>
<th><a href="#generateRandomKey"><strong>generateRandomKey</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Generates a key and encodes it.</td>
</tr>
<tr>
<th><a href="#setNewEncryptionKey"><strong>setNewEncryptionKey</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Sets the new encryption key in your .env file.</td>
</tr>
<tr>
<th><a href="#confirmOverwrite"><strong>confirmOverwrite</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Checks whether to overwrite existing encryption key.</td>
</tr>
<tr>
<th><a href="#writeNewEncryptionKeyToFile"><strong>writeNewEncryptionKeyToFile</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Writes the new encryption key to .env file.</td>
</tr>
<tr>
<th><a href="#keyPattern"><strong>keyPattern</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get the regex of the current encryption key.</td>
</tr>

</table>





### Properties


<hr>

#### $group

```php
protected $group = 'Encryption';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Command's group.
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
protected $name = 'key:generate';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Command's name.
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
protected $usage = 'key:generate [options]';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Command's usage.
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
protected $description = 'Generates a new encryption key and writes it in an `.env` file.';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Command's short description.
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
protected $options = [
	'-force'  => 'Force overwrite existing key in `.env` file.',
	'-length' => 'The length of the random string that should be returned in bytes. Defaults to 32.',
	'-prefix' => 'Prefix to prepend to encoded key (either hex2bin or base64). Defaults to hex2bin.',
	'-show'   => 'Shows the generated key in the terminal instead of storing in the `.env` file.',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The command's options
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
Actually execute the command.
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 45 lines (99 - 143)</small></summary>

```php
public function run(array $params)
{
	$prefix = $params['prefix'] ?? CLI::getOption('prefix');
	if (in_array($prefix, [null, true], true))
	{
		$prefix = 'hex2bin';
	}
	elseif (! in_array($prefix, ['hex2bin', 'base64'], true))
	{
		// @codeCoverageIgnoreStart
		$prefix = CLI::prompt('Please provide a valid prefix to use.', ['hex2bin', 'base64'], 'required');
		// @codeCoverageIgnoreEnd
	}

	$length = $params['length'] ?? CLI::getOption('length');
	if (in_array($length, [null, true], true))
	{
		$length = 32;
	}

	$encodedKey = $this->generateRandomKey($prefix, $length);

	if (array_key_exists('show', $params) || (bool) CLI::getOption('show'))
	{
		CLI::write($encodedKey, 'yellow');
		CLI::newLine();
		return;
	}

	if (! $this->setNewEncryptionKey($encodedKey, $params))
	{
		CLI::write('Error in setting new encryption key to .env file.', 'light_gray', 'red');
		CLI::newLine();
		return;
	}

	// force DotEnv to reload the new env vars
	putenv('encryption.key');
	unset($_ENV['encryption.key'], $_SERVER['encryption.key']);
	$dotenv = new DotEnv(ROOTPATH);
	$dotenv->load();

	CLI::write('Application\'s new encryption key was successfully set.', 'green');
	CLI::newLine();
}
```

</details>


<hr>

#### generateRandomKey()

```php
protected function generateRandomKey(string $prefix, int $length) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates a key and encodes it.
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
<td><code>$prefix</code></td>
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
<summary><small>Source: 11 lines (153 - 163)</small></summary>

```php
protected function generateRandomKey(string $prefix, int $length): string
{
	$key = Encryption::createKey($length);

	if ($prefix === 'hex2bin')
	{
		return 'hex2bin:' . bin2hex($key);
	}

	return 'base64:' . base64_encode($key);
}
```

</details>


<hr>

#### setNewEncryptionKey()

```php
protected function setNewEncryptionKey(string $key, array $params) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the new encryption key in your .env file.
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (173 - 186)</small></summary>

```php
protected function setNewEncryptionKey(string $key, array $params): bool
{
	$currentKey = env('encryption.key', '');

	if (strlen($currentKey) !== 0 && ! $this->confirmOverwrite($params))
	{
		// Not yet testable since it requires keyboard input
		// @codeCoverageIgnoreStart
		return false;
		// @codeCoverageIgnoreEnd
	}

	return $this->writeNewEncryptionKeyToFile($currentKey, $key);
}
```

</details>


<hr>

#### confirmOverwrite()

```php
protected function confirmOverwrite(array $params) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks whether to overwrite existing encryption key.
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (195 - 198)</small></summary>

```php
protected function confirmOverwrite(array $params): bool
{
	return (array_key_exists('force', $params) || CLI::getOption('force')) || CLI::prompt('Overwrite existing key?', ['n', 'y']) === 'y';
}
```

</details>


<hr>

#### writeNewEncryptionKeyToFile()

```php
protected function writeNewEncryptionKeyToFile(string $oldKey, string $newKey) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Writes the new encryption key to .env file.
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
<summary><small>Source: 26 lines (207 - 232)</small></summary>

```php
protected function writeNewEncryptionKeyToFile(string $oldKey, string $newKey): bool
{
	$baseEnv = ROOTPATH . 'env';
	$envFile = ROOTPATH . '.env';

	if (! file_exists($envFile))
	{
		if (! file_exists($baseEnv))
		{
			CLI::write('Both default shipped `env` file and custom `.env` are missing.', 'yellow');
			CLI::write('Here\'s your new key instead: ' . CLI::color($newKey, 'yellow'));
			CLI::newLine();
			return false;
		}

		copy($baseEnv, $envFile);
	}

	$ret = file_put_contents($envFile, preg_replace(
		$this->keyPattern($oldKey),
		"\nencryption.key = $newKey",
		file_get_contents($envFile)
	));

	return $ret !== false;
}
```

</details>


<hr>

#### keyPattern()

```php
protected function keyPattern(string $oldKey) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get the regex of the current encryption key.
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
<td><code>$oldKey</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (241 - 251)</small></summary>

```php
protected function keyPattern(string $oldKey): string
{
	$escaped = preg_quote($oldKey, '/');

	if ($escaped !== '')
	{
		$escaped = "[$escaped]*";
	}

	return "/^[#\s]*encryption.key[=\s]*{$escaped}$/m";
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Commands/Encryption/GenerateKey.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Database/Seed.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Commands/Help.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:09**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>