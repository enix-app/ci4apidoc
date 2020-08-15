


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/ArrayHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Exceptions/SessionException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">next</a></td>
</tr>
</table>







# CodeIgniter\Session\Handlers 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Session\Handlers</td></tr>
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
<td>framework/system/Session/Handlers/ArrayHandler.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/ArrayHandler.md">CodeIgniter\Session\Handlers\ArrayHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">CodeIgniter\Session\Handlers\BaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/DatabaseHandler.md">CodeIgniter\Session\Handlers\DatabaseHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/FileHandler.md">CodeIgniter\Session\Handlers\FileHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/MemcachedHandler.md">CodeIgniter\Session\Handlers\MemcachedHandler</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/RedisHandler.md">CodeIgniter\Session\Handlers\RedisHandler</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>Config\Database</strong>
</td>
<td>Database</td>
</tr>
</table>



 
## CodeIgniter\Session\Handlers\ArrayHandler

<table style="text-align:left">
<tr><th>Class</th><td>ArrayHandler</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Session\Handlers\ArrayHandler</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">CodeIgniter\Session\Handlers\BaseHandler</a></td></tr>
<tr><th>Implements</th>
<td>
<a href="">CodeIgniter\Session\Handlers\SessionHandlerInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Session handler using static array for storage.
</td></tr>
</table>

<table>
<tr><td>
Intended only for use during testing.
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
<th><a href="#cache"><strong>cache</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td></td>
</tr>

<tr>
<th><a href="#open"><strong>open</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Open</td>
</tr>
<tr>
<th><a href="#read"><strong>read</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Read</td>
</tr>
<tr>
<th><a href="#write"><strong>write</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Write</td>
</tr>
<tr>
<th><a href="#close"><strong>close</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Close</td>
</tr>
<tr>
<th><a href="#destroy"><strong>destroy</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Destroy</td>
</tr>
<tr>
<th><a href="#gc"><strong>gc</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Garbage Collector</td>
</tr>

</table>





### Properties


<hr>

#### $cache

```php
protected static $cache = [];
```











### Methods


<hr>

#### open()

```php
public function open($savePath, $name) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Open
</td></tr>
</table>

<table>
<tr><td>
Ensures we have an initialized database connection.
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
<td><code>$savePath</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Path to session files' directory</td>
</tr>

<tr>
<td>2.</td>
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Session cookie name</td>
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
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (65 - 68)</small></summary>

```php
public function open($savePath, $name): bool
{
	return true;
}
```

</details>


<hr>

#### read()

```php
public function read($sessionID) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Read
</td></tr>
</table>

<table>
<tr><td>
Reads session data and acquires a lock
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
<td><code>$sessionID</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Session ID</td>
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
<summary><small>Source: 4 lines (81 - 84)</small></summary>

```php
public function read($sessionID): string
{
	return '';
}
```

</details>


<hr>

#### write()

```php
public function write($sessionID, $sessionData) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Write
</td></tr>
</table>

<table>
<tr><td>
Writes (create / update) session data
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
<td><code>$sessionID</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Session ID</td>
</tr>

<tr>
<td>2.</td>
<td><code>$sessionData</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Serialized session data</td>
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
<summary><small>Source: 4 lines (98 - 101)</small></summary>

```php
public function write($sessionID, $sessionData): bool
{
	return true;
}
```

</details>


<hr>

#### close()

```php
public function close() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Close
</td></tr>
</table>

<table>
<tr><td>
Releases locks and closes file descriptor.
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
<summary><small>Source: 4 lines (112 - 115)</small></summary>

```php
public function close(): bool
{
	return true;
}
```

</details>


<hr>

#### destroy()

```php
public function destroy($sessionID) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Destroy
</td></tr>
</table>

<table>
<tr><td>
Destroys the current session.
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
<td><code>$sessionID</code></td>
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
<summary><small>Source: 4 lines (128 - 131)</small></summary>

```php
public function destroy($sessionID): bool
{
	return true;
}
```

</details>


<hr>

#### gc()

```php
public function gc($maxlifetime) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Garbage Collector
</td></tr>
</table>

<table>
<tr><td>
Deletes expired sessions
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
<td><code>$maxlifetime</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Maximum lifetime of sessions</td>
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
<summary><small>Source: 4 lines (144 - 147)</small></summary>

```php
public function gc($maxlifetime): bool
{
	return true;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Session/Handlers/ArrayHandler.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Exceptions/SessionException.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Handlers/BaseHandler.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:18**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>