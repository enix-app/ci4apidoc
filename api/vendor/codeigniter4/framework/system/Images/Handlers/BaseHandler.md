


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Handlers/BaseHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Exceptions/ImageException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/GDHandler.md">next</a></td>
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
<td>framework/system/Images/Handlers/BaseHandler.php
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
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Image.md"><strong>CodeIgniter\Images\Image</strong></a>
</td>
<td>Image</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/ImageHandlerInterface.md"><strong>CodeIgniter\Images\ImageHandlerInterface</strong></a>
</td>
<td>ImageHandlerInterface</td>
</tr>
<tr>
<td>
<strong>Config\Images</strong>
</td>
<td>Images</td>
</tr>
</table>



 
## CodeIgniter\Images\Handlers\BaseHandler

<table style="text-align:left">
<tr><th>Abstract</th><td>BaseHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Images\Handlers\BaseHandler</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/ImageHandlerInterface.md">CodeIgniter\Images\ImageHandlerInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Base image handling implementation
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
<th><a href="#config"><strong>config</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Configuration settings.</td>
</tr>
<tr>
<th><a href="#image"><strong>image</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The image/file instance</td>
</tr>
<tr>
<th><a href="#verified"><strong>verified</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether the image file has been confirmed.</td>
</tr>
<tr>
<th><a href="#width"><strong>width</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Image width.</td>
</tr>
<tr>
<th><a href="#height"><strong>height</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Image height.</td>
</tr>
<tr>
<th><a href="#filePermissions"><strong>filePermissions</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>File permission mask.</td>
</tr>
<tr>
<th><a href="#xAxis"><strong>xAxis</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>X-axis.</td>
</tr>
<tr>
<th><a href="#yAxis"><strong>yAxis</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Y-axis.</td>
</tr>
<tr>
<th><a href="#masterDim"><strong>masterDim</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Master dimensioning.</td>
</tr>
<tr>
<th><a href="#textDefaults"><strong>textDefaults</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Default options for text watermarking.</td>
</tr>
<tr>
<th><a href="#resource"><strong>resource</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Temporary image used by the different engines.</td>
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
<th><a href="#withFile"><strong>withFile</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets another image for this handler to work on.</td>
</tr>
<tr>
<th><a href="#ensureResource"><strong>ensureResource</strong>()</a></th>
<td>method</td>
<td>
protected<br>abstract

</td>
<td>Make the image resource object if needed</td>
</tr>
<tr>
<th><a href="#getFile"><strong>getFile</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the image instance.</td>
</tr>
<tr>
<th><a href="#image"><strong>image</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Verifies that a file has been supplied and it is an image.</td>
</tr>
<tr>
<th><a href="#getResource"><strong>getResource</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the temporary image used during the image processing.</td>
</tr>
<tr>
<th><a href="#withResource"><strong>withResource</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Load the temporary image used during the image processing.</td>
</tr>
<tr>
<th><a href="#resize"><strong>resize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Resize the image</td>
</tr>
<tr>
<th><a href="#crop"><strong>crop</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Crops the image to the desired height and width. If one of the height/width values
is not provided, that value will be set the appropriate value based on offsets and
image dimensions.</td>
</tr>
<tr>
<th><a href="#convert"><strong>convert</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Changes the stored image type to indicate the new file format to use when saving.</td>
</tr>
<tr>
<th><a href="#rotate"><strong>rotate</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Rotates the image on the current canvas.</td>
</tr>
<tr>
<th><a href="#flatten"><strong>flatten</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Flattens transparencies, default white background</td>
</tr>
<tr>
<th><a href="#_flatten"><strong>_flatten</strong>()</a></th>
<td>method</td>
<td>
protected<br>abstract

</td>
<td>Handler-specific method to flattening an image&#039;s transparencies.</td>
</tr>
<tr>
<th><a href="#_rotate"><strong>_rotate</strong>()</a></th>
<td>method</td>
<td>
protected<br>abstract

