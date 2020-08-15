


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/FormatRules.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FileRules.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Rules.md">next</a></td>
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
<td>framework/system/Validation/FormatRules.php
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



 

 
## CodeIgniter\Validation\FormatRules

<table style="text-align:left">
<tr><th>Class</th><td>FormatRules</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Validation\FormatRules</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Format validation Rules.
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Validation
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
<th><a href="#alpha"><strong>alpha</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Alpha</td>
</tr>
<tr>
<th><a href="#alpha_space"><strong>alpha_space</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Alpha with spaces.</td>
</tr>
<tr>
<th><a href="#alpha_dash"><strong>alpha_dash</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Alphanumeric with underscores and dashes</td>
</tr>
<tr>
<th><a href="#alpha_numeric_punct"><strong>alpha_numeric_punct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Alphanumeric, spaces, and a limited set of punctuation characters.</td>
</tr>
<tr>
<th><a href="#alpha_numeric"><strong>alpha_numeric</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Alphanumeric</td>
</tr>
<tr>
<th><a href="#alpha_numeric_space"><strong>alpha_numeric_space</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Alphanumeric w/ spaces</td>
</tr>
<tr>
<th><a href="#string"><strong>string</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Any type of string</td>
</tr>
<tr>
<th><a href="#decimal"><strong>decimal</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Decimal number</td>
</tr>
<tr>
<th><a href="#hex"><strong>hex</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>String of hexidecimal characters</td>
</tr>
<tr>
<th><a href="#integer"><strong>integer</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Integer</td>
</tr>
<tr>
<th><a href="#is_natural"><strong>is_natural</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Is a Natural number  (0,1,2,3, etc.)</td>
</tr>
<tr>
<th><a href="#is_natural_no_zero"><strong>is_natural_no_zero</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Is a Natural number, but not a zero  (1,2,3, etc.)</td>
</tr>
<tr>
<th><a href="#numeric"><strong>numeric</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Numeric</td>
</tr>
<tr>
<th><a href="#regex_match"><strong>regex_match</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Compares value against a regular expression pattern.</td>
</tr>
<tr>
<th><a href="#timezone"><strong>timezone</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Validates that the string is a valid timezone as per the
timezone_identifiers_list function.</td>
</tr>
<tr>
<th><a href="#valid_base64"><strong>valid_base64</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Valid Base64</td>
</tr>
<tr>
<th><a href="#valid_json"><strong>valid_json</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Valid JSON</td>
</tr>
<tr>
<th><a href="#valid_email"><strong>valid_email</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks for a correctly formatted email address</td>
</tr>
<tr>
<th><a href="#valid_emails"><strong>valid_emails</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Validate a comma-separated list of email addresses.</td>
</tr>
<tr>
<th><a href="#valid_ip"><strong>valid_ip</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Validate an IP address (human readable format or binary string - inet_pton)</td>
</tr>
<tr>
<th><a href="#valid_url"><strong>valid_url</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks a URL to ensure it&#039;s formed correctly.</td>
</tr>
<tr>
<th><a href="#valid_date"><strong>valid_date</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks for a valid date and matches a given date format</td>
</tr>

</table>






### Methods


<hr>

#### alpha()

