


 



<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Files/UploadedFileInterface.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFile.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Header.md">next</a></td>
</tr>
</table>







# CodeIgniter\HTTP\Files 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\HTTP\Files</td></tr>
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
<td>framework/system/HTTP/Files/UploadedFileInterface.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/FileCollection.md">CodeIgniter\HTTP\Files\FileCollection</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFile.md">CodeIgniter\HTTP\Files\UploadedFile</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFileInterface.md">CodeIgniter\HTTP\Files\UploadedFileInterface</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\HTTP\Files\UploadedFileInterface

<table style="text-align:left">
<tr><th>Interface</th><td>UploadedFileInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\HTTP\Files\UploadedFileInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Value object representing a single file uploaded through an
HTTP request. Used by the IncomingRequest class to
provide files.
</td></tr>
</table>

<table>
<tr><td>
Typically, implementors will extend the SplFileInfo class.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\HTTP
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
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Accepts the file information as would be filled in from the $_FILES array.</td>
</tr>
<tr>
<th><a href="#move"><strong>move</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Move the uploaded file to a new location.</td>
</tr>
<tr>
<th><a href="#hasMoved"><strong>hasMoved</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns whether the file has been moved or not. If it has,
the move() method will not work and certain properties, like
the tempName, will no longer be available.</td>
</tr>
<tr>
<th><a href="#getError"><strong>getError</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve the error associated with the uploaded file.</td>
</tr>
<tr>
<th><a href="#getName"><strong>getName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve the filename sent by the client.</td>
</tr>
<tr>
<th><a href="#getTempName"><strong>getTempName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Gets the temporary filename where the file was uploaded to.</td>
</tr>
<tr>
<th><a href="#getClientExtension"><strong>getClientExtension</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the original file extension, based on the file name that
was uploaded. This is NOT a trusted source.</td>
</tr>
<tr>
<th><a href="#getClientMimeType"><strong>getClientMimeType</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the mime type as provided by the client.</td>
</tr>
<tr>
<th><a href="#isValid"><strong>isValid</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns whether the file was uploaded successfully, based on whether
it was uploaded via HTTP and has no errors.</td>
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






### Methods


<hr>

#### __construct()

```php
public function __construct(string $path, string $originalName, string $mimeType = null, int $size = null, int $error = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Accepts the file information as would be filled in from the $_FILES array.
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
<td>The temporary location of the uploaded file.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$originalName</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The client-provided filename.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$mimeType</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The type of file as provided by PHP</td>
</tr>

<tr>
<td>4.</td>
<td><code>$size</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The size of the file, in bytes</td>
</tr>

<tr>
<td>5.</td>
<td><code>$error</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The error constant of the upload (one of PHP's UPLOADERRXXX constants)</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: line 63</small></summary>

```php
public function __construct(string $path, string $originalName, string $mimeType = null, int $size = null, int $error = null);
```

</details>


<hr>

#### move()

```php
public function move(string $targetPath, string $name = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Move the uploaded file to a new location.
</td></tr>
</table>

<table>
<tr><td>
$targetPath may be an absolute path, or a relative path. If it is a
relative path, resolution should be the same as used by PHP's rename()
function.

The original file MUST be removed on completion.

If this method is called more than once, any subsequent calls MUST raise
an exception.

When used in an SAPI environment where $_FILES is populated, when writing
files via moveTo(), is_uploaded_file() and move_uploaded_file() SHOULD be
used to ensure permissions and upload status are verified correctly.

If you wish to move to a stream, use getStream(), as SAPI operations
cannot guarantee writing to stream destinations.
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
<td>Path to which to move the uploaded file.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the name to rename the file to.</td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\InvalidArgumentException
</td>
</tr>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\RuntimeException
</td>
</tr>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\RuntimeException
</td>
</tr>
</table>



<details>
<summary><small>Source: line 96</small></summary>

```php
public function move(string $targetPath, string $name = null);
```

</details>


<hr>

#### hasMoved()

```php
public function hasMoved() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns whether the file has been moved or not. If it has,
the move() method will not work and certain properties, like
the tempName, will no longer be available.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: line 107</small></summary>

```php
public function hasMoved(): bool;
```

</details>


<hr>

#### getError()

```php
public function getError() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve the error associated with the uploaded file.
</td></tr>
</table>

<table>
<tr><td>
The return value MUST be one of PHP's UPLOAD_ERR_XXX constants.

If the file was uploaded successfully, this method MUST return
UPLOAD_ERR_OK.

Implementations SHOULD return the value stored in the "error" key of
the file in the $_FILES array.
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
<summary><small>Source: line 125</small></summary>

```php
public function getError(): int;
```

</details>


<hr>

#### getName()

```php
public function getName() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Retrieve the filename sent by the client.
</td></tr>
</table>

<table>
<tr><td>
Do not trust the value returned by this method. A client could send
a malicious filename with the intention to corrupt or hack your
application.

Implementations SHOULD return the value stored in the "name" key of
the file in the $_FILES array.
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
<summary><small>Source: line 142</small></summary>

```php
public function getName(): string;
```

</details>


<hr>

#### getTempName()

```php
public function getTempName() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets the temporary filename where the file was uploaded to.
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
<summary><small>Source: line 151</small></summary>

```php
public function getTempName(): string;
```

</details>


<hr>

#### getClientExtension()

```php
public function getClientExtension() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the original file extension, based on the file name that
was uploaded. This is NOT a trusted source.
</td></tr>
</table>

<table>
<tr><td>
For a trusted version, use guessExtension() instead.
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
<summary><small>Source: line 162</small></summary>

```php
public function getClientExtension(): string;
```

</details>


<hr>

#### getClientMimeType()

```php
public function getClientMimeType() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the mime type as provided by the client.
</td></tr>
</table>

<table>
<tr><td>
This is NOT a trusted value.
For a trusted version, use getMimeType() instead.
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
<summary><small>Source: line 173</small></summary>

```php
public function getClientMimeType(): string;
```

</details>


<hr>

#### isValid()

```php
public function isValid() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns whether the file was uploaded successfully, based on whether
it was uploaded via HTTP and has no errors.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: line 183</small></summary>

```php
public function isValid(): bool;
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
<summary><small>Source: line 200</small></summary>

```php
public function getDestination(string $destination, string $delimiter = '_', int $i = 0): string;
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Files/UploadedFileInterface.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFile.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Header.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>