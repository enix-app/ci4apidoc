


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/FileRules.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FormatRules.md">next</a></td>
</tr>
</table>







# CodeIgniter\Validation 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Validation</td></tr>
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
<td>framework/system/Validation/FileRules.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/CreditCardRules.md">CodeIgniter\Validation\CreditCardRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md">CodeIgniter\Validation\Exceptions\ValidationException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FileRules.md">CodeIgniter\Validation\FileRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FormatRules.md">CodeIgniter\Validation\FormatRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Rules.md">CodeIgniter\Validation\Rules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md">CodeIgniter\Validation\Validation</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">CodeIgniter\Validation\ValidationInterface</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md"><strong>CodeIgniter\HTTP\RequestInterface</strong></a>
</td>
<td>RequestInterface</td>
</tr>
<tr>
<td>
<strong>Config\Services</strong>
</td>
<td>Services</td>
</tr>
</table>



 
## CodeIgniter\Validation\FileRules

<table style="text-align:left">
<tr><th>Class</th><td>FileRules</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Validation\FileRules</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
File validation rules
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
<th><a href="#request"><strong>request</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Request instance. So we can get access to the files.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor.</td>
</tr>
<tr>
<th><a href="#uploaded"><strong>uploaded</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Verifies that $name is the name of a valid uploaded file.</td>
</tr>
<tr>
<th><a href="#max_size"><strong>max_size</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Verifies if the file&#039;s size in Kilobytes is no larger than the parameter.</td>
</tr>
<tr>
<th><a href="#is_image"><strong>is_image</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Uses the mime config file to determine if a file is considered an &quot;image&quot;,
which for our purposes basically means that it&#039;s a raster image or svg.</td>
</tr>
<tr>
<th><a href="#mime_in"><strong>mime_in</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if an uploaded file&#039;s mime type matches one in the parameter.</td>
</tr>
<tr>
<th><a href="#ext_in"><strong>ext_in</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if an uploaded file&#039;s extension matches one in the parameter.</td>
</tr>
<tr>
<th><a href="#max_dims"><strong>max_dims</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks an uploaded file to verify that the dimensions are within
a specified allowable dimension.</td>
</tr>

</table>





### Properties


<hr>

#### $request

```php
protected $request;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Request instance. So we can get access to the files.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\HTTP\RequestInterface
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(RequestInterface $request = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor.
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
<td><code>$request</code></td>
<td><em>\RequestInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (65 - 73)</small></summary>

```php
public function __construct(RequestInterface $request = null)
{
	if (is_null($request))
	{
		$request = Services::request();
	}

	$this->request = $request;
}
```

</details>


<hr>

#### uploaded()

```php
public function uploaded(string $blank = null, string $name) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Verifies that $name is the name of a valid uploaded file.
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
<td><code>$blank</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$name</code></td>
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
<summary><small>Source: 35 lines (85 - 119)</small></summary>

```php
public function uploaded(string $blank = null, string $name): bool
{
	if (! ($files = $this->request->getFileMultiple($name)))
	{
		$files = [$this->request->getFile($name)];
	}

	foreach ($files as $file)
	{
		if (is_null($file))
		{
			return false;
		}

		if (ENVIRONMENT === 'testing')
		{
			if ($file->getError() !== 0)
			{
				return false;
			}
		}
		else
		{
			// Note: cannot unit test this; no way to over-ride ENVIRONMENT?
			// @codeCoverageIgnoreStart
			if (! $file->isValid())
			{
				return false;
			}
			// @codeCoverageIgnoreEnd
		}
	}

	return true;
}
```

</details>


<hr>

#### max_size()

```php
public function max_size(string $blank = null, string $params) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Verifies if the file's size in Kilobytes is no larger than the parameter.
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
<td><code>$blank</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
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
<summary><small>Source: 37 lines (131 - 167)</small></summary>

```php
public function max_size(string $blank = null, string $params): bool
{
	// Grab the file name off the top of the $params
	// after we split it.
	$params = explode(',', $params);
	$name   = array_shift($params);

	if (! ($files = $this->request->getFileMultiple($name)))
	{
		$files = [$this->request->getFile($name)];
	}

	foreach ($files as $file)
	{
		if (is_null($file))
		{
			return false;
		}

		if ($file->getError() === UPLOAD_ERR_NO_FILE)
		{
			return true;
		}

		if ($file->getError() === UPLOAD_ERR_INI_SIZE)
		{
			return false;
		}

		if ($file->getSize() / 1024 > $params[0])
		{
			return false;
		}
	}

	return true;
}
```

</details>


<hr>

#### is_image()

```php
public function is_image(string $blank = null, string $params) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Uses the mime config file to determine if a file is considered an "image",
which for our purposes basically means that it's a raster image or svg.
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
<td><code>$blank</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
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
<summary><small>Source: 36 lines (180 - 215)</small></summary>

