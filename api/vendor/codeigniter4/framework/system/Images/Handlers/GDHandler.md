


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Handlers/GDHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/BaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/ImageMagickHandler.md">next</a></td>
</tr>
</table>







# CodeIgniter\Images\Handlers 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Images\Handlers</td></tr>
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
<td>framework/system/Images/Handlers/GDHandler.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/BaseHandler.md">CodeIgniter\Images\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/GDHandler.md">CodeIgniter\Images\Handlers\GDHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/ImageMagickHandler.md">CodeIgniter\Images\Handlers\ImageMagickHandler</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Exceptions/ImageException.md"><strong>CodeIgniter\Images\Exceptions\ImageException</strong></a>
</td>
<td>ImageException</td>
</tr>
</table>



 
## CodeIgniter\Images\Handlers\GDHandler

<table style="text-align:left">
<tr><th>Class</th><td>GDHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Images\Handlers\GDHandler</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/BaseHandler.md">CodeIgniter\Images\Handlers\BaseHandler</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Image handler for GD package
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
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor.</td>
</tr>
<tr>
<th><a href="#_rotate"><strong>_rotate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Handles the rotation of an image resource.</td>
</tr>
<tr>
<th><a href="#_flatten"><strong>_flatten</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Flattens transparencies</td>
</tr>
<tr>
<th><a href="#_flip"><strong>_flip</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Flips an image along it&#039;s vertical or horizontal axis.</td>
</tr>
<tr>
<th><a href="#getVersion"><strong>getVersion</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get GD version</td>
</tr>
<tr>
<th><a href="#_resize"><strong>_resize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Resizes the image.</td>
</tr>
<tr>
<th><a href="#_crop"><strong>_crop</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Crops the image.</td>
</tr>
<tr>
<th><a href="#process"><strong>process</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Handles all of the grunt work of resizing, etc.</td>
</tr>
<tr>
<th><a href="#save"><strong>save</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Saves any changes that have been made to file. If no new filename is
provided, the existing image is overwritten, otherwise a copy of the
file is made at $target.</td>
</tr>
<tr>
<th><a href="#createImage"><strong>createImage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Create Image Resource</td>
</tr>
<tr>
<th><a href="#ensureResource"><strong>ensureResource</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Make the image resource object if needed</td>
</tr>
<tr>
<th><a href="#getImageResource"><strong>getImageResource</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Check if image type is supported and return image resource</td>
</tr>
<tr>
<th><a href="#_text"><strong>_text</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Add text overlay to an image.</td>
</tr>
<tr>
<th><a href="#textOverlay"><strong>textOverlay</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Handler-specific method for overlaying text on an image.</td>
</tr>
<tr>
<th><a href="#_getWidth"><strong>_getWidth</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return image width.</td>
</tr>
<tr>
<th><a href="#_getHeight"><strong>_getHeight</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return image height.</td>
</tr>

</table>






### Methods


<hr>

#### __construct()

```php
public function __construct($config = null)
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
<td><code>$config</code></td>
<td><em>\Config\Images<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ImageException
</td>
</tr>
</table>



<details>
<summary><small>Source: 12 lines (55 - 66)</small></summary>

```php
public function __construct($config = null)
{
	parent::__construct($config);

	// We should never see this, so can't test it
	// @codeCoverageIgnoreStart
	if (! extension_loaded('gd'))
	{
		throw ImageException::forMissingExtension('GD');
	}
	// @codeCoverageIgnoreEnd
}
```

</details>


<hr>

#### _rotate()

```php
protected function _rotate(int $angle) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles the rotation of an image resource.
</td></tr>
</table>

<table>
<tr><td>
Doesn't save the image, but replaces the current resource.
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
<td><code>$angle</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 22 lines (78 - 99)</small></summary>

```php
protected function _rotate(int $angle): bool
{
	// Create the image handle
	$srcImg = $this->createImage();

	// Set the background color
	// This won't work with transparent PNG files so we are
	// going to have to figure out how to determine the color
	// of the alpha channel in a future release.

	$white = imagecolorallocate($srcImg, 255, 255, 255);

	// Rotate it!
	$destImg = imagerotate($srcImg, $angle, $white);

	// Kill the file handles
	imagedestroy($srcImg);

	$this->resource = $destImg;

	return true;
}
```

</details>


<hr>

#### _flatten()