</td>
<td>Handler-specific method to handle rotating an image in 90 degree increments.</td>
</tr>
<tr>
<th><a href="#flip"><strong>flip</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Flips an image either horizontally or vertically.</td>
</tr>
<tr>
<th><a href="#_flip"><strong>_flip</strong>()</a></th>
<td>method</td>
<td>
protected<br>abstract

</td>
<td>Handler-specific method to handle flipping an image along its
horizontal or vertical axis.</td>
</tr>
<tr>
<th><a href="#text"><strong>text</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Overlays a string of text over the image.</td>
</tr>
<tr>
<th><a href="#_text"><strong>_text</strong>()</a></th>
<td>method</td>
<td>
protected<br>abstract

</td>
<td>Handler-specific method for overlaying text on an image.</td>
</tr>
<tr>
<th><a href="#reorient"><strong>reorient</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Reads the EXIF information from the image and modifies the orientation
so that displays correctly in the browser. This is especially an issue
with images taken by smartphones who always store the image up-right,
but set the orientation flag to display it correctly.</td>
</tr>
<tr>
<th><a href="#getEXIF"><strong>getEXIF</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve the EXIF information from the image, if possible. Returns
an array of the information, or null if nothing can be found.</td>
</tr>
<tr>
<th><a href="#fit"><strong>fit</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Combine cropping and resizing into a single command.</td>
</tr>
<tr>
<th><a href="#calcAspectRatio"><strong>calcAspectRatio</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Calculate image aspect ratio.</td>
</tr>
<tr>
<th><a href="#calcCropCoords"><strong>calcCropCoords</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Based on the position, will determine the correct x/y coords to
crop the desired portion from the image.</td>
</tr>
<tr>
<th><a href="#getVersion"><strong>getVersion</strong>()</a></th>
<td>method</td>
<td>
public<br>abstract

</td>
<td>Get the version of the image library in use.</td>
</tr>
<tr>
<th><a href="#save"><strong>save</strong>()</a></th>
<td>method</td>
<td>
public<br>abstract

</td>
<td>Saves any changes that have been made to file.</td>
</tr>
<tr>
<th><a href="#process"><strong>process</strong>()</a></th>
<td>method</td>
<td>
protected<br>abstract

</td>
<td>Does the driver-specific processing of the image.</td>
</tr>
<tr>
<th><a href="#__call"><strong>__call</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Provide access to the Image class&#039; methods if they don&#039;t exist
on the handler itself.</td>
</tr>
<tr>
<th><a href="#reproportion"><strong>reproportion</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Re-proportion Image Width/Height</td>
</tr>
<tr>
<th><a href="#getWidth"><strong>getWidth</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return image width.</td>
</tr>
<tr>
<th><a href="#getHeight"><strong>getHeight</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return image height.</td>
</tr>

</table>





### Properties


<hr>

#### $config

```php
protected $config;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Configuration settings.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Config\Images
</td>
</tr>
</table>


<hr>

#### $image

```php
protected $image;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The image/file instance
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Images\Image
</td>
</tr>
</table>


<hr>

#### $verified

```php
protected $verified = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether the image file has been confirmed.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>bool
</td>
</tr>
</table>


<hr>

#### $width

```php
protected $width = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Image width.
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

#### $height

```php
protected $height = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Image height.
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

#### $filePermissions

```php
protected $filePermissions = 0644;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
File permission mask.
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

#### $xAxis

```php
protected $xAxis = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
X-axis.
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

#### $yAxis

```php
protected $yAxis = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Y-axis.
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

#### $masterDim

