


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Config/AutoloadConfig.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/ComposerScripts.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">next</a></td>
</tr>
</table>







# CodeIgniter\Config 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Config</td></tr>
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
<td>framework/system/Config/AutoloadConfig.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/AutoloadConfig.md">CodeIgniter\Config\AutoloadConfig</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">CodeIgniter\Config\BaseConfig</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseService.md">CodeIgniter\Config\BaseService</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Config.md">CodeIgniter\Config\Config</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md">CodeIgniter\Config\DotEnv</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/ForeignCharacters.md">CodeIgniter\Config\ForeignCharacters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Services.md">CodeIgniter\Config\Services</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/View.md">CodeIgniter\Config\View</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Config\AutoloadConfig

<table style="text-align:left">
<tr><th>Class</th><td>AutoloadConfig</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Config\AutoloadConfig</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
AUTO-LOADER
</td></tr>
</table>

<table>
<tr><td>
This file defines the namespaces and class maps so the Autoloader
can find the files as needed.
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
<th><a href="#corePsr4"><strong>corePsr4</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>-------------------------------------------------------------------
Namespaces
-------------------------------------------------------------------
This maps the locations of any namespaces in your application to
their location on the file system. These are used by the autoloader
to locate files the first time they have been instantiated.</td>
</tr>
<tr>
<th><a href="#coreClassmap"><strong>coreClassmap</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>-------------------------------------------------------------------
Class Map
-------------------------------------------------------------------
The class map provides a map of class names and their exact
location on the drive. Classes loaded in this manner will have
slightly faster performance because they will not have to be
searched for within one or more directories as they would if they
were being autoloaded through a namespace.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor.</td>
</tr>

</table>





### Properties


<hr>

#### $corePsr4

```php
protected $corePsr4 = [
	'CodeIgniter' => SYSTEMPATH,
	'App'         => APPPATH, // To ensure filters, etc still found,
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
-------------------------------------------------------------------
Namespaces
-------------------------------------------------------------------
This maps the locations of any namespaces in your application to
their location on the file system. These are used by the autoloader
to locate files the first time they have been instantiated.
</td></tr>
</table>

<table>
<tr><td>
Do not change the name of the CodeIgniter namespace or your application
will break.
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

#### $coreClassmap

```php
protected $coreClassmap = [
	'Psr\Log\AbstractLogger'           => SYSTEMPATH . 'ThirdParty/PSR/Log/AbstractLogger.php',
	'Psr\Log\InvalidArgumentException' => SYSTEMPATH . 'ThirdParty/PSR/Log/InvalidArgumentException.php',
	'Psr\Log\LoggerAwareInterface'     => SYSTEMPATH . 'ThirdParty/PSR/Log/LoggerAwareInterface.php',
	'Psr\Log\LoggerAwareTrait'         => SYSTEMPATH . 'ThirdParty/PSR/Log/LoggerAwareTrait.php',
	'Psr\Log\LoggerInterface'          => SYSTEMPATH . 'ThirdParty/PSR/Log/LoggerInterface.php',
	'Psr\Log\LoggerTrait'              => SYSTEMPATH . 'ThirdParty/PSR/Log/LoggerTrait.php',
	'Psr\Log\LogLevel'                 => SYSTEMPATH . 'ThirdParty/PSR/Log/LogLevel.php',
	'Psr\Log\NullLogger'               => SYSTEMPATH . 'ThirdParty/PSR/Log/NullLogger.php',
	'Laminas\Escaper\Escaper'          => SYSTEMPATH . 'ThirdParty/Escaper/Escaper.php',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
-------------------------------------------------------------------
Class Map
-------------------------------------------------------------------
The class map provides a map of class names and their exact
location on the drive. Classes loaded in this manner will have
slightly faster performance because they will not have to be
searched for within one or more directories as they would if they
were being autoloaded through a namespace.
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
public function __construct()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor.
</td></tr>
</table>

<table>
<tr><td>
Merge the built-in and developer-configured psr4 and classmap,
with preference to the developer ones.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 12 lines (101 - 112)</small></summary>

```php
public function __construct()
{
	if (isset($_SERVER['CI_ENVIRONMENT']) && $_SERVER['CI_ENVIRONMENT'] === 'testing')
	{
		$this->psr4['Tests\Support']                  = SUPPORTPATH;
		$this->classmap['CodeIgniter\Log\TestLogger'] = SYSTEMPATH . 'Test/TestLogger.php';
		$this->classmap['CIDatabaseTestCase']         = SYSTEMPATH . 'Test/CIDatabaseTestCase.php';
	}

	$this->psr4     = array_merge($this->corePsr4, $this->psr4);
	$this->classmap = array_merge($this->coreClassmap, $this->classmap);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Config/AutoloadConfig.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/ComposerScripts.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:10**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>