```php
public function alpha(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alpha
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (57 - 60)</small></summary>

```php
public function alpha(string $str = null): bool
{
	return ctype_alpha($str);
}
```

</details>


<hr>

#### alpha_space()

```php
public function alpha_space(string $value = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alpha with spaces.
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
<td><em>string
</em></td>
<td>false</td>
<td>Value.</td>
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
<summary><small>Source: 9 lines (69 - 77)</small></summary>

```php
public function alpha_space(string $value = null): bool
{
	if ($value === null)
	{
		return true;
	}

	return (bool) preg_match('/^[A-Z ]+$/i', $value);
}
```

</details>


<hr>

#### alpha_dash()

```php
public function alpha_dash(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alphanumeric with underscores and dashes
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (86 - 89)</small></summary>

```php
public function alpha_dash(string $str = null): bool
{
		return (bool) preg_match('/^[a-z0-9_-]+$/i', $str);
}
```

</details>


<hr>

#### alpha_numeric_punct()

```php
public function alpha_numeric_punct($str)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alphanumeric, spaces, and a limited set of punctuation characters.
</td></tr>
</table>

<table>
<tr><td>
Accepted punctuation characters are: ~ tilde, ! exclamation,
# number, $ dollar, %% percent, & ampersand, * asterisk, - dash,
_ underscore, + plus, = equals, | vertical bar, : colon, . period
~ ! # $ %% & * - _ + = | : .
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (102 - 105)</small></summary>

```php
public function alpha_numeric_punct($str)
{
	return (bool) preg_match('/^[A-Z0-9 ~!#$%\&\*\-_+=|:.]+$/i', $str);
}
```

</details>


<hr>

#### alpha_numeric()

```php
public function alpha_numeric(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alphanumeric
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (114 - 117)</small></summary>

```php
public function alpha_numeric(string $str = null): bool
{
	return ctype_alnum($str);
}
```

</details>


<hr>

#### alpha_numeric_space()

```php
public function alpha_numeric_space(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alphanumeric w/ spaces
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (126 - 129)</small></summary>

```php
public function alpha_numeric_space(string $str = null): bool
{
	return (bool) preg_match('/^[A-Z0-9 ]+$/i', $str);
}
```

</details>


<hr>

#### string()

```php
public function string($str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Any type of string
</td></tr>
</table>

<table>
<tr><td>
Note: we specifically do NOT type hint $str here so that
it doesn't convert numbers into strings.
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
<td><code>$str</code></td>
<td><em>string<br>null
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
<summary><small>Source: 4 lines (141 - 144)</small></summary>

```php
public function string($str = null): bool
{
	return is_string($str);
}
```

</details>


<hr>

#### decimal()

```php
public function decimal(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Decimal number
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (153 - 156)</small></summary>

```php
public function decimal(string $str = null): bool
{
	return (bool) preg_match('/^[-+]?[0-9]{0,}\.?[0-9]+$/', $str);
}
```

</details>


<hr>

#### hex()

```php
public function hex(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
String of hexidecimal characters
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (165 - 168)</small></summary>

```php
public function hex(string $str = null): bool
{
	return ctype_xdigit($str);
}
```

</details>


<hr>

#### integer()

```php
public function integer(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Integer
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (177 - 180)</small></summary>

```php
public function integer(string $str = null): bool
{
	return (bool) preg_match('/^[\-+]?[0-9]+$/', $str);
}
```

</details>


<hr>

#### is_natural()

```php
public function is_natural(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Is a Natural number  (0,1,2,3, etc.)
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (188 - 191)</small></summary>

```php
public function is_natural(string $str = null): bool
{
	return ctype_digit($str);
}
```

</details>


<hr>

#### is_natural_no_zero()

```php
public function is_natural_no_zero(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Is a Natural number, but not a zero  (1,2,3, etc.)
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (199 - 202)</small></summary>

```php
public function is_natural_no_zero(string $str = null): bool
{
	return ($str !== '0' && ctype_digit($str));
}
```

</details>


<hr>

#### numeric()

```php
public function numeric(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Numeric
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (211 - 214)</small></summary>

```php
public function numeric(string $str = null): bool
{
	return (bool) preg_match('/^[\-+]?[0-9]*\.?[0-9]+$/', $str);
}
```

</details>


<hr>

#### regex_match()

```php
public function regex_match(string $str = null, string $pattern) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Compares value against a regular expression pattern.
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$pattern</code></td>
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
<summary><small>Source: 9 lines (224 - 232)</small></summary>

```php
public function regex_match(string $str = null, string $pattern): bool
{
	if (strpos($pattern, '/') !== 0)
	{
		$pattern = "/{$pattern}/";
	}

	return (bool) preg_match($pattern, $str);
}
```

</details>


<hr>

#### timezone()

```php
public function timezone(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validates that the string is a valid timezone as per the
timezone_identifiers_list function.
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (244 - 247)</small></summary>

```php
public function timezone(string $str = null): bool
{
	return in_array($str, timezone_identifiers_list());
}
```

</details>


<hr>

#### valid_base64()

```php
public function valid_base64(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Valid Base64
</td></tr>
</table>

<table>
<tr><td>
Tests a string for characters outside of the Base64 alphabet
as defined by RFC 2045 <a href="http://www.faqs.org/rfcs/rfc2045">http://www.faqs.org/rfcs/rfc2045</a>
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (258 - 261)</small></summary>

```php
public function valid_base64(string $str = null): bool
{
	return (base64_encode(base64_decode($str)) === $str);
}
```

</details>


<hr>

#### valid_json()

```php
public function valid_json(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Valid JSON
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
<td><code>$str</code></td>
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
<summary><small>Source: 5 lines (270 - 274)</small></summary>

```php
public function valid_json(string $str = null): bool
{
	json_decode($str);
	return json_last_error() === JSON_ERROR_NONE;
}
```

</details>


<hr>

#### valid_email()

```php
public function valid_email(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks for a correctly formatted email address
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
<td><code>$str</code></td>
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
<summary><small>Source: 9 lines (283 - 291)</small></summary>

```php
public function valid_email(string $str = null): bool
{
	if (function_exists('idn_to_ascii') && defined('INTL_IDNA_VARIANT_UTS46') && preg_match('#\A([^@]+)@(.+)\z#', $str, $matches))
	{
		$str = $matches[1] . '@' . idn_to_ascii($matches[2], 0, INTL_IDNA_VARIANT_UTS46);
	}

	return (bool) filter_var($str, FILTER_VALIDATE_EMAIL);
}
```

</details>


<hr>

#### valid_emails()

```php
public function valid_emails(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validate a comma-separated list of email addresses.
</td></tr>
</table>

<table>
<tr><td>
Example:
valid_emails[<script type="text/javascript">var l=new Array();l[0] = '>';l[1] = 'a';l[2] = '/';l[3] = '<';l[4] = '|109';l[5] = '|111';l[6] = '|99';l[7] = '|46';l[8] = '|101';l[9] = '|108';l[10] = '|112';l[11] = '|109';l[12] = '|97';l[13] = '|120';l[14] = '|101';l[15] = '|64';l[16] = '|101';l[17] = '|110';l[18] = '|111';l[19] = '>';l[20] = '"';l[21] = '|109';l[22] = '|111';l[23] = '|99';l[24] = '|46';l[25] = '|101';l[26] = '|108';l[27] = '|112';l[28] = '|109';l[29] = '|97';l[30] = '|120';l[31] = '|101';l[32] = '|64';l[33] = '|101';l[34] = '|110';l[35] = '|111';l[36] = ':';l[37] = 'o';l[38] = 't';l[39] = 'l';l[40] = 'i';l[41] = 'a';l[42] = 'm';l[43] = '"';l[44] = '=';l[45] = 'f';l[46] = 'e';l[47] = 'r';l[48] = 'h';l[49] = ' ';l[50] = 'a';l[51] = '<';for (var i = l.length-1; i >= 0; i=i-1) {if (l[i].substring(0, 1) === '|') document.write("&#"+unescape(l[i].substring(1))+";");else document.write(unescape(l[i]));}</script>,<script type="text/javascript">var l=new Array();l[0] = '>';l[1] = 'a';l[2] = '/';l[3] = '<';l[4] = '|109';l[5] = '|111';l[6] = '|99';l[7] = '|46';l[8] = '|101';l[9] = '|108';l[10] = '|112';l[11] = '|109';l[12] = '|97';l[13] = '|120';l[14] = '|101';l[15] = '|64';l[16] = '|111';l[17] = '|119';l[18] = '|116';l[19] = '>';l[20] = '"';l[21] = '|109';l[22] = '|111';l[23] = '|99';l[24] = '|46';l[25] = '|101';l[26] = '|108';l[27] = '|112';l[28] = '|109';l[29] = '|97';l[30] = '|120';l[31] = '|101';l[32] = '|64';l[33] = '|111';l[34] = '|119';l[35] = '|116';l[36] = ':';l[37] = 'o';l[38] = 't';l[39] = 'l';l[40] = 'i';l[41] = 'a';l[42] = 'm';l[43] = '"';l[44] = '=';l[45] = 'f';l[46] = 'e';l[47] = 'r';l[48] = 'h';l[49] = ' ';l[50] = 'a';l[51] = '<';for (var i = l.length-1; i >= 0; i=i-1) {if (l[i].substring(0, 1) === '|') document.write("&#"+unescape(l[i].substring(1))+";");else document.write(unescape(l[i]));}</script>]
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
<td><code>$str</code></td>
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
<summary><small>Source: 18 lines (303 - 320)</small></summary>

```php
public function valid_emails(string $str = null): bool
{
	foreach (explode(',', $str) as $email)
	{
		$email = trim($email);
		if ($email === '')
		{
			return false;
		}

		if ($this->valid_email($email) === false)
		{
			return false;
		}
	}

	return true;
}
```

</details>


<hr>

#### valid_ip()

```php
public function valid_ip(string $ip = null, string $which = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validate an IP address (human readable format or binary string - inet_pton)
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
<td><code>$ip</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>IP Address</td>
</tr>

<tr>
<td>2.</td>
<td><code>$which</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>IP protocol: 'ipv4' or 'ipv6'</td>
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
<summary><small>Source: 21 lines (330 - 350)</small></summary>

```php
public function valid_ip(string $ip = null, string $which = null): bool
{
	if (empty($ip))
	{
		return false;
	}
	switch (strtolower($which))
	{
		case 'ipv4':
			$which = FILTER_FLAG_IPV4;
			break;
		case 'ipv6':
			$which = FILTER_FLAG_IPV6;
			break;
		default:
			$which = null;
			break;
	}

	return (bool) filter_var($ip, FILTER_VALIDATE_IP, $which) || (! ctype_print($ip) && (bool) filter_var(inet_ntop($ip), FILTER_VALIDATE_IP, $which));
}
```

</details>


<hr>

#### valid_url()

```php
public function valid_url(string $str = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks a URL to ensure it's formed correctly.
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
<td><code>$str</code></td>
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
<summary><small>Source: 20 lines (359 - 378)</small></summary>

```php
public function valid_url(string $str = null): bool
{
	if (empty($str))
	{
		return false;
	}
	elseif (preg_match('/^(?:([^:]*)\:)?\/\/(.+)$/', $str, $matches))
	{
		if (! in_array($matches[1], ['http', 'https'], true))
		{
			return false;
		}

		$str = $matches[2];
	}

	$str = 'http://' . $str;

	return (filter_var($str, FILTER_VALIDATE_URL) !== false);
}
```

</details>


<hr>

#### valid_date()

```php
public function valid_date(string $str = null, string $format = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks for a valid date and matches a given date format
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (388 - 398)</small></summary>

```php
public function valid_date(string $str = null, string $format = null): bool
{
	if (empty($format))
	{
		return (bool) strtotime($str);
	}

	$date = \DateTime::createFromFormat($format, $str);

	return (bool) $date && \DateTime::getLastErrors()['warning_count'] === 0 && \DateTime::getLastErrors()['error_count'] === 0;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/FormatRules.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FileRules.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Rules.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>