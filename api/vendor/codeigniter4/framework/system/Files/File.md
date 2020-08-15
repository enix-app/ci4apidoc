


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Files/File.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileNotFoundException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/CSRF.md">next</a></td>
</tr>
</table>







# CodeIgniter\Files 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Files</td></tr>
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
<td>framework/system/Files/File.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileException.md">CodeIgniter\Files\Exceptions\FileException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileNotFoundException.md">CodeIgniter\Files\Exceptions\FileNotFoundException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/File.md">CodeIgniter\Files\File</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileException.md"><strong>CodeIgniter\Files\Exceptions\FileException</strong></a>
</td>
<td>FileException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileNotFoundException.md"><strong>CodeIgniter\Files\Exceptions\FileNotFoundException</strong></a>
</td>
<td>FileNotFoundException</td>
</tr>
<tr>
<td>
<strong>SplFileInfo</strong>
</td>
<td>SplFileInfo</td>
</tr>
</table>



 
## CodeIgniter\Files\File

<table style="text-align:left">
<tr><th>Class</th><td>File</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Files\File</td></tr>
<tr><th>Extends</th><td><a href="">SplFileInfo</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Wrapper for PHP's built-in SplFileInfo, with goodies.
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Files
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
<th><a href="#size"><strong>size</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The files size in bytes</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Run our SplFileInfo constructor with an optional verification
that the path is really a file.</td>
</tr>
<tr>
<th><a href="#getSize"><strong>getSize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve the file size.</td>
</tr>
<tr>
<th><a href="#getSizeByUnit"><strong>getSizeByUnit</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve the file size by unit.</td>
</tr>
<tr>
<th><a href="#guessExtension"><strong>guessExtension</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attempts to determine the file extension based on the trusted
getType() method. If the mime type is unknown, will return null.</td>
</tr>
<tr>
<th><a href="#getMimeType"><strong>getMimeType</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve the media type of the file. SHOULD not use information from
the $_FILES array, but should use other methods to more accurately
determine the type of file, like finfo, or mime_content_type().</td>
</tr>
<tr>
<th><a href="#getRandomName"><strong>getRandomName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Generates a random names based on a simple hash and the time, with
the correct file extension attached.</td>
</tr>
<tr>
<th><a href="#move"><strong>move</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Moves a file to a new location.</td>
</tr>
<tr>
<th><a href="#getDestination"><strong>getDestination</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the destination path for the move operation where overwriting is not expected.</td>
</tr>

</table>





### Properties


<hr>

#### $size

```php
protected $size;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The files size in bytes
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>float
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct(string $path, bool $checkFile = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Run our SplFileInfo constructor with an optional verification
that the path is really a file.
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
<td><code>$path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$checkFile</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 9 lines (70 - 78)</small></summary>

```php
public function __construct(string $path, bool $checkFile = false)
{
	if ($checkFile && ! is_file($path))
	{
		throw FileNotFoundException::forFileNotFound($path);
	}

	parent::__construct($path);
}
```

</details>


<hr>

#### getSize()

```php
public function getSize()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve the file size.
</td></tr>
</table>

<table>
<tr><td>
Implementations SHOULD return the value stored in the "size" key of
the file in the $_FILES array if available, as PHP calculates this based
on the actual size transmitted.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (91 - 99)</small></summary>

```php
public function getSize()
{
	if (is_null($this->size))
	{
		$this->size = parent::getSize();
	}

	return $this->size;
}
```

</details>


<hr>

#### getSizeByUnit()

```php
public function getSizeByUnit(string $unit = 'b')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve the file size by unit.
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
<td><code>$unit</code></td>
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
<td>int<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 12 lines (108 - 119)</small></summary>

```php
public function getSizeByUnit(string $unit = 'b')
{
	switch (strtolower($unit))
	{
		case 'kb':
			return number_format($this->getSize() / 1024, 3);
		case 'mb':
			return number_format(($this->getSize() / 1024) / 1024, 3);
		default:
			return $this->getSize();
	}
}
```

</details>


<hr>

#### guessExtension()

```php
public function guessExtension() : ?string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to determine the file extension based on the trusted
getType() method. If the mime type is unknown, will return null.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (129 - 132)</small></summary>