```php
protected $masterDim = 'auto';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Master dimensioning.
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

#### $textDefaults

```php
protected $textDefaults = [
	'fontPath'     => null,
	'fontSize'     => 16,
	'color'        => 'ffffff',
	'opacity'      => 1.0,
	'vAlign'       => 'bottom',
	'hAlign'       => 'center',
	'vOffset'      => 0,
	'hOffset'      => 0,
	'padding'      => 0,
	'withShadow'   => false,
	'shadowColor'  => '000000',
	'shadowOffset' => 3,
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Default options for text watermarking.
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

#### $resource

```php
protected $resource;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Temporary image used by the different engines.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>resource
</td>
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








<details>
<summary><small>Source: 4 lines (149 - 152)</small></summary>

```php
public function __construct($config = null)
{
	$this->config = $config ?? new Images();
}
```

</details>


<hr>

#### withFile()

```php
public function withFile(string $path)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets another image for this handler to work on.
</td></tr>
</table>

<table>
<tr><td>
Keeps us from needing to continually instantiate the handler.
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
<summary><small>Source: 15 lines (164 - 178)</small></summary>

```php
public function withFile(string $path)
{
	// Clear out the old resource so that
	// it doesn't try to use a previous image
	$this->resource = null;
	$this->verified = false;

	$this->image = new Image($path, true);

	$this->image->getProperties(false);
	$this->width  = $this->image->origWidth;
	$this->height = $this->image->origHeight;

	return $this;
}
```

</details>


<hr>

#### ensureResource()

```php
protected abstract function ensureResource()
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
<summary><small>Source: line 185</small></summary>

```php
protected abstract function ensureResource();
```

</details>


<hr>

#### getFile()

```php
public function getFile()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the image instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Images\Image
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (194 - 197)</small></summary>

```php
public function getFile()
{
	return $this->image;
}
```

</details>


<hr>

#### image()

```php
protected function image() : Image
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Verifies that a file has been supplied and it is an image.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Image
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
<summary><small>Source: 30 lines (205 - 234)</small></summary>

```php
protected function image(): Image
{
	if ($this->verified)
	{
		return $this->image;
	}

	// Verify withFile has been called
	if (empty($this->image))
	{
		throw ImageException::forMissingImage();
	}

	// Verify the loaded image is an Image instance
	if (! $this->image instanceof Image)
	{
		throw ImageException::forInvalidPath();
	}

	// File::__construct has verified the file exists - make sure it is an image
	if (! is_int($this->image->imageType))
	{
		throw ImageException::forFileNotSupported();
	}

	// Note that the image has been verified
	$this->verified = true;

	return $this->image;
}
```

</details>


<hr>

#### getResource()

```php
public function getResource()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the temporary image used during the image processing.
</td></tr>
</table>

<table>
<tr><td>
Good for extending the system or doing things this library
is not intended to do.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>resource
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (245 - 249)</small></summary>

```php
public function getResource()
{
	$this->ensureResource();
	return $this->resource;
}
```

</details>


<hr>

#### withResource()

```php
public function withResource()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Load the temporary image used during the image processing.
</td></tr>
</table>

<table>
<tr><td>
Some functions e.g. save() will only copy and not compress
your image otherwise.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (260 - 264)</small></summary>

```php
public function withResource()
{
	$this->ensureResource();
	return $this;
}
```

</details>


<hr>

#### resize()

```php
public function resize(int $width, int $height, bool $maintainRatio = false, string $masterDim = 'auto')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Resize the image
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
<td><code>$width</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$height</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$maintainRatio</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>If true, will get the closest match possible while keeping aspect ratio true.</td>
</tr>

<tr>
<td>4.</td>
<td><code>$masterDim</code></td>
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
<td>\BaseHandler
</td>
</tr>
</table>





<details>
<summary><small>Source: 19 lines (278 - 296)</small></summary>

```php
public function resize(int $width, int $height, bool $maintainRatio = false, string $masterDim = 'auto')
{
	// If the target width/height match the source, then we have nothing to do here.
	if ($this->image()->origWidth === $width && $this->image()->origHeight === $height)
	{
		return $this;
	}

	$this->width  = $width;
	$this->height = $height;

	if ($maintainRatio)
	{
		$this->masterDim = $masterDim;
		$this->reproportion();
	}

	return $this->_resize($maintainRatio);
}
```

</details>


<hr>

#### crop()

```php
public function crop(int $width = null, int $height = null, int $x = null, int $y = null, bool $maintainRatio = false, string $masterDim = 'auto')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Crops the image to the desired height and width. If one of the height/width values
is not provided, that value will be set the appropriate value based on offsets and
image dimensions.
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
<td><code>$width</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$height</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$x</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td>X-axis coord to start cropping from the left of image</td>
</tr>

<tr>
<td>4.</td>
<td><code>$y</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td>Y-axis coord to start cropping from the top of image</td>
</tr>

<tr>
<td>5.</td>
<td><code>$maintainRatio</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>6.</td>
<td><code>$masterDim</code></td>
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
<summary><small>Source: 20 lines (314 - 333)</small></summary>

```php
public function crop(int $width = null, int $height = null, int $x = null, int $y = null, bool $maintainRatio = false, string $masterDim = 'auto')
{
	$this->width  = $width;
	$this->height = $height;
	$this->xAxis  = $x;
	$this->yAxis  = $y;

	if ($maintainRatio)
	{
		$this->masterDim = $masterDim;
		$this->reproportion();
	}

	$result = $this->_crop();

	$this->xAxis = null;
	$this->yAxis = null;

	return $result;
}
```

</details>


<hr>

#### convert()

```php
public function convert(int $imageType)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Changes the stored image type to indicate the new file format to use when saving.
</td></tr>
</table>

<table>
<tr><td>
Does not touch the actual resource.
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
<td><code>$imageType</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td>A PHP imageType constant, e.g. <a href="https://www.php.net/manual/en/function.image-type-to-mime-type.php">https://www.php.net/manual/en/function.image-type-to-mime-type.php</a></td>
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
<summary><small>Source: 5 lines (345 - 349)</small></summary>

```php
public function convert(int $imageType)
{
	$this->image()->imageType = $imageType;
	return $this;
}
```

</details>


<hr>

#### rotate()

```php
public function rotate(float $angle)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Rotates the image on the current canvas.
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
<td><em>float
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
<summary><small>Source: 30 lines (360 - 389)</small></summary>

```php
public function rotate(float $angle)
{
	// Allowed rotation values
	$degs = [
		90,
		180,
		270,
	];

	if ($angle === '' || ! in_array($angle, $degs))
	{
		throw ImageException::forMissingAngle();
	}

	// cast angle as an int, for our use
	$angle = (int) $angle;

	// Reassign the width and height
	if ($angle === 90 || $angle === 270)
	{
		$temp         = $this->height;
		$this->width  = $this->height;
		$this->height = $temp;
	}

	// Call the Handler-specific version.
	$this->_rotate($angle);

	return $this;
}
```

</details>


<hr>

#### flatten()

```php
public function flatten(int $red = 255, int $green = 255, int $blue = 255)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Flattens transparencies, default white background
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
<summary><small>Source: 7 lines (402 - 408)</small></summary>

```php
public function flatten(int $red = 255, int $green = 255, int $blue = 255)
{
	$this->width  = $this->image()->origWidth;
	$this->height = $this->image()->origHeight;

	return $this->_flatten();
}
```

</details>


<hr>

#### _flatten()

```php
protected abstract function _flatten(int $red = 255, int $green = 255, int $blue = 255)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handler-specific method to flattening an image's transparencies.
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>internal</th>
<td>
</td>
</tr>
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
<summary><small>Source: line 422</small></summary>

```php
protected abstract function _flatten(int $red = 255, int $green = 255, int $blue = 255);
```

</details>


<hr>

#### _rotate()

```php
protected abstract function _rotate(int $angle)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handler-specific method to handle rotating an image in 90 degree increments.
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: line 433</small></summary>

```php
protected abstract function _rotate(int $angle);
```

</details>


<hr>

#### flip()

```php
public function flip(string $dir = 'vertical')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Flips an image either horizontally or vertically.
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
<td><code>$dir</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Either 'vertical' or 'horizontal'</td>
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
<summary><small>Source: 11 lines (444 - 454)</small></summary>

```php
public function flip(string $dir = 'vertical')
{
	$dir = strtolower($dir);

	if ($dir !== 'vertical' && $dir !== 'horizontal')
	{
		throw ImageException::forInvalidDirection($dir);
	}

	return $this->_flip($dir);
}
```

</details>


<hr>

#### _flip()

```php
protected abstract function _flip(string $direction)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handler-specific method to handle flipping an image along its
horizontal or vertical axis.
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
<summary><small>Source: line 466</small></summary>

```php
protected abstract function _flip(string $direction);
```

</details>


<hr>

#### text()

```php
public function text(string $text, array $options = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Overlays a string of text over the image.
</td></tr>
</table>

<table>
<tr><td>
Valid options:

- color         Text Color (hex number)
- shadowColor   Color of the shadow (hex number)
- hAlign        Horizontal alignment: left, center, right
- vAlign        Vertical alignment: top, middle, bottom
- hOffset
- vOffset
- fontPath
- fontSize
- shadowOffset
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (490 - 499)</small></summary>

```php
public function text(string $text, array $options = [])
{
	$options                = array_merge($this->textDefaults, $options);
	$options['color']       = trim($options['color'], '# ');
	$options['shadowColor'] = trim($options['shadowColor'], '# ');

	$this->_text($text, $options);

	return $this;
}
```

</details>


<hr>

#### _text()

```php
protected abstract function _text(string $text, array $options = array())
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


</tbody>
</table>








<details>
<summary><small>Source: line 509</small></summary>

```php
protected abstract function _text(string $text, array $options = []);
```

</details>


<hr>

#### reorient()

```php
public function reorient(bool $silent = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reads the EXIF information from the image and modifies the orientation
so that displays correctly in the browser. This is especially an issue
with images taken by smartphones who always store the image up-right,
but set the orientation flag to display it correctly.
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
<td><code>$silent</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>If true, will ignore exceptions when PHP doesn't support EXIF.</td>
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
<summary><small>Source: 27 lines (523 - 549)</small></summary>

```php
public function reorient(bool $silent = false)
{
	$orientation = $this->getEXIF('Orientation', $silent);

	switch ($orientation)
	{
		case 2:
			return $this->flip('horizontal');
		case 3:
			return $this->rotate(180);
		case 4:
			return $this->rotate(180)
							->flip('horizontal');
		case 5:
			return $this->rotate(270)
							->flip('horizontal');
		case 6:
			return $this->rotate(270);
		case 7:
			return $this->rotate(90)
							->flip('horizontal');
		case 8:
			return $this->rotate(90);
		default:
			return $this;
	}
}
```

</details>


<hr>

#### getEXIF()

```php
public function getEXIF(string $key = null, bool $silent = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve the EXIF information from the image, if possible. Returns
an array of the information, or null if nothing can be found.
</td></tr>
</table>

<table>
<tr><td>
EXIF data is only supported fr JPEG & TIFF formats.
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
<td><em>string<br>null
</em></td>
<td>false</td>
<td>If specified, will only return this piece of EXIF data.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$silent</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>If true, will not throw our own exceptions.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 24 lines (564 - 587)</small></summary>

```php
public function getEXIF(string $key = null, bool $silent = false)
{
	if (! function_exists('exif_read_data'))
	{
		if ($silent)
		{
			return null;
		}
	}

	$exif = null; // default
	switch ($this->image()->imageType)
	{
		case IMAGETYPE_JPEG:
		case IMAGETYPE_TIFF_II:
			$exif = exif_read_data($this->image()->getPathname());
			if (! is_null($key) && is_array($exif))
			{
				$exif = $exif[$key] ?? false;
			}
	}

	return $exif;
}
```

</details>


<hr>

#### fit()

```php
public function fit(int $width, int $height = null, string $position = 'center')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Combine cropping and resizing into a single command.
</td></tr>
</table>

<table>
<tr><td>
Supported positions:
- top-left
- top
- top-right
- left
- center
- right
- bottom-left
- bottom
- bottom-right
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
<td><code>$width</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$height</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$position</code></td>
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
<summary><small>Source: 17 lines (611 - 627)</small></summary>

```php
public function fit(int $width, int $height = null, string $position = 'center')
{
	$origWidth  = $this->image()->origWidth;
	$origHeight = $this->image()->origHeight;

	list($cropWidth, $cropHeight) = $this->calcAspectRatio($width, $height, $origWidth, $origHeight);

	if (is_null($height))
	{
		$height = ceil(($width / $cropWidth) * $cropHeight);
	}

	list($x, $y) = $this->calcCropCoords($cropWidth, $cropHeight, $origWidth, $origHeight, $position);

	return $this->crop($cropWidth, $cropHeight, $x, $y)
					->resize($width, $height);
}
```

</details>


<hr>

#### calcAspectRatio()

```php
protected function calcAspectRatio($width, $height = null, $origWidth, $origHeight) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Calculate image aspect ratio.
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
<td><code>$width</code></td>
<td><em>int<br>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$height</code></td>
<td><em>int<br>float<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$origWidth</code></td>
<td><em>int<br>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$origHeight</code></td>
<td><em>int<br>float
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 30 lines (641 - 670)</small></summary>

```php
protected function calcAspectRatio($width, $height = null, $origWidth, $origHeight): array
{
	// If $height is null, then we have it easy.
	// Calc based on full image size and be done.
	if (is_null($height))
	{
		$height = ($width / $origWidth) * $origHeight;

		return [
			$width,
			(int) $height,
		];
	}

	$xRatio = $width / $origWidth;
	$yRatio = $height / $origHeight;

	if ($xRatio > $yRatio)
	{
		return [
			$origWidth,
			(int) ($origWidth * $height / $width),
		];
	}

	return [
		(int) ($origHeight * $width / $height),
		$origHeight,
	];
}
```

</details>


<hr>

#### calcCropCoords()

```php
protected function calcCropCoords($width, $height, $origWidth, $origHeight, $position) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Based on the position, will determine the correct x/y coords to
crop the desired portion from the image.
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
<td><code>$width</code></td>
<td><em>int<br>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$height</code></td>
<td><em>int<br>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$origWidth</code></td>
<td><em>int<br>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$origHeight</code></td>
<td><em>int<br>float
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$position</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 50 lines (686 - 735)</small></summary>

```php
protected function calcCropCoords($width, $height, $origWidth, $origHeight, $position): array
{
	$position = strtolower($position);
	$x        = $y = 0;

	switch ($position)
	{
		case 'top-left':
			$x = 0;
			$y = 0;
			break;
		case 'top':
			$x = floor(($origWidth - $width) / 2);
			$y = 0;
			break;
		case 'top-right':
			$x = $origWidth - $width;
			$y = 0;
			break;
		case 'left':
			$x = 0;
			$y = floor(($origHeight - $height) / 2);
			break;
		case 'center':
			$x = floor(($origWidth - $width) / 2);
			$y = floor(($origHeight - $height) / 2);
			break;
		case 'right':
			$x = ($origWidth - $width);
			$y = floor(($origHeight - $height) / 2);
			break;
		case 'bottom-left':
			$x = 0;
			$y = $origHeight - $height;
			break;
		case 'bottom':
			$x = floor(($origWidth - $width) / 2);
			$y = $origHeight - $height;
			break;
		case 'bottom-right':
			$x = ($origWidth - $width);
			$y = $origHeight - $height;
			break;
	}

	return [
		$x,
		$y,
	];
}
```

</details>


<hr>

#### getVersion()

```php
public abstract function getVersion()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get the version of the image library in use.
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
<summary><small>Source: line 744</small></summary>

```php
public abstract function getVersion();
```

</details>


<hr>

#### save()

```php
public abstract function save(string $target = null, int $quality = 90)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Saves any changes that have been made to file.
</td></tr>
</table>

<table>
<tr><td>
Example:
$image->resize(100, 200, true)
      ->save($target);
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
<summary><small>Source: line 760</small></summary>

```php
public abstract function save(string $target = null, int $quality = 90);
```

</details>


<hr>

#### process()

```php
protected abstract function process(string $action)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Does the driver-specific processing of the image.
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: line 771</small></summary>

```php
protected abstract function process(string $action);
```

</details>


<hr>

#### __call()

```php
public function __call(string $name, array $args = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provide access to the Image class' methods if they don't exist
on the handler itself.
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
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$args</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 7 lines (784 - 790)</small></summary>

```php
public function __call(string $name, array $args = [])
{
	if (method_exists($this->image(), $name))
	{
		return $this->image()->$name(...$args);
	}
}
```

</details>


<hr>

#### reproportion()

```php
protected function reproportion()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Re-proportion Image Width/Height
</td></tr>
</table>

<table>
<tr><td>
When creating thumbs, the desired width/height
can end up warping the image due to an incorrect
ratio between the full-sized image and the thumb.

This function lets us re-proportion the width/height
if users choose to maintain the aspect ratio when resizing.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 43 lines (806 - 848)</small></summary>

```php
protected function reproportion()
{
	if (($this->width === 0 && $this->height === 0) ||
			$this->image()->origWidth === 0 ||
			$this->image()->origHeight === 0 ||
			( ! ctype_digit((string) $this->width) && ! ctype_digit((string) $this->height)) ||
			! ctype_digit((string) $this->image()->origWidth) ||
			! ctype_digit((string) $this->image()->origHeight)
	)
	{
		return;
	}

	// Sanitize
	$this->width  = (int) $this->width;
	$this->height = (int) $this->height;

	if ($this->masterDim !== 'width' && $this->masterDim !== 'height')
	{
		if ($this->width > 0 && $this->height > 0)
		{
			$this->masterDim = ((($this->image()->origHeight / $this->image()->origWidth) - ($this->height / $this->width)) < 0) ? 'width' : 'height';
		}
		else
		{
			$this->masterDim = ($this->height === 0) ? 'width' : 'height';
		}
	}
	elseif (($this->masterDim === 'width' && $this->width === 0) || ($this->masterDim === 'height' && $this->height === 0)
	)
	{
		return;
	}

	if ($this->masterDim === 'width')
	{
		$this->height = (int) ceil($this->width * $this->image()->origHeight / $this->image()->origWidth);
	}
	else
	{
		$this->width = (int) ceil($this->image()->origWidth * $this->height / $this->image()->origHeight);
	}
}
```

</details>


<hr>

#### getWidth()

```php
public function getWidth()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return image width.
</td></tr>
</table>

<table>
<tr><td>
accessor for testing; not part of interface
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
<summary><small>Source: 4 lines (859 - 862)</small></summary>

```php
public function getWidth()
{
	return ($this->resource !== null) ? $this->_getWidth() : $this->width;
}
```

</details>


<hr>

#### getHeight()

```php
public function getHeight()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return image height.
</td></tr>
</table>

<table>
<tr><td>
accessor for testing; not part of interface
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
<summary><small>Source: 4 lines (871 - 874)</small></summary>

```php
public function getHeight()
{
	return ($this->resource !== null) ? $this->_getHeight() : $this->height;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Handlers/BaseHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Exceptions/ImageException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/GDHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:13**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>