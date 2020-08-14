


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Log/Handlers/HandlerInterface.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/FileHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Logger.md">next</a></td>
</tr>
</table>







# CodeIgniter\Log\Handlers 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Log\Handlers</td></tr>
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
<td>framework/system/Log/Handlers/HandlerInterface.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/BaseHandler.md">CodeIgniter\Log\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/ChromeLoggerHandler.md">CodeIgniter\Log\Handlers\ChromeLoggerHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/FileHandler.md">CodeIgniter\Log\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/HandlerInterface.md">CodeIgniter\Log\Handlers\HandlerInterface</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Log\Handlers\HandlerInterface

<table style="text-align:left">
<tr><th>Interface</th><td>HandlerInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Log\Handlers\HandlerInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Expected behavior for a Log handler
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
<th><a href="#handle"><strong>handle</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Handles logging the message.</td>
</tr>
<tr>
<th><a href="#canHandle"><strong>canHandle</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks whether the Handler will handle logging items of this
log Level.</td>
</tr>
<tr>
<th><a href="#setDateFormat"><strong>setDateFormat</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the preferred date format to use when logging.</td>
</tr>

</table>






### Methods


<hr>

#### handle()

```php
public function handle($level, $message) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Handles logging the message.
</td></tr>
</table>

<table>
<tr><td>
If the handler returns false, then execution of handlers
will stop. Any handlers that have not run, yet, will not
be run.
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
<td><code>$level</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$message</code></td>
<td><em>
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
<summary><small>Source: line 59</small></summary>

```php
public function handle($level, $message): bool;
```

</details>


<hr>

#### canHandle()

```php
public function canHandle(string $level) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks whether the Handler will handle logging items of this
log Level.
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
<td><code>$level</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: line 71</small></summary>

```php
public function canHandle(string $level): bool;
```

</details>


<hr>

#### setDateFormat()

```php
public function setDateFormat(string $format)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the preferred date format to use when logging.
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



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\HandlerInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 82</small></summary>

```php
public function setDateFormat(string $format);
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Log/Handlers/HandlerInterface.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Handlers/FileHandler.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Log/Logger.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>