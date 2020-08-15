


 



<table>
<tr>
<td style="width:100%"><em>framework/system/RESTful/ResourcePresenter.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/RESTful/ResourceController.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RedirectException.md">next</a></td>
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
<td>framework/system/RESTful/ResourcePresenter.php
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



 
## CodeIgniter\RESTful\ResourcePresenter

<table style="text-align:left">
<tr><th>Class</th><td>ResourcePresenter</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\RESTful\ResourcePresenter</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Controller.md">CodeIgniter\Controller</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
An extendable controller to help provide a UI for a resource.
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
<td>Present a view of resource objects</td>
</tr>
<tr>
<th><a href="#show"><strong>show</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Present a view to present a specific resource object</td>
</tr>
<tr>
<th><a href="#new"><strong>new</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Present a view to present a new single resource object</td>
</tr>
<tr>
<th><a href="#create"><strong>create</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Process the creation/insertion of a new resource object.</td>
</tr>
<tr>
<th><a href="#remove"><strong>remove</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Present a view to confirm the deletion of a specific resource object</td>
</tr>
<tr>
<th><a href="#delete"><strong>delete</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Process the deletion of a specific resource object</td>
</tr>
<tr>
<th><a href="#edit"><strong>edit</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Present a view to edit the properties of a specific resource object</td>
</tr>
<tr>
<th><a href="#update"><strong>update</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Process the updating, full or partial, of a specific resource object.</td>
</tr>
<tr>
<th><a href="#setModel"><strong>setModel</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set or change the model this controller is bound to.</td>
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
<summary><small>Source: 7 lines (68 - 74)</small></summary>

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
Present a view of resource objects
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
<summary><small>Source: 4 lines (83 - 86)</small></summary>

```php
public function index()
{
	return lang('RESTful.notImplemented', ['index']);
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
Present a view to present a specific resource object
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
<td><code>$id</code></td>
<td><em>\type
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
<summary><small>Source: 4 lines (94 - 97)</small></summary>

```php
public function show($id = null)
{
	return lang('RESTful.notImplemented', ['show']);
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
Present a view to present a new single resource object
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
<summary><small>Source: 4 lines (104 - 107)</small></summary>

```php
public function new()
{
	return lang('RESTful.notImplemented', ['new']);
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
Process the creation/insertion of a new resource object.
</td></tr>
</table>

<table>
<tr><td>
This should be a POST.
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
<summary><small>Source: 4 lines (115 - 118)</small></summary>

```php
public function create()
{
	return lang('RESTful.notImplemented', ['create']);
}
```

</details>


<hr>

#### remove()

```php
public function remove($id = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Present a view to confirm the deletion of a specific resource object
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
<td><code>$id</code></td>
<td><em>\type
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
<summary><small>Source: 4 lines (126 - 129)</small></summary>

```php
public function remove($id = null)
{
	return lang('RESTful.notImplemented', ['remove']);
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
Process the deletion of a specific resource object
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
<td><code>$id</code></td>
<td><em>\type
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
<summary><small>Source: 4 lines (137 - 140)</small></summary>

```php
public function delete($id = null)
{
	return lang('RESTful.notImplemented', ['delete']);
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
Present a view to edit the properties of a specific resource object
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
<td><code>$id</code></td>
<td><em>\type
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
<summary><small>Source: 4 lines (148 - 151)</small></summary>

```php
public function edit($id = null)
{
	return lang('RESTful.notImplemented', ['edit']);
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
Process the updating, full or partial, of a specific resource object.
</td></tr>
</table>

<table>
<tr><td>
This should be a POST.
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
<td><code>$id</code></td>
<td><em>\type
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
<summary><small>Source: 4 lines (160 - 163)</small></summary>

```php
public function update($id = null)
{
	return lang('RESTful.notImplemented', ['update']);
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
<summary><small>Source: 32 lines (173 - 204)</small></summary>

```php
public function setModel($which = null)
{
	// save what we have been given
	if (! empty($which))
	{
		if (is_object($which))
		{
			$this->model     = $which;
			$this->modelName = null;
		}
		else
		{
			$this->model     = null;
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

<table>
<tr>
<td style="width:100%"><em>framework/system/RESTful/ResourcePresenter.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/RESTful/ResourceController.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Router/Exceptions/RedirectException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:18**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>