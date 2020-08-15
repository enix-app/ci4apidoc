


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Handlers/ImageMagickHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/GDHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Image.md">next</a></td>
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
<td>framework/system/Images/Handlers/ImageMagickHandler.php
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



 
## CodeIgniter\Images\Handlers\ImageMagickHandler

<table style="text-align:left">
<tr><th>Class</th><td>ImageMagickHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Images\Handlers\ImageMagickHandler</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/BaseHandler.md">CodeIgniter\Images\Handlers\BaseHandler</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class ImageMagickHandler
</td></tr>
</table>

<table>
<tr><td>
To make this library as compatible as possible with the broadest
number of installations, we do not use the Imagick extension,
but simply use the command line version.

hmm - the width & height accessors at the end use the imagick extension.

FIXME - This needs conversion & unit testing, to use the imagick extension
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Images\Handlers
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
<th><a href="#resource"><strong>resource</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores image resource in memory.</td>
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
<th><a href="#_resize"><strong>_resize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Handles the actual resizing of the image.</td>
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
<td>Flattens transparencies, default white background</td>
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
<td>Get driver version</td>
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
<th><a href="#getResourcePath"><strong>getResourcePath</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get Image Resource</td>
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
<th><a href="#supportedFormatCheck"><strong>supportedFormatCheck</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Check if given image format is supported</td>
</tr>
<tr>
<th><a href="#_text"><strong>_text</strong>()</a></th>
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
<td>Return the width of an image.</td>
</tr>
<tr>
<th><a href="#_getHeight"><strong>_getHeight</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the height of an image.</td>
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

</table>





### Properties


<hr>

#### $resource