```php
public function _flatten(int $red = 255, int $green = 255, int $blue = 255)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Flattens transparencies
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
<td><code>$red</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$green</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$blue</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 28 lines (112 - 139)</small></summary>

```php
public function _flatten(int $red = 255, int $green = 255, int $blue = 255)
{
	$srcImg = $this->createImage();

	if (function_exists('imagecreatetruecolor'))
	{
		$create = 'imagecreatetruecolor';
		$copy   = 'imagecopyresampled';
	}
	else
	{
		$create = 'imagecreate';
		$copy   = 'imagecopyresized';
	}
	$dest = $create($this->width, $this->height);

	$matte = imagecolorallocate($dest, $red, $green, $blue);

	imagefilledrectangle($dest, 0, 0, $this->width, $this->height, $matte);
	imagecopy($dest, $srcImg, 0, 0, 0, 0, $this->width, $this->height);

	// Kill the file handles
	imagedestroy($srcImg);

	$this->resource = $dest;

	return $this;
}
```

</details>


<hr>

#### _flip()

```php
public function _flip(string $direction)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Flips an image along it's vertical or horizontal axis.
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
<td><code>$direction</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 12 lines (150 - 161)</small></summary>

```php
public function _flip(string $direction)
{
	$srcImg = $this->createImage();

	$angle = $direction === 'horizontal' ? IMG_FLIP_HORIZONTAL : IMG_FLIP_VERTICAL;

	imageflip($srcImg, $angle);

	$this->resource = $srcImg;

	return $this;
}
```

</details>


<hr>

#### getVersion()

```php
public function getVersion()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get GD version
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (170 - 180)</small></summary>

```php
public function getVersion()
{
	if (function_exists('gd_info'))
	{
		$gd_version = @gd_info();

		return preg_replace('/\D/', '', $gd_version['GD Version']);
	}

	return false;
}
```

</details>


<hr>

#### _resize()

```php
public function _resize()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Resizes the image.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Images\Handlers\GDHandler
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (189 - 192)</small></summary>

```php
public function _resize()
{
	return $this->process('resize');
}
```

</details>


<hr>

#### _crop()

```php
public function _crop()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Crops the image.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Images\Handlers\GDHandler
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (201 - 204)</small></summary>

```php
public function _crop()
{
	return $this->process('crop');
}
```

</details>


<hr>

#### process()

```php
protected function process(string $action)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles all of the grunt work of resizing, etc.
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
<td><code>$action</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 47 lines (215 - 261)</small></summary>

```php
protected function process(string $action)
{
	$origWidth  = $this->image()->origWidth;
	$origHeight = $this->image()->origHeight;

	if ($action === 'crop')
	{
		// Reassign the source width/height if cropping
		$origWidth  = $this->width;
		$origHeight = $this->height;

		// Modify the "original" width/height to the new
		// values so that methods that come after have the
		// correct size to work with.
		$this->image()->origHeight = $this->height;
		$this->image()->origWidth  = $this->width;
	}

	// Create the image handle
	$src = $this->createImage();

	if (function_exists('imagecreatetruecolor'))
	{
		$create = 'imagecreatetruecolor';
		$copy   = 'imagecopyresampled';
	}
	else
	{
		$create = 'imagecreate';
		$copy   = 'imagecopyresized';
	}

	$dest = $create($this->width, $this->height);

	if ($this->image()->imageType === IMAGETYPE_PNG) // png we can actually preserve transparency
	{
		imagealphablending($dest, false);
		imagesavealpha($dest, true);
	}

	$copy($dest, $src, 0, 0, $this->xAxis, $this->yAxis, $this->width, $this->height, $origWidth, $origHeight);

	imagedestroy($src);
	$this->resource = $dest;

	return $this;
}
```

</details>


<hr>

#### save()

