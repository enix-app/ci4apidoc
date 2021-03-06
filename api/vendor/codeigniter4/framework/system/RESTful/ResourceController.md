


 



<table>
<tr>
<td style="width:100%"><em>framework/system/RESTful/ResourceController.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerRenderer.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/RESTful/ResourcePresenter.md">next</a></td>
</tr>
</table>







# CodeIgniter\RESTful 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\RESTful</td></tr>
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
<td>framework/system/RESTful/ResourceController.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/RESTful/ResourceController.md">CodeIgniter\RESTful\ResourceController</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/RESTful/ResourcePresenter.md">CodeIgniter\RESTful\ResourcePresenter</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/API/ResponseTrait.md"><strong>CodeIgniter\API\ResponseTrait</strong></a>
</td>
<td>ResponseTrait</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Controller.md"><strong>CodeIgniter\Controller</strong></a>
</td>
<td>Controller</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md"><strong>CodeIgniter\HTTP\RequestInterface</strong></a>
</td>
<td>RequestInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/ResponseInterface.md"><strong>CodeIgniter\HTTP\ResponseInterface</strong></a>
</td>
<td>ResponseInterface</td>
</tr>
<tr>
<td>
<strong>Psr\Log\LoggerInterface</strong>
</td>
<td>LoggerInterface</td>
</tr>
</table>



 
## CodeIgniter\RESTful\ResourceController

<table style="text-align:left">
<tr><th>Class</th><td>ResourceController</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\RESTful\ResourceController</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Controller.md">CodeIgniter\Controller</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
An extendable controller to provide a RESTful API for a resource.
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\RESTful
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
<th><a href="#modelName"><strong>modelName</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#model"><strong>model</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>

<tr>
<th><a href="#initController"><strong>initController</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#index"><strong>index</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return an array of resource objects, themselves in array format</td>
</tr>
<tr>
<th><a href="#show"><strong>show</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the properties of a resource object</td>
</tr>
<tr>
<th><a href="#new"><strong>new</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return a new resource object, with default properties</td>
</tr>
<tr>
<th><a href="#create"><strong>create</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Create a new resource object, from &quot;posted&quot; parameters</td>
</tr>
<tr>
<th><a href="#edit"><strong>edit</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the editable properties of a resource object</td>
</tr>
<tr>
<th><a href="#update"><strong>update</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Add or update a model resource, from &quot;posted&quot; properties</td>
</tr>
<tr>
<th><a href="#delete"><strong>delete</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Delete the designated resource object from the model</td>
</tr>
<tr>
<th><a href="#setModel"><strong>setModel</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set or change the model this controller is bound to.</td>
</tr>
<tr>
<th><a href="#setFormat"><strong>setFormat</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set/change the expected response representation for returned objects</td>
</tr>

</table>





### Properties


<hr>

#### $modelName

```php
protected $modelName;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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

#### $model

```php
protected $model;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Model
</td>
</tr>
</table>







### Methods


<hr>

#### initController()

```php
public function initController(RequestInterface $request, ResponseInterface $response, LoggerInterface $logger)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td><em>RequestInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$response</code></td>
<td><em>ResponseInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$logger</code></td>
<td><em>LoggerInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 7 lines (71 - 77)</small></summary>

```php
public function initController(RequestInterface $request, ResponseInterface $response, LoggerInterface $logger)
{
	parent::initController($request, $response, $logger);

	// instantiate our model, if needed
	$this->setModel($this->modelName);
}
```

</details>


<hr>

#### index()

```php
public function index()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return an array of resource objects, themselves in array format
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (86 - 89)</small></summary>

```php
public function index()
{
	return $this->fail(lang('RESTful.notImplemented', ['index']), 501);
}
```

</details>


<hr>

#### show()

```php
public function show($id = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the properties of a resource object
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (96 - 99)</small></summary>

```php
public function show($id = null)
{
	return $this->fail(lang('RESTful.notImplemented', ['show']), 501);
}
```

</details>


<hr>

#### new()

```php
public function new()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return a new resource object, with default properties
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (106 - 109)</small></summary>

```php
public function new()
{
	return $this->fail(lang('RESTful.notImplemented', ['new']), 501);
}
```

</details>


<hr>

#### create()

```php
public function create()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Create a new resource object, from "posted" parameters
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (116 - 119)</small></summary>

```php
public function create()
{
	return $this->fail(lang('RESTful.notImplemented', ['create']), 501);
}
```

</details>


<hr>

#### edit()

```php
public function edit($id = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the editable properties of a resource object
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (126 - 129)</small></summary>

```php
public function edit($id = null)
{
	return $this->fail(lang('RESTful.notImplemented', ['edit']), 501);
}
```

</details>


<hr>

#### update()

```php
public function update($id = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add or update a model resource, from "posted" properties
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (136 - 139)</small></summary>

```php
public function update($id = null)
{
	return $this->fail(lang('RESTful.notImplemented', ['update']), 501);
}
```

</details>


<hr>

#### delete()

```php
public function delete($id = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Delete the designated resource object from the model
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (146 - 149)</small></summary>

```php
public function delete($id = null)
{
	return $this->fail(lang('RESTful.notImplemented', ['delete']), 501);
}
```

</details>


<hr>

#### setModel()

```php
public function setModel($which = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set or change the model this controller is bound to.
</td></tr>
</table>

<table>
<tr><td>
Given either the name or the object, determine the other.
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
<td><code>$which</code></td>
<td><em>string<br>object
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 30 lines (159 - 188)</small></summary>

```php
public function setModel($which = null)
{
	// save what we have been given
	if (! empty($which))
	{
		if (is_object($which))
		{
			$this->model = $which;
		}
		else
		{
			$this->modelName = $which;
		}
	}

	// make a model object if needed
	if (empty($this->model) && ! empty($this->modelName))
	{
		if (class_exists($this->modelName))
		{
			$this->model = model($this->modelName);
		}
	}

	// determine model name if needed
	if (empty($this->modelName) && ! empty($this->model))
	{
		$this->modelName = get_class($this->model);
	}
}
```

</details>


<hr>

#### setFormat()

```php
public function setFormat(string $format = 'json')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set/change the expected response representation for returned objects
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
<td><code>$format</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 7 lines (195 - 201)</small></summary>

```php
public function setFormat(string $format = 'json')
{
	if (in_array($format, ['json', 'xml']))
	{
		$this->format = $format;
	}
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/RESTful/ResourceController.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Pager/PagerRenderer.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/RESTful/ResourcePresenter.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:18**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>