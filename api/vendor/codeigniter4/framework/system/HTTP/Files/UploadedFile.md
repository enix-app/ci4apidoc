


 



<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Files/UploadedFile.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/FileCollection.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFileInterface.md">next</a></td>
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
<td>framework/system/HTTP/Files/UploadedFile.php
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



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/File.md"><strong>CodeIgniter\Files\File</strong></a>
</td>
<td>File</td>
</tr>
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Exceptions/HTTPException.md"><strong>CodeIgniter\HTTP\Exceptions\HTTPException</strong></a>
</td>
<td>HTTPException</td>
</tr>
<tr>
<td>
<strong>Config\Mimes</strong>
</td>
<td>Mimes</td>
</tr>
<tr>
<td>
<strong>Exception</strong>
</td>
<td>Exception</td>
</tr>
</table>



 
## CodeIgniter\HTTP\Files\UploadedFile

<table style="text-align:left">
<tr><th>Class</th><td>UploadedFile</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\HTTP\Files\UploadedFile</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Files/File.md">CodeIgniter\Files\File</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFileInterface.md">CodeIgniter\HTTP\Files\UploadedFileInterface</a><br>
</td>
</tr>
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
<th><a href="#path"><strong>path</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The path to the temporary file.</td>
</tr>
<tr>
<th><a href="#originalName"><strong>originalName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The original filename as provided by the client.</td>
</tr>
<tr>
<th><a href="#name"><strong>name</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The filename given to a file during a move.</td>
</tr>
<tr>
<th><a href="#originalMimeType"><strong>originalMimeType</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The type of file as provided by PHP</td>
</tr>
<tr>
<th><a href="#error"><strong>error</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The error constant of the upload
(one of PHP&#039;s UPLOADERRXXX constants)</td>
</tr>
<tr>
<th><a href="#hasMoved"><strong>hasMoved</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether the file has been moved already or not.</td>
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
<th><a href="#setPath"><strong>setPath</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>create file target path if
the set path does not exist</td>
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
<th><a href="#getErrorString"><strong>getErrorString</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get error string</td>
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
<th><a href="#getName"><strong>getName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Retrieve the filename. This will typically be the filename sent
by the client, and should not be trusted. If the file has been
moved, this will return the final name of the moved file.</td>
</tr>
<tr>
<th><a href="#getClientName"><strong>getClientName</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the name of the file as provided by the client during upload.</td>
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
<th><a href="#getExtension"><strong>getExtension</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Overrides SPLFileInfo&#039;s to work with uploaded files, since
the temp file that&#039;s been uploaded doesn&#039;t have an extension.</td>
</tr>
<tr>
<th><a href="#guessExtension"><strong>guessExtension</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attempts to determine the best file extension.</td>
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
<th><a href="#isValid"><strong>isValid</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns whether the file was uploaded successfully, based on whether
it was uploaded via HTTP and has no errors.</td>
</tr>
<tr>
<th><a href="#store"><strong>store</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Save the uploaded file to a new location.</td>
</tr>

</table>





### Properties


<hr>

#### $path

```php
protected $path;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The path to the temporary file.
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

#### $originalName

```php
protected $originalName;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The original filename as provided by the client.
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

#### $name

```php
protected $name;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The filename given to a file during a move.
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

#### $originalMimeType

```php
protected $originalMimeType;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The type of file as provided by PHP
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

#### $error

```php
protected $error;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The error constant of the upload
(one of PHP's UPLOADERRXXX constants)
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

#### $hasMoved

```php
protected $hasMoved = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether the file has been moved already or not.
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
<summary><small>Source: 11 lines (114 - 124)</small></summary>

```php
public function __construct(string $path, string $originalName, string $mimeType = null, int $size = null, int $error = null)
{
	$this->path             = $path;
	$this->name             = $originalName;
	$this->originalName     = $originalName;
	$this->originalMimeType = $mimeType;
	$this->size             = $size;
	$this->error            = $error;

	parent::__construct($path, false);
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

<tr>
<td>3.</td>
<td><code>$overwrite</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>State for indicating whether to overwrite the previously generated file with the same
name or not.</td>
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
<summary><small>Source: 38 lines (161 - 198)</small></summary>

```php
public function move(string $targetPath, string $name = null, bool $overwrite = false)
{
	$targetPath = $this->setPath($targetPath); //set the target path

	if ($this->hasMoved)
	{
		throw HTTPException::forAlreadyMoved();
	}

	if (! $this->isValid())
	{
		throw HTTPException::forInvalidFile();
	}

	$targetPath  = rtrim($targetPath, '/') . '/';
	$name        = is_null($name) ? $this->getName() : $name;
	$destination = $overwrite ? $targetPath . $name : $this->getDestination($targetPath . $name);

	try
	{
		move_uploaded_file($this->path, $destination);
	}
	catch (Exception $e)
	{
		$error   = error_get_last();
		$message = isset($error['message']) ? strip_tags($error['message']) : '';
		throw HTTPException::forMoveFailed(basename($this->path), $targetPath, $message);
	}

	@chmod($targetPath, 0777 & ~umask());

	// Success, so store our new information
	$this->path     = $targetPath;
	$this->name     = basename($destination);
	$this->hasMoved = true;

	return true;
}
```

</details>


<hr>

#### setPath()

```php
protected function setPath(string $path) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
create file target path if
the set path does not exist
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (208 - 221)</small></summary>

```php
protected function setPath(string $path): string
{
	if (! is_dir($path))
	{
		mkdir($path, 0777, true);
		//create the index.html file
		if (! is_file($path . 'index.html'))
		{
			$file = fopen($path . 'index.html', 'x+');
			fclose($file);
		}
	}
	return $path;
}
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
<summary><small>Source: 4 lines (232 - 235)</small></summary>

```php
public function hasMoved(): bool
{
	return $this->hasMoved;
}
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
<summary><small>Source: 9 lines (253 - 261)</small></summary>

```php
public function getError(): int
{
	if (is_null($this->error))
	{
		return UPLOAD_ERR_OK;
	}

	return $this->error;
}
```

</details>


<hr>

#### getErrorString()

```php
public function getErrorString() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get error string
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
<summary><small>Source: 17 lines (270 - 286)</small></summary>

```php
public function getErrorString(): string
{
	$errors = [
		UPLOAD_ERR_OK         => lang('HTTP.uploadErrOk'),
		UPLOAD_ERR_INI_SIZE   => lang('HTTP.uploadErrIniSize'),
		UPLOAD_ERR_FORM_SIZE  => lang('HTTP.uploadErrFormSize'),
		UPLOAD_ERR_PARTIAL    => lang('HTTP.uploadErrPartial'),
		UPLOAD_ERR_NO_FILE    => lang('HTTP.uploadErrNoFile'),
		UPLOAD_ERR_CANT_WRITE => lang('HTTP.uploadErrCantWrite'),
		UPLOAD_ERR_NO_TMP_DIR => lang('HTTP.uploadErrNoTmpDir'),
		UPLOAD_ERR_EXTENSION  => lang('HTTP.uploadErrExtension'),
	];

	$error = is_null($this->error) ? UPLOAD_ERR_OK : $this->error;

	return sprintf($errors[$error] ?? lang('HTTP.uploadErrUnknown'), $this->getName());
}
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (297 - 300)</small></summary>

```php
public function getClientMimeType(): string
{
	return $this->originalMimeType;
}
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
Retrieve the filename. This will typically be the filename sent
by the client, and should not be trusted. If the file has been
moved, this will return the final name of the moved file.
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
<summary><small>Source: 4 lines (311 - 314)</small></summary>

```php
public function getName(): string
{
	return $this->name;
}
```

</details>


<hr>

#### getClientName()

```php
public function getClientName() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the name of the file as provided by the client during upload.
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
<summary><small>Source: 4 lines (323 - 326)</small></summary>

```php
public function getClientName(): string
{
	return $this->originalName;
}
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
<summary><small>Source: 4 lines (335 - 338)</small></summary>

```php
public function getTempName(): string
{
	return $this->path;
}
```

</details>


<hr>

#### getExtension()

```php
public function getExtension() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Overrides SPLFileInfo's to work with uploaded files, since
the temp file that's been uploaded doesn't have an extension.
</td></tr>
</table>

<table>
<tr><td>
Is simply an alias for guessExtension for a safer method
than simply relying on the provided extension.
Additionally it will return clientExtension in case if there are
other extensions with the same mime type.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (351 - 354)</small></summary>

```php
public function getExtension(): string
{
	return $this->guessExtension();
}
```

</details>


<hr>

#### guessExtension()

```php
public function guessExtension() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to determine the best file extension.
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
<summary><small>Source: 4 lines (361 - 364)</small></summary>

```php
public function guessExtension(): string
{
	return Mimes::guessExtensionFromType($this->getClientMimeType(), $this->getClientExtension()) ?? $this->getClientExtension();
}
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (375 - 378)</small></summary>

```php
public function getClientExtension(): string
{
	return pathinfo($this->originalName, PATHINFO_EXTENSION) ?? '';
}
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
<summary><small>Source: 4 lines (388 - 391)</small></summary>

```php
public function isValid(): bool
{
	return is_uploaded_file($this->path) && $this->error === UPLOAD_ERR_OK;
}
```

</details>


<hr>

#### store()

```php
public function store(string $folderName = null, string $fileName = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Save the uploaded file to a new location.
</td></tr>
</table>

<table>
<tr><td>
By default, upload files are saved in writable/uploads directory. The YYYYMMDD folder
and random file name will be created.
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
<td><code>$folderName</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the folder name to writable/uploads directory.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$fileName</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the name to rename the file to.</td>
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
<summary><small>Source: 9 lines (403 - 411)</small></summary>

```php
public function store(string $folderName = null, string $fileName = null): string
{
	$folderName = rtrim($folderName ?? date('Ymd'), '/') . '/' ;
	$fileName   = $fileName ?? $this->getRandomName();

	// Move the uploaded file to a new location.
	return ($this->move(WRITEPATH . 'uploads/' . $folderName, $fileName)) ?
			$folderName . $this->name : null;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Files/UploadedFile.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/FileCollection.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFileInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>