```php
public function save(string $target = null, int $quality = 90) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Saves any changes that have been made to file. If no new filename is
provided, the existing image is overwritten, otherwise a copy of the
file is made at $target.
</td></tr>
</table>

<table>
<tr><td>
Example:
$image->resize(100, 200, true)
      ->save();
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
<td><code>$target</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$quality</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 78 lines (279 - 356)</small></summary>

```php
public function save(string $target = null, int $quality = 90): bool
{
	$original = $target;
	$target   = empty($target) ? $this->image()->getPathname() : $target;

	// If no new resource has been created, then we're
	// simply copy the existing one.
	if (empty($this->resource) && $quality === 100)
	{
		if ($original === null)
		{
			return true;
		}

		$name = basename($target);
		$path = pathinfo($target, PATHINFO_DIRNAME);

		return $this->image()->copy($path, $name);
	}

	$this->ensureResource();

	switch ($this->image()->imageType)
	{
		case IMAGETYPE_GIF:
			if (! function_exists('imagegif'))
			{
				throw ImageException::forInvalidImageCreate(lang('images.gifNotSupported'));
			}

			if (! @imagegif($this->resource, $target))
			{
				throw ImageException::forSaveFailed();
			}
			break;
		case IMAGETYPE_JPEG:
			if (! function_exists('imagejpeg'))
			{
				throw ImageException::forInvalidImageCreate(lang('images.jpgNotSupported'));
			}

			if (! @imagejpeg($this->resource, $target, $quality))
			{
				throw ImageException::forSaveFailed();
			}
			break;
		case IMAGETYPE_PNG:
			if (! function_exists('imagepng'))
			{
				throw ImageException::forInvalidImageCreate(lang('images.pngNotSupported'));
			}

			if (! @imagepng($this->resource, $target))
			{
				throw ImageException::forSaveFailed();
			}
			break;
		case IMAGETYPE_WEBP:
			if (! function_exists('imagewebp'))
			{
				throw ImageException::forInvalidImageCreate(lang('images.webpNotSupported'));
			}

			if (! @imagewebp($this->resource, $target))
			{
				throw ImageException::forSaveFailed();
			}
			break;
		default:
			throw ImageException::forInvalidImageCreate();
	}

	imagedestroy($this->resource);

	chmod($target, $this->filePermissions);

	return true;
}
```

</details>


<hr>

#### createImage()

```php
protected function createImage(string $path = '', string $imageType = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create Image Resource
</td></tr>
</table>

<table>
<tr><td>
This simply creates an image resource handle
based on the type of image being processed
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
<td><code>$imageType</code></td>
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
<td>resource<br>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 19 lines (371 - 389)</small></summary>

```php
protected function createImage(string $path = '', string $imageType = '')
{
	if ($this->resource !== null)
	{
		return $this->resource;
	}

	if ($path === '')
	{
		$path = $this->image()->getPathname();
	}

	if ($imageType === '')
	{
		$imageType = $this->image()->imageType;
	}

	return $this->getImageResource($path, $imageType);
}
```

</details>


<hr>

#### ensureResource()

```php
protected function ensureResource()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Make the image resource object if needed
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 10 lines (396 - 405)</small></summary>

```php
protected function ensureResource()
{
	if ($this->resource === null)
	{
		// if valid image type, make corresponding image resource
		$this->resource = $this->getImageResource(
			$this->image()->getPathname(), $this->image()->imageType
		);
	}
}
```

</details>


<hr>

#### getImageResource()

```php
protected function getImageResource(string $path, int $imageType)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Check if image type is supported and return image resource
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
<td>Image path</td>
</tr>

<tr>
<td>2.</td>
<td><code>$imageType</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Image type</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>resource<br>bool
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ImageException
</td>
</tr>
</table>



<details>
<summary><small>Source: 36 lines (418 - 453)</small></summary>

```php
protected function getImageResource(string $path, int $imageType)
{
	switch ($imageType)
	{
		case IMAGETYPE_GIF:
			if (! function_exists('imagecreatefromgif'))
			{
				throw ImageException::forInvalidImageCreate(lang('images.gifNotSupported'));
			}

			return imagecreatefromgif($path);
		case IMAGETYPE_JPEG:
			if (! function_exists('imagecreatefromjpeg'))
			{
				throw ImageException::forInvalidImageCreate(lang('images.jpgNotSupported'));
			}

			return imagecreatefromjpeg($path);
		case IMAGETYPE_PNG:
			if (! function_exists('imagecreatefrompng'))
			{
				throw ImageException::forInvalidImageCreate(lang('images.pngNotSupported'));
			}

			return imagecreatefrompng($path);
		case IMAGETYPE_WEBP:
			if (! function_exists('imagecreatefromwebp'))
			{
				throw ImageException::forInvalidImageCreate(lang('images.webpNotSupported'));
			}

			return imagecreatefromwebp($path);
		default:
			throw ImageException::forInvalidImageCreate('Ima');
	}
}
```

</details>


<hr>

#### _text()

```php
protected function _text(string $text, array $options = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add text overlay to an image.
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
<td><code>$text</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
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
<summary><small>Source: 86 lines (465 - 550)</small></summary>

```php
protected function _text(string $text, array $options = [])
{
	// Reverse the vertical offset
	// When the image is positioned at the bottom
	// we don't want the vertical offset to push it
	// further down. We want the reverse, so we'll
	// invert the offset. Note: The horizontal
	// offset flips itself automatically

	if ($options['vAlign'] === 'bottom')
	{
		$options['vOffset'] = $options['vOffset'] * -1;
	}

	if ($options['hAlign'] === 'right')
	{
		$options['hOffset'] = $options['hOffset'] * -1;
	}

	// Set font width and height
	// These are calculated differently depending on
	// whether we are using the true type font or not
	if (! empty($options['fontPath']))
	{
		if (function_exists('imagettfbbox'))
		{
			$temp = imagettfbbox($options['fontSize'], 0, $options['fontPath'], $text);
			$temp = $temp[2] - $temp[0];

			$fontwidth = $temp / strlen($text);
		}
		else
		{
			$fontwidth = $options['fontSize'] - ($options['fontSize'] / 4);
		}

		$fontheight = $options['fontSize'];
	}
	else
	{
		$fontwidth  = imagefontwidth($options['fontSize']);
		$fontheight = imagefontheight($options['fontSize']);
	}

	$options['fontheight'] = $fontheight;
	$options['fontwidth']  = $fontwidth;

	// Set base X and Y axis values
	$xAxis = $options['hOffset'] + $options['padding'];
	$yAxis = $options['vOffset'] + $options['padding'];

	// Set vertical alignment
	if ($options['vAlign'] === 'middle')
	{
		// Don't apply padding when you're in the middle of the image.
		$yAxis += ($this->image()->origHeight / 2) + ($fontheight / 2) - $options['padding'] - $fontheight - $options['shadowOffset'];
	}
	elseif ($options['vAlign'] === 'bottom')
	{
		$yAxis = ($this->image()->origHeight - $fontheight - $options['shadowOffset'] - ($fontheight / 2)) - $yAxis;
	}

	// Set horizontal alignment
	if ($options['hAlign'] === 'right')
	{
		$xAxis += ($this->image()->origWidth - ($fontwidth * strlen($text)) - $options['shadowOffset']) - (2 * $options['padding']);
	}
	elseif ($options['hAlign'] === 'center')
	{
		$xAxis += floor(($this->image()->origWidth - ($fontwidth * strlen($text))) / 2);
	}

	$options['xAxis'] = $xAxis;
	$options['yAxis'] = $yAxis;

	if ($options['withShadow'])
	{
		// Offset from text
		$options['xShadow'] = $xAxis + $options['shadowOffset'];
		$options['yShadow'] = $yAxis + $options['shadowOffset'];

		$this->textOverlay($text, $options, true);
	}

	$this->textOverlay($text, $options);
}
```

</details>


<hr>

#### textOverlay()

```php
protected function textOverlay(string $text, array $options = array(), bool $isShadow = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handler-specific method for overlaying text on an image.
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
<td><code>$text</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$isShadow</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether we are drawing the dropshadow or actual text</td>
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
<summary><small>Source: 41 lines (563 - 603)</small></summary>

```php
protected function textOverlay(string $text, array $options = [], bool $isShadow = false)
{
	$src = $this->createImage();

	/* Set RGB values for shadow
	 *
	 * Get the rest of the string and split it into 2-length
	 * hex values:
	 */
	$opacity = ($options['opacity'] * 127);

	// Allow opacity to be applied to the text
	imagealphablending($src, true);

	$color = $isShadow ? $options['shadowColor'] : $options['color'];

	// shorthand hex, #f00
	if (strlen($color) === 3)
	{
		$color = implode('', array_map('str_repeat', str_split($color), [2, 2, 2]));
	}

	$color = str_split(substr($color, 0, 6), 2);
	$color = imagecolorclosestalpha($src, hexdec($color[0]), hexdec($color[1]), hexdec($color[2]), $opacity);

	$xAxis = $isShadow ? $options['xShadow'] : $options['xAxis'];
	$yAxis = $isShadow ? $options['yShadow'] : $options['yAxis'];

	// Add the shadow to the source image
	if (! empty($options['fontPath']))
	{
		// We have to add fontheight because imagettftext locates the bottom left corner, not top-left corner.
		imagettftext($src, $options['fontSize'], 0, $xAxis, $yAxis + $options['fontheight'], $color, $options['fontPath'], $text);
	}
	else
	{
		imagestring($src, $options['fontSize'], $xAxis, $yAxis, $text, $color);
	}

	$this->resource = $src;
}
```

</details>


<hr>

#### _getWidth()

```php
public function _getWidth()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return image width.
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
<summary><small>Source: 4 lines (612 - 615)</small></summary>

```php
public function _getWidth()
{
	return imagesx($this->resource);
}
```

</details>


<hr>

#### _getHeight()

```php
public function _getHeight()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return image height.
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
<summary><small>Source: 4 lines (622 - 625)</small></summary>

```php
public function _getHeight()
{
	return imagesy($this->resource);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Handlers/GDHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/BaseHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/ImageMagickHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:17**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>