```php
public function is_image(string $blank = null, string $params): bool
{
	// Grab the file name off the top of the $params
	// after we split it.
	$params = explode(',', $params);
	$name   = array_shift($params);

	if (! ($files = $this->request->getFileMultiple($name)))
	{
		$files = [$this->request->getFile($name)];
	}

	foreach ($files as $file)
	{
		if (is_null($file))
		{
			return false;
		}

		if ($file->getError() === UPLOAD_ERR_NO_FILE)
		{
			return true;
		}

		// We know that our mimes list always has the first mime
		// start with `image` even when then are multiple accepted types.
		$type = \Config\Mimes::guessTypeFromExtension($file->getExtension());

		if (mb_strpos($type, 'image') !== 0)
		{
			return false;
		}
	}

	return true;
}
```

</details>


<hr>

#### mime_in()

```php
public function mime_in(string $blank = null, string $params) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if an uploaded file's mime type matches one in the parameter.
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
<td><code>$blank</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
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
<summary><small>Source: 32 lines (227 - 258)</small></summary>

```php
public function mime_in(string $blank = null, string $params): bool
{
	// Grab the file name off the top of the $params
	// after we split it.
	$params = explode(',', $params);
	$name   = array_shift($params);

	if (! ($files = $this->request->getFileMultiple($name)))
	{
		$files = [$this->request->getFile($name)];
	}

	foreach ($files as $file)
	{
		if (is_null($file))
		{
			return false;
		}

		if ($file->getError() === UPLOAD_ERR_NO_FILE)
		{
			return true;
		}

		if (! in_array($file->getMimeType(), $params))
		{
			return false;
		}
	}

	return true;
}
```

</details>


<hr>

#### ext_in()

```php
public function ext_in(string $blank = null, string $params) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if an uploaded file's extension matches one in the parameter.
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
<td><code>$blank</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
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
<summary><small>Source: 32 lines (270 - 301)</small></summary>

```php
public function ext_in(string $blank = null, string $params): bool
{
	// Grab the file name off the top of the $params
	// after we split it.
	$params = explode(',', $params);
	$name   = array_shift($params);

	if (! ($files = $this->request->getFileMultiple($name)))
	{
		$files = [$this->request->getFile($name)];
	}

	foreach ($files as $file)
	{
		if (is_null($file))
		{
			return false;
		}

		if ($file->getError() === UPLOAD_ERR_NO_FILE)
		{
			return true;
		}

		if (! in_array($file->getExtension(), $params))
		{
			return false;
		}
	}

	return true;
}
```

</details>


<hr>

#### max_dims()

```php
public function max_dims(string $blank = null, string $params) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks an uploaded file to verify that the dimensions are within
a specified allowable dimension.
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
<td><code>$blank</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$params</code></td>
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
<summary><small>Source: 41 lines (314 - 354)</small></summary>

```php
public function max_dims(string $blank = null, string $params): bool
{
	// Grab the file name off the top of the $params
	// after we split it.
	$params = explode(',', $params);
	$name   = array_shift($params);

	if (! ($files = $this->request->getFileMultiple($name)))
	{
		$files = [$this->request->getFile($name)];
	}

	foreach ($files as $file)
	{
		if (is_null($file))
		{
			return false;
		}

		if ($file->getError() === UPLOAD_ERR_NO_FILE)
		{
			return true;
		}

		// Get Parameter sizes
		$allowedWidth  = $params[0] ?? 0;
		$allowedHeight = $params[1] ?? 0;

		// Get uploaded image size
		$info       = getimagesize($file->getTempName());
		$fileWidth  = $info[0];
		$fileHeight = $info[1];

		if ($fileWidth > $allowedWidth || $fileHeight > $allowedHeight)
		{
			return false;
		}
	}

	return true;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/FileRules.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FormatRules.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>