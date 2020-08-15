


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/ValidationInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Cell.md">next</a></td>
</tr>
</table>







# CodeIgniter\Validation 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Validation</td></tr>
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
<td>framework/system/Validation/ValidationInterface.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/CreditCardRules.md">CodeIgniter\Validation\CreditCardRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md">CodeIgniter\Validation\Exceptions\ValidationException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FileRules.md">CodeIgniter\Validation\FileRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FormatRules.md">CodeIgniter\Validation\FormatRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Rules.md">CodeIgniter\Validation\Rules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md">CodeIgniter\Validation\Validation</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">CodeIgniter\Validation\ValidationInterface</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/HTTP/RequestInterface.md"><strong>CodeIgniter\HTTP\RequestInterface</strong></a>
</td>
<td>RequestInterface</td>
</tr>
</table>



 
## CodeIgniter\Validation\ValidationInterface

<table style="text-align:left">
<tr><th>Interface</th><td>ValidationInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Validation\ValidationInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Expected behavior of a validator
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
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runs the validation process, returning true/false determining whether
or not validation was successful.</td>
</tr>
<tr>
<th><a href="#check"><strong>check</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Check; runs the validation process, returning true or false
determining whether or not validation was successful.</td>
</tr>
<tr>
<th><a href="#withRequest"><strong>withRequest</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Takes a Request object and grabs the input data to use from its
array values.</td>
</tr>
<tr>
<th><a href="#setRules"><strong>setRules</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Stores the rules that should be used to validate the items.</td>
</tr>
<tr>
<th><a href="#hasRule"><strong>hasRule</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if the rule for key $field has been set or not.</td>
</tr>
<tr>
<th><a href="#getError"><strong>getError</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the error for a specified $field (or empty string if not set).</td>
</tr>
<tr>
<th><a href="#getErrors"><strong>getErrors</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the array of errors that were encountered during
a run() call. The array should be in the following format:</td>
</tr>
<tr>
<th><a href="#setError"><strong>setError</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the error for a specific field. Used by custom validation methods.</td>
</tr>
<tr>
<th><a href="#reset"><strong>reset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Resets the class to a blank slate. Should be called whenever
you need to process more than one array.</td>
</tr>

</table>






### Methods


<hr>

#### run()

```php
public function run(array $data = null, string $group = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs the validation process, returning true/false determining whether
or not validation was successful.
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
<td>The array of data to validate.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The pre-defined group of rules to apply.</td>
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
public function run(array $data = null, string $group = null): bool;
```

</details>


<hr>

#### check()

```php
public function check($value, string $rule, array $errors = array()) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Check; runs the validation process, returning true or false
determining whether or not validation was successful.
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
<td><code>$value</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Value to validation.</td>
</tr>

<tr>
<td>2.</td>
<td><code>$rule</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Rule.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$errors</code></td>
<td><em>string[]
</em></td>
<td>false</td>
<td>Errors.</td>
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
<summary><small>Source: line 73</small></summary>

```php
public function check($value, string $rule, array $errors = []): bool;
```

</details>


<hr>

#### withRequest()

```php
public function withRequest(RequestInterface $request) : ValidationInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes a Request object and grabs the input data to use from its
array values.
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
<td><code>$request</code></td>
<td><em>\CodeIgniter\HTTP\RequestInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Validation\ValidationInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 85</small></summary>

```php
public function withRequest(RequestInterface $request): ValidationInterface;
```

</details>


<hr>

#### setRules()

```php
public function setRules(array $rules, array $messages = array()) : ValidationInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the rules that should be used to validate the items.
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
<td><code>$rules</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$messages</code></td>
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
<td>\CodeIgniter\Validation\ValidationInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 99</small></summary>

```php
public function setRules(array $rules, array $messages = []): ValidationInterface;
```

</details>


<hr>

#### hasRule()

```php
public function hasRule(string $field) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if the rule for key $field has been set or not.
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
<td><code>$field</code></td>
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
<summary><small>Source: line 110</small></summary>

```php
public function hasRule(string $field): bool;
```

</details>


<hr>

#### getError()

```php
public function getError(string $field) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the error for a specified $field (or empty string if not set).
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
<td><code>$field</code></td>
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
<summary><small>Source: line 124</small></summary>

```php
public function getError(string $field): string;
```

</details>


<hr>

#### getErrors()

```php
public function getErrors() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the array of errors that were encountered during
a run() call. The array should be in the following format:
</td></tr>
</table>

<table>
<tr><td>
[
    'field1' => 'error message',
    'field2' => 'error message',
]
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
<summary><small>Source: line 139</small></summary>

```php
public function getErrors(): array;
```

</details>


<hr>

#### setError()

```php
public function setError(string $alias, string $error) : ValidationInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the error for a specific field. Used by custom validation methods.
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
<td><code>$alias</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$error</code></td>
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
<td>\CodeIgniter\Validation\ValidationInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 151</small></summary>

```php
public function setError(string $alias, string $error): ValidationInterface;
```

</details>


<hr>

#### reset()

```php
public function reset() : ValidationInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Resets the class to a blank slate. Should be called whenever
you need to process more than one array.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\CodeIgniter\Validation\ValidationInterface
</td>
</tr>
</table>





<details>
<summary><small>Source: line 163</small></summary>

```php
public function reset(): ValidationInterface;
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/ValidationInterface.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/View/Cell.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>