```php
protected $resource;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores image resource in memory.
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
<td><em>\Config\Images
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
<summary><small>Source: 12 lines (75 - 86)</small></summary>

```php
public function __construct($config = null)
{
	parent::__construct($config);

	// We should never see this, so can't test it
	// @codeCoverageIgnoreStart
	if (! (extension_loaded('imagick') || class_exists('Imagick')))
	{
		throw ImageException::forMissingExtension('IMAGICK');
	}
	// @codeCoverageIgnoreEnd
}
```

</details>


<hr>

#### _resize()

```php
public function _resize(bool $maintainRatio = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles the actual resizing of the image.
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
<td><code>$maintainRatio</code></td>
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
<td>\ImageMagickHandler
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 19 lines (98 - 116)</small></summary>

```php
public function _resize(bool $maintainRatio = false)
{
	$source      = ! empty($this->resource) ? $this->resource : $this->image()->getPathname();
	$destination = $this->getResourcePath();

	$escape = '\\';
	if (stripos(PHP_OS, 'WIN') === 0)
	{
		$escape = '';
	}

	$action = $maintainRatio === true
		? ' -resize ' . ($this->width ?? 0) . 'x' . ($this->height ?? 0) . ' "' . $source . '" "' . $destination . '"'
		: ' -resize ' . ($this->width ?? 0) . 'x' . ($this->height ?? 0) . "{$escape}! \"" . $source . '" "' . $destination . '"';

	$this->process($action);

	return $this;
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
<td>bool<br>\CodeIgniter\Images\Handlers\ImageMagickHandler
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 17 lines (126 - 142)</small></summary>

```php
public function _crop()
{
	$source      = ! empty($this->resource) ? $this->resource : $this->image()->getPathname();
	$destination = $this->getResourcePath();

	$extent = ' ';
	if ($this->xAxis >= $this->width || $this->yAxis > $this->height)
	{
		$extent = ' -background transparent -extent ' . ($this->width ?? 0) . 'x' . ($this->height ?? 0) . ' ';
	}

	$action = ' -crop ' . ($this->width ?? 0) . 'x' . ($this->height ?? 0) . '+' . ($this->xAxis ?? 0) . '+' . ($this->yAxis ?? 0) . $extent . escapeshellarg($source) . ' ' . escapeshellarg($destination);

	$this->process($action);

	return $this;
}
```

</details>


<hr>

#### _rotate()

```php
protected function _rotate(int $angle)
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
<td>$this
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 13 lines (155 - 167)</small></summary>

```php
protected function _rotate(int $angle)
{
	$angle = '-rotate ' . $angle;

	$source      = ! empty($this->resource) ? $this->resource : $this->image()->getPathname();
	$destination = $this->getResourcePath();

	$action = ' ' . $angle . ' ' . escapeshellarg($source) . ' ' . escapeshellarg($destination);

	$this->process($action);

	return $this;
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 13 lines (181 - 193)</small></summary>

```php
public function _flatten(int $red = 255, int $green = 255, int $blue = 255)
{
	$flatten = "-background 'rgb({$red},{$green},{$blue})' -flatten";

	$source      = ! empty($this->resource) ? $this->resource : $this->image()->getPathname();
	$destination = $this->getResourcePath();

	$action = ' ' . $flatten . ' ' . escapeshellarg($source) . ' ' . escapeshellarg($destination);

	$this->process($action);

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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 13 lines (205 - 217)</small></summary>

```php
public function _flip(string $direction)
{
	$angle = $direction === 'horizontal' ? '-flop' : '-flip';

	$source      = ! empty($this->resource) ? $this->resource : $this->image()->getPathname();
	$destination = $this->getResourcePath();

	$action = ' ' . $angle . ' ' . escapeshellarg($source) . ' ' . escapeshellarg($destination);

	$this->process($action);

	return $this;
}
```

</details>


<hr>

#### getVersion()

```php
public function getVersion() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get driver version
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
<summary><small>Source: 9 lines (226 - 234)</small></summary>

```php
public function getVersion(): string
{
	$result = $this->process('-version');

	// The first line has the version in it...
	preg_match('/(ImageMagick\s[\S]+)/', $result[0], $matches);

	return str_replace('ImageMagick ', '', $matches[0]);
}
```

</details>


<hr>

#### process()

```php
protected function process(string $action, int $quality = 100) : array
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
<td>array
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 36 lines (247 - 282)</small></summary>

```php
protected function process(string $action, int $quality = 100): array
{
	// Do we have a vaild library path?
	if (empty($this->config->libraryPath))
	{
		throw ImageException::forInvalidImageLibraryPath($this->config->libraryPath);
	}

	if ($action !== '-version')
	{
		$this->supportedFormatCheck();
	}

	if (! preg_match('/convert$/i', $this->config->libraryPath))
	{
		$this->config->libraryPath = rtrim($this->config->libraryPath, '/') . '/convert';
	}

	$cmd  = $this->config->libraryPath;
	$cmd .= $action === '-version' ? ' ' . $action : ' -quality ' . $quality . ' ' . $action;

	$retval = 1;
	// exec() might be disabled
	if (function_usable('exec'))
	{
		@exec($cmd, $output, $retval);
	}

	// Did it work?
	if ($retval > 0)
	{
		throw ImageException::forImageProcessFailed();
	}

	return $output;
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
<summary><small>Source: 32 lines (300 - 331)</small></summary>

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

	// Copy the file through ImageMagick so that it has
	// a chance to convert file format.
	$action = escapeshellarg($this->resource) . ' ' . escapeshellarg($target);

	$result = $this->process($action, $quality);

	unlink($this->resource);

	return true;
}
```

</details>


<hr>

#### getResourcePath()

```php
protected function getResourcePath()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get Image Resource
</td></tr>
</table>

<table>
<tr><td>
This simply creates an image resource handle
based on the type of image being processed.
Since ImageMagick is used on the cli, we need to
ensure we have a temporary file on the server
that we can use.

To ensure we can use all features, like transparency,
during the process, we'll use a PNG as the temp file type.
</td></tr>
</table>

</details>



<table style="text-align:left">
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
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 16 lines (350 - 365)</small></summary>

```php
protected function getResourcePath()
{
	if (! is_null($this->resource))
	{
		return $this->resource;
	}

	$this->resource = WRITEPATH . 'cache/' . time() . '_' . bin2hex(random_bytes(10)) . '.png';

	$name = basename($this->resource);
	$path = pathinfo($this->resource, PATHINFO_DIRNAME);

	$this->image()->copy($path, $name);

	return $this->resource;
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







<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 6 lines (374 - 379)</small></summary>

```php
protected function ensureResource()
{
	$this->getResourcePath();

	$this->supportedFormatCheck();
}
```

</details>


<hr>

#### supportedFormatCheck()

```php
protected function supportedFormatCheck()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Check if given image format is supported
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>







<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ImageException
</td>
</tr>
</table>



<details>
<summary><small>Source: 12 lines (386 - 397)</small></summary>

```php
protected function supportedFormatCheck()
{
	switch ($this->image()->imageType)
	{
		case IMAGETYPE_WEBP:
			if (! in_array('WEBP', \Imagick::queryFormats()))
			{
				throw ImageException::forInvalidImageCreate(lang('images.webpNotSupported'));
			}
			break;
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





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 92 lines (409 - 500)</small></summary>

```php
protected function _text(string $text, array $options = [])
{
	$cmd = '';

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

	// Font
	if (! empty($options['fontPath']))
	{
		$cmd .= " -font '{$options['fontPath']}'";
	}

	if (isset($options['hAlign']) && isset($options['vAlign']))
	{
		switch ($options['hAlign'])
		{
			case 'left':
				$xAxis   = $options['hOffset'] + $options['padding'];
				$yAxis   = $options['vOffset'] + $options['padding'];
				$gravity = $options['vAlign'] === 'top' ? 'NorthWest' : 'West';
				if ($options['vAlign'] === 'bottom')
				{
					$gravity = 'SouthWest';
					$yAxis   = $options['vOffset'] - $options['padding'];
				}
				break;
			case 'center':
				$xAxis   = $options['hOffset'] + $options['padding'];
				$yAxis   = $options['vOffset'] + $options['padding'];
				$gravity = $options['vAlign'] === 'top' ? 'North' : 'Center';
				if ($options['vAlign'] === 'bottom')
				{
					$yAxis   = $options['vOffset'] - $options['padding'];
					$gravity = 'South';
				}
				break;
			case 'right':
				$xAxis   = $options['hOffset'] - $options['padding'];
				$yAxis   = $options['vOffset'] + $options['padding'];
				$gravity = $options['vAlign'] === 'top' ? 'NorthEast' : 'East';
				if ($options['vAlign'] === 'bottom')
				{
					$gravity = 'SouthEast';
					$yAxis   = $options['vOffset'] - $options['padding'];
				}
				break;
		}

		$xAxis = $xAxis >= 0 ? '+' . $xAxis : $xAxis;
		$yAxis = $yAxis >= 0 ? '+' . $yAxis : $yAxis;

		$cmd .= " -gravity {$gravity} -geometry {$xAxis}{$yAxis}";
	}

	// Color
	if (isset($options['color']))
	{
		list($r, $g, $b) = sscanf("#{$options['color']}", '#%02x%02x%02x');

		$cmd .= " -fill 'rgba({$r},{$g},{$b},{$options['opacity']})'";
	}

	// Font Size - use points....
	if (isset($options['fontSize']))
	{
		$cmd .= " -pointsize {$options['fontSize']}";
	}

	// Text
	$cmd .= " -annotate 0 '{$text}'";

	$source      = ! empty($this->resource) ? $this->resource : $this->image()->getPathname();
	$destination = $this->getResourcePath();

	$cmd = " '{$source}' {$cmd} '{$destination}'";

	$this->process($cmd);
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
Return the width of an image.
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
<summary><small>Source: 4 lines (509 - 512)</small></summary>

```php
public function _getWidth()
{
	return imagesx(imagecreatefromstring(file_get_contents($this->resource)));
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
Return the height of an image.
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
<summary><small>Source: 4 lines (519 - 522)</small></summary>

```php
public function _getHeight()
{
	return imagesy(imagecreatefromstring(file_get_contents($this->resource)));
}
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
<summary><small>Source: 27 lines (536 - 562)</small></summary>

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
			return $this->rotate(90)
							->flip('horizontal');
		case 6:
			return $this->rotate(90);
		case 7:
			return $this->rotate(270)
							->flip('horizontal');
		case 8:
			return $this->rotate(270);
		default:
			return $this;
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Images/Handlers/ImageMagickHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Handlers/GDHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Images/Image.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:17**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>