```php
public function guessExtension(): ?string
{
	return \Config\Mimes::guessExtensionFromType($this->getMimeType());
}
```

</details>


<hr>

#### getMimeType()

```php
public function getMimeType() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve the media type of the file. SHOULD not use information from
the $_FILES array, but should use other methods to more accurately
determine the type of file, like finfo, or mime_content_type().
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (143 - 156)</small></summary>

```php
public function getMimeType(): string
{
	if (! function_exists('finfo_open'))
	{
		// @codeCoverageIgnoreStart
		return $this->originalMimeType ?? 'application/octet-stream';
		// @codeCoverageIgnoreEnd
	}

	$finfo    = finfo_open(FILEINFO_MIME_TYPE);
	$mimeType = finfo_file($finfo, $this->getRealPath());
	finfo_close($finfo);
	return $mimeType;
}
```

</details>


<hr>

#### getRandomName()

```php
public function getRandomName() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Generates a random names based on a simple hash and the time, with
the correct file extension attached.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (166 - 171)</small></summary>

```php
public function getRandomName(): string
{
	$extension = $this->getExtension();
	$extension = empty($extension) ? '' : '.' . $extension;
	return time() . '_' . bin2hex(random_bytes(10)) . $extension;
}
```

</details>


<hr>

#### move()

```php
public function move(string $targetPath, string $name = null, bool $overwrite = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Moves a file to a new location.
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
<td><code>$targetPath</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$name</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$overwrite</code></td>
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
<td>\CodeIgniter\Files\File
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (184 - 201)</small></summary>

```php
public function move(string $targetPath, string $name = null, bool $overwrite = false)
{
	$targetPath  = rtrim($targetPath, '/') . '/';
	$name        = $name ?? $this->getBaseName();
	$destination = $overwrite ? $targetPath . $name : $this->getDestination($targetPath . $name);

	$oldName = empty($this->getRealPath()) ? $this->getPath() : $this->getRealPath();

	if (! @rename($oldName, $destination))
	{
		$error = error_get_last();
		throw FileException::forUnableToMove($this->getBasename(), $targetPath, strip_tags($error['message']));
	}

	@chmod($destination, 0777 & ~umask());

	return new File($destination);
}
```

</details>


<hr>

#### getDestination()

```php
public function getDestination(string $destination, string $delimiter = '_', int $i = 0) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the destination path for the move operation where overwriting is not expected.
</td></tr>
</table>

<table>
<tr><td>
First, it checks whether the delimiter is present in the filename, if it is, then it checks whether the
last element is an integer as there may be cases that the delimiter may be present in the filename.
For the all other cases, it appends an integer starting from zero before the file's extension.
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
<td><code>$destination</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$delimiter</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$i</code></td>
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
<summary><small>Source: 28 lines (218 - 245)</small></summary>

```php
public function getDestination(string $destination, string $delimiter = '_', int $i = 0): string
{
	while (is_file($destination))
	{
		$info      = pathinfo($destination);
		$extension = isset($info['extension']) ? '.' . $info['extension'] : '';
		if (strpos($info['filename'], $delimiter) !== false)
		{
			$parts = explode($delimiter, $info['filename']);
			if (is_numeric(end($parts)))
			{
				$i = end($parts);
				array_pop($parts);
				array_push($parts, ++ $i);
				$destination = $info['dirname'] . '/' . implode($delimiter, $parts) . $extension;
			}
			else
			{
				$destination = $info['dirname'] . '/' . $info['filename'] . $delimiter . ++ $i . $extension;
			}
		}
		else
		{
			$destination = $info['dirname'] . '/' . $info['filename'] . $delimiter . ++ $i . $extension;
		}
	}
	return $destination;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Files/File.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/Exceptions/FileNotFoundException.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Filters/CSRF.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>