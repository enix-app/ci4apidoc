


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Image.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/ImageMagickHandler.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/ImageHandlerInterface.md">next</a></td>
</tr>
</table>







# CodeIgniter\Images 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Images</td></tr>
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
<td><a href="https://opensource.org/licenses/MIT">https://opensource.org/licenses/MIT</a>    MIT License
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com">https://codeigniter.com</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>filesource</th>
<td>framework/system/Images/Image.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Exceptions/ImageException.md">CodeIgniter\Images\Exceptions\ImageException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/BaseHandler.md">CodeIgniter\Images\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/GDHandler.md">CodeIgniter\Images\Handlers\GDHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/ImageMagickHandler.md">CodeIgniter\Images\Handlers\ImageMagickHandler</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Image.md">CodeIgniter\Images\Image</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/ImageHandlerInterface.md">CodeIgniter\Images\ImageHandlerInterface</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/File.md"><strong>CodeIgniter\Files\File</strong></a>
</td>
<td>File</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Exceptions/ImageException.md"><strong>CodeIgniter\Images\Exceptions\ImageException</strong></a>
</td>
<td>ImageException</td>
</tr>
</table>



 
## CodeIgniter\Images\Image

<table style="text-align:left">
<tr><th>Class</th><td>Image</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Images\Image</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Files/File.md">CodeIgniter\Files\File</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Encapsulation of an Image file
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
<th><a href="#origWidth"><strong>origWidth</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>The original image width in pixels.</td>
</tr>
<tr>
<th><a href="#origHeight"><strong>origHeight</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>The original image height in pixels.</td>
</tr>
<tr>
<th><a href="#imageType"><strong>imageType</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>The image type constant.</td>
</tr>
<tr>
<th><a href="#sizeStr"><strong>sizeStr</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>attributes string with size info:
&#039;height=&quot;100&quot; width=&quot;200&quot;&#039;</td>
</tr>
<tr>
<th><a href="#mime"><strong>mime</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>The image&#039;s mime type, i.e. image/jpeg</td>
</tr>

<tr>
<th><a href="#copy"><strong>copy</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Makes a copy of itself to the new location. If no filename is provided
it will use the existing filename.</td>
</tr>
<tr>
<th><a href="#getProperties"><strong>getProperties</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get image properties</td>
</tr>

</table>





### Properties


<hr>

#### $origWidth

```php
public $origWidth;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The original image width in pixels.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int<br>float
</td>
</tr>
</table>


<hr>

#### $origHeight

```php
public $origHeight;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The original image height in pixels.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int<br>float
</td>
</tr>
</table>


<hr>

#### $imageType

```php
public $imageType;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The image type constant.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $sizeStr

```php
public $sizeStr;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
attributes string with size info:
'height="100" width="200"'
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

#### $mime

```php
public $mime;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The image's mime type, i.e. image/jpeg
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







### Methods


<hr>

#### copy()

```php
public function copy(string $targetPath, string $targetName = null, int $perms = 0644) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Makes a copy of itself to the new location. If no filename is provided
it will use the existing filename.
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
<td>The directory to store the file in</td>
</tr>

<tr>
<td>2.</td>
<td><code>$targetName</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td>The new name of the copied file.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$perms</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>File permissions to be applied after copy.</td>
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
<summary><small>Source: 25 lines (99 - 123)</small></summary>

```php
public function copy(string $targetPath, string $targetName = null, int $perms = 0644): bool
{
	$targetPath = rtrim($targetPath, '/ ') . '/';

	$targetName = is_null($targetName) ? $this->getFilename() : $targetName;

	if (empty($targetName))
	{
		throw ImageException::forInvalidFile($targetName);
	}

	if (! is_dir($targetPath))
	{
		mkdir($targetName, 0755, true);
	}

	if (! copy($this->getPathname(), "{$targetPath}{$targetName}"))
	{
		throw ImageException::forCopyError($targetPath);
	}

	chmod("{$targetPath}/{$targetName}", $perms);

	return true;
}
```

</details>


<hr>

#### getProperties()

```php
public function getProperties(bool $return = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get image properties
</td></tr>
</table>

<table>
<tr><td>
A helper function that gets info about the file
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
<td><code>$return</code></td>
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
<td>array<br>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 37 lines (136 - 172)</small></summary>

```php
public function getProperties(bool $return = false)
{
	$path = $this->getPathname();

	if (! $vals = getimagesize($path))
	{
		throw ImageException::forFileNotSupported();
	}

	$types = [
		IMAGETYPE_GIF  => 'gif',
		IMAGETYPE_JPEG => 'jpeg',
		IMAGETYPE_PNG  => 'png',
		IMAGETYPE_WEBP => 'webp',
	];

	$mime = 'image/' . ($types[$vals[2]] ?? 'jpg');

	if ($return === true)
	{
		return [
			'width'      => $vals[0],
			'height'     => $vals[1],
			'image_type' => $vals[2],
			'size_str'   => $vals[3],
			'mime_type'  => $mime,
		];
	}

	$this->origWidth  = $vals[0];
	$this->origHeight = $vals[1];
	$this->imageType  = $vals[2];
	$this->sizeStr    = $vals[3];
	$this->mime       = $mime;

	return true;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Image.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/ImageMagickHandler.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/ImageHandlerInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:17**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>