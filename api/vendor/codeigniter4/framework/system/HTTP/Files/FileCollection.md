


 



<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Files/FileCollection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Exceptions/HTTPException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFile.md">next</a></td>
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
<td>framework/system/HTTP/Files/FileCollection.php
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



 

 
## CodeIgniter\HTTP\Files\FileCollection

<table style="text-align:left">
<tr><th>Class</th><td>FileCollection</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\HTTP\Files\FileCollection</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class FileCollection
</td></tr>
</table>

<table>
<tr><td>
Provides easy access to uploaded files for a request.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\HTTP\Files
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
<th><a href="#files"><strong>files</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>An array of UploadedFile instances for any files
uploaded as part of this request.</td>
</tr>

<tr>
<th><a href="#all"><strong>all</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an array of all uploaded files that were found.</td>
</tr>
<tr>
<th><a href="#getFile"><strong>getFile</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Attempts to get a single file from the collection of uploaded files.</td>
</tr>
<tr>
<th><a href="#getFileMultiple"><strong>getFileMultiple</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Verify if a file exist in the collection of uploaded files and is have been uploaded with multiple option.</td>
</tr>
<tr>
<th><a href="#hasFile"><strong>hasFile</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks whether an uploaded file with name $fileID exists in
this request.</td>
</tr>
<tr>
<th><a href="#populateFiles"><strong>populateFiles</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Taking information from the $_FILES array, it creates an instance
of UploadedFile for each one, saving the results to this-&gt;files.</td>
</tr>
<tr>
<th><a href="#createFileObject"><strong>createFileObject</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Given a file array, will create UploadedFile instances. Will
loop over an array and create objects for each.</td>
</tr>
<tr>
<th><a href="#fixFilesArray"><strong>fixFilesArray</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Reformats the odd $_FILES array into something much more like
we would expect, with each object having its own array.</td>
</tr>
<tr>
<th><a href="#getValueDotNotationSyntax"><strong>getValueDotNotationSyntax</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Navigate through a array looking for a particular index</td>
</tr>

</table>





### Properties


<hr>

#### $files

```php
protected $files;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
An array of UploadedFile instances for any files
uploaded as part of this request.
</td></tr>
</table>

<table>
<tr><td>
Populated the first time either files(), file(), or hasFile()
is called.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array<br>null
</td>
</tr>
</table>







### Methods


<hr>

#### all()

```php
public function all()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array of all uploaded files that were found.
</td></tr>
</table>

<table>
<tr><td>
Each element in the array will be an instance of UploadedFile.
The key of each element will be the client filename.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (72 - 77)</small></summary>

```php
public function all()
{
	$this->populateFiles();

	return $this->files;
}
```

</details>


<hr>

#### getFile()

```php
public function getFile(string $name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to get a single file from the collection of uploaded files.
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


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\UploadedFile<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 24 lines (88 - 111)</small></summary>

```php
public function getFile(string $name)
{
	$this->populateFiles();

	if ($this->hasFile($name))
	{
		if (strpos($name, '.') !== false)
		{
			$name         = explode('.', $name);
			$uploadedFile = $this->getValueDotNotationSyntax($name, $this->files);
			return ($uploadedFile instanceof UploadedFile) ?
				 $uploadedFile : null;
		}

		if (array_key_exists($name, $this->files))
		{
			$uploadedFile = $this->files[$name];
			return  ($uploadedFile instanceof UploadedFile) ?
				$uploadedFile : null;
		}
	}

	return null;
}
```

</details>


<hr>

#### getFileMultiple()

```php
public function getFileMultiple(string $name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Verify if a file exist in the collection of uploaded files and is have been uploaded with multiple option.
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


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 25 lines (122 - 146)</small></summary>

```php
public function getFileMultiple(string $name)
{
	$this->populateFiles();

	if ($this->hasFile($name))
	{
		if (strpos($name, '.') !== false)
		{
			$name         = explode('.', $name);
			$uploadedFile = $this->getValueDotNotationSyntax($name, $this->files);

			return (is_array($uploadedFile) && ($uploadedFile[0] instanceof UploadedFile)) ?
				$uploadedFile : null;
		}

		if (array_key_exists($name, $this->files))
		{
			$uploadedFile = $this->files[$name];
			return (is_array($uploadedFile) && ($uploadedFile[0] instanceof UploadedFile)) ?
				$uploadedFile : null;
		}
	}

	return null;
}
```

</details>


<hr>

#### hasFile()

```php
public function hasFile(string $fileID) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks whether an uploaded file with name $fileID exists in
this request.
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
<td><code>$fileID</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The name of the uploaded file (from the input)</td>
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
<summary><small>Source: 25 lines (158 - 182)</small></summary>

```php
public function hasFile(string $fileID): bool
{
	$this->populateFiles();

	if (strpos($fileID, '.') !== false)
	{
		$segments = explode('.', $fileID);

		$el = $this->files;

		foreach ($segments as $segment)
		{
			if (! array_key_exists($segment, $el))
			{
				return false;
			}

			$el = $el[$segment];
		}

		return true;
	}

	return isset($this->files[$fileID]);
}
```

</details>


<hr>

#### populateFiles()

```php
protected function populateFiles()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Taking information from the $_FILES array, it creates an instance
of UploadedFile for each one, saving the results to this->files.
</td></tr>
</table>

<table>
<tr><td>
Called by files(), file(), and hasFile()
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 21 lines (192 - 212)</small></summary>

```php
protected function populateFiles()
{
	if (is_array($this->files))
	{
		return;
	}

	$this->files = [];

	if (empty($_FILES))
	{
		return;
	}

	$files = $this->fixFilesArray($_FILES);

	foreach ($files as $name => $file)
	{
		$this->files[$name] = $this->createFileObject($file);
	}
}
```

</details>


<hr>

#### createFileObject()

```php
protected function createFileObject(array $array)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Given a file array, will create UploadedFile instances. Will
loop over an array and create objects for each.
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
<td><code>$array</code></td>
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
<td>array<br>\UploadedFile
</td>
</tr>
</table>





<details>
<summary><small>Source: 23 lines (224 - 246)</small></summary>

```php
protected function createFileObject(array $array)
{
	if (! isset($array['name']))
	{
		$output = [];

		foreach ($array as $key => $values)
		{
			if (! is_array($values))
			{
				continue;
			}

			$output[$key] = $this->createFileObject($values);
		}

		return $output;
	}

	return new UploadedFile(
			$array['tmp_name'] ?? null, $array['name'] ?? null, $array['type'] ?? null, $array['size'] ?? null, $array['error'] ?? null
	);
}
```

</details>


<hr>

#### fixFilesArray()

```php
protected function fixFilesArray(array $data) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reformats the odd $_FILES array into something much more like
we would expect, with each object having its own array.
</td></tr>
</table>

<table>
<tr><td>
Thanks to Jack Sleight on the PHP Manual page for the basis
of this method.
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
<summary><small>Source: 37 lines (263 - 299)</small></summary>

```php
protected function fixFilesArray(array $data): array
{
	$output = [];

	foreach ($data as $name => $array)
	{
		foreach ($array as $field => $value)
		{
			$pointer = &$output[$name];

			if (! is_array($value))
			{
				$pointer[$field] = $value;
				continue;
			}

			$stack    = [&$pointer];
			$iterator = new \RecursiveIteratorIterator(
					new \RecursiveArrayIterator($value), \RecursiveIteratorIterator::SELF_FIRST
			);

			foreach ($iterator as $key => $val)
			{
				array_splice($stack, $iterator->getDepth() + 1);
				$pointer = &$stack[count($stack) - 1];
				$pointer = &$pointer[$key];
				$stack[] = &$pointer;
				if (! $iterator->hasChildren())
				{
					$pointer[$field] = $val;
				}
			}
		}
	}

	return $output;
}
```

</details>


<hr>

#### getValueDotNotationSyntax()

```php
protected function getValueDotNotationSyntax(array $index, array $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Navigate through a array looking for a particular index
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
<td><code>$index</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>The index sequence we are navigating down</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>The portion of the array to process</td>
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
<summary><small>Source: 13 lines (311 - 323)</small></summary>

```php
protected function getValueDotNotationSyntax(array $index, array $value)
{
	if (! empty($index))
	{
		$current_index = array_shift($index);
	}
	if (is_array($index) && $index && is_array($value[$current_index]) && $value[$current_index])
	{
		return $this->getValueDotNotationSyntax($index, $value[$current_index]);
	}

	return (isset($value[$current_index])) ? $value[$current_index] : null;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/HTTP/Files/FileCollection.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Exceptions/HTTPException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/Files/UploadedFile.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:12**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>