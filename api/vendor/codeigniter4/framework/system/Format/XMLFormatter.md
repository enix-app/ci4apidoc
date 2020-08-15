


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Format/XMLFormatter.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/JSONFormatter.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/CLIRequest.md">next</a></td>
</tr>
</table>







# CodeIgniter\Format 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Format</td></tr>
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
<td>framework/system/Format/XMLFormatter.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/Exceptions/FormatException.md">CodeIgniter\Format\Exceptions\FormatException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/FormatterInterface.md">CodeIgniter\Format\FormatterInterface</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/JSONFormatter.md">CodeIgniter\Format\JSONFormatter</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/XMLFormatter.md">CodeIgniter\Format\XMLFormatter</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/Exceptions/FormatException.md"><strong>CodeIgniter\Format\Exceptions\FormatException</strong></a>
</td>
<td>FormatException</td>
</tr>
<tr>
<td>
<strong>Config\Format</strong>
</td>
<td>Format</td>
</tr>
</table>



 
## CodeIgniter\Format\XMLFormatter

<table style="text-align:left">
<tr><th>Class</th><td>XMLFormatter</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Format\XMLFormatter</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/FormatterInterface.md">CodeIgniter\Format\FormatterInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
XML data formatter
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
<th><a href="#format"><strong>format</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Takes the given data and formats it.</td>
</tr>
<tr>
<th><a href="#arrayToXML"><strong>arrayToXML</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A recursive method to convert an array into a valid XML string.</td>
</tr>

</table>






### Methods


<hr>

#### format()

```php
public function format($data)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes the given data and formats it.
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
<td><code>$data</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 21 lines (58 - 78)</small></summary>

```php
public function format($data)
{
	$config = new Format();

	// SimpleXML is installed but default
	// but best to check, and then provide a fallback.
	if (! extension_loaded('simplexml'))
	{
		// never thrown in travis-ci
		// @codeCoverageIgnoreStart
		throw FormatException::forMissingExtension();
		// @codeCoverageIgnoreEnd
	}

	$options = $config->formatterOptions['application/xml'] ?? 0;
	$output  = new \SimpleXMLElement('<?xml version="1.0"?><response></response>', $options);

	$this->arrayToXML((array)$data, $output);

	return $output->asXML();
}
```

</details>


<hr>

#### arrayToXML()

```php
protected function arrayToXML(array $data, &$output)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A recursive method to convert an array into a valid XML string.
</td></tr>
</table>

<table>
<tr><td>
Written by CodexWorld. Received permission by email on Nov 24, 2016 to use this code.
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
<td><code>$data</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$output</code></td>
<td><em>\SimpleXMLElement
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 25 lines (92 - 116)</small></summary>

```php
protected function arrayToXML(array $data, &$output)
{
	foreach ($data as $key => $value)
	{
		if (is_array($value))
		{
			if (is_numeric($key))
			{
				$key = "item{$key}";
			}

			$subnode = $output->addChild("$key");
			$this->arrayToXML($value, $subnode);
		}
		else
		{
			if (is_numeric($key))
			{
				$key = "item{$key}";
			}

			$output->addChild("$key", htmlspecialchars("$value"));
		}
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Format/XMLFormatter.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Format/JSONFormatter.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/CLIRequest.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>