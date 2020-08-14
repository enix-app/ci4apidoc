


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Images/ImageHandlerInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Image.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Language/Language.md">next</a></td>
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
<td>framework/system/Images/ImageHandlerInterface.php
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



 

 
## CodeIgniter\Images\ImageHandlerInterface

<table style="text-align:left">
<tr><th>Interface</th><td>ImageHandlerInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Images\ImageHandlerInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Expected behavior of an Image handler
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
<th><a href="#reorient"><strong>reorient</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Reads the EXIF information from the image and modifies the orientation
so that displays correctly in the browser.</td>
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
<th><a href="#flip"><strong>flip</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Flip an image horizontally or vertically</td>
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
<th><a href="#text"><strong>text</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Overlays a string of text over the image.</td>
</tr>
<tr>
<th><a href="#save"><strong>save</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Saves any changes that have been made to file.</td>
</tr>

</table>






### Methods


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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: line 58</small></summary>

```php
public function resize(int $width, int $height, bool $maintainRatio = false, string $masterDim = 'auto');
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
<summary><small>Source: line 76</small></summary>

```php
public function crop(int $width = null, int $height = null, int $x = null, int $y = null, bool $maintainRatio = false, string $masterDim = 'auto');
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
<td>A PHP imagetype constant, e.g. <a href="https://www.php.net/manual/en/function.image-type-to-mime-type.php">https://www.php.net/manual/en/function.image-type-to-mime-type.php</a></td>
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
<summary><small>Source: line 88</small></summary>

```php
public function convert(int $imageType);
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
<summary><small>Source: line 99</small></summary>

```php
public function rotate(float $angle);
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
<summary><small>Source: line 112</small></summary>

```php
public function flatten(int $red = 255, int $green = 255, int $blue = 255);
```

</details>


<hr>

#### reorient()

```php
public function reorient()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reads the EXIF information from the image and modifies the orientation
so that displays correctly in the browser.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\ImageHandlerInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 122</small></summary>

```php
public function reorient();
```

</details>


<hr>

#### getEXIF()

```php
public function getEXIF(string $key = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve the EXIF information from the image, if possible. Returns
an array of the information, or null if nothing can be found.
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
<summary><small>Source: line 134</small></summary>

```php
public function getEXIF(string $key = null);
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
Flip an image horizontally or vertically
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
<td>Direction to flip, either 'vertical' or 'horizontal'</td>
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
<summary><small>Source: line 145</small></summary>

```php
public function flip(string $dir = 'vertical');
```

</details>


<hr>

#### fit()

```php
public function fit(int $width, int $height, string $position)
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
<summary><small>Source: line 169</small></summary>

```php
public function fit(int $width, int $height, string $position);
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
<summary><small>Source: line 193</small></summary>

```php
public function text(string $text, array $options = []);
```

</details>


<hr>

#### save()

```php
public function save(string $target = null, int $quality = 90)
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: line 209</small></summary>

```php
public function save(string $target = null, int $quality = 90);
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Images/ImageHandlerInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Images/Image.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Language/Language.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>