


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Config/View.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Services.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Controller.md">next</a></td>
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
<td>framework/system/Config/View.php
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



 

 
## CodeIgniter\Config\View

<table style="text-align:left">
<tr><th>Class</th><td>View</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Config\View</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">CodeIgniter\Config\BaseConfig</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
View configuration
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
<th><a href="#coreFilters"><strong>coreFilters</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Built-in View filters.</td>
</tr>
<tr>
<th><a href="#corePlugins"><strong>corePlugins</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Built-in View plugins.</td>
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

#### $coreFilters

```php
protected $coreFilters = [
	'abs'            => '\abs',
	'capitalize'     => '\CodeIgniter\View\Filters::capitalize',
	'date'           => '\CodeIgniter\View\Filters::date',
	'date_modify'    => '\CodeIgniter\View\Filters::date_modify',
	'default'        => '\CodeIgniter\View\Filters::default',
	'esc'            => '\CodeIgniter\View\Filters::esc',
	'excerpt'        => '\CodeIgniter\View\Filters::excerpt',
	'highlight'      => '\CodeIgniter\View\Filters::highlight',
	'highlight_code' => '\CodeIgniter\View\Filters::highlight_code',
	'limit_words'    => '\CodeIgniter\View\Filters::limit_words',
	'limit_chars'    => '\CodeIgniter\View\Filters::limit_chars',
	'local_currency' => '\CodeIgniter\View\Filters::local_currency',
	'local_number'   => '\CodeIgniter\View\Filters::local_number',
	'lower'          => '\strtolower',
	'nl2br'          => '\CodeIgniter\View\Filters::nl2br',
	'number_format'  => '\number_format',
	'prose'          => '\CodeIgniter\View\Filters::prose',
	'round'          => '\CodeIgniter\View\Filters::round',
	'strip_tags'     => '\strip_tags',
	'title'          => '\CodeIgniter\View\Filters::title',
	'upper'          => '\strtoupper',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Built-in View filters.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\type
</td>
</tr>
</table>


<hr>

#### $corePlugins

```php
protected $corePlugins = [
	'current_url'       => '\CodeIgniter\View\Plugins::currentURL',
	'previous_url'      => '\CodeIgniter\View\Plugins::previousURL',
	'mailto'            => '\CodeIgniter\View\Plugins::mailto',
	'safe_mailto'       => '\CodeIgniter\View\Plugins::safeMailto',
	'lang'              => '\CodeIgniter\View\Plugins::lang',
	'validation_errors' => '\CodeIgniter\View\Plugins::validationErrors',
	'route'             => '\CodeIgniter\View\Plugins::route',
	'siteURL'           => '\CodeIgniter\View\Plugins::siteURL',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Built-in View plugins.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\type
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
Merge the built-in and developer-configured filters and plugins,
with preference to the developer ones.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 7 lines (99 - 105)</small></summary>

```php
public function __construct()
{
	$this->filters = array_merge($this->coreFilters, $this->filters);
	$this->plugins = array_merge($this->corePlugins, $this->plugins);

	parent::__construct();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Config/View.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Services.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Controller.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>