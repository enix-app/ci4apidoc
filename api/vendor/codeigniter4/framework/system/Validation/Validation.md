


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/Validation.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Rules.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">next</a></td>
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
<td>framework/system/Validation/Validation.php
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
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md"><strong>CodeIgniter\Validation\Exceptions\ValidationException</strong></a>
</td>
<td>ValidationException</td>
</tr>
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/View/RendererInterface.md"><strong>CodeIgniter\View\RendererInterface</strong></a>
</td>
<td>RendererInterface</td>
</tr>
</table>



 
## CodeIgniter\Validation\Validation

<table style="text-align:left">
<tr><th>Class</th><td>Validation</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Validation\Validation</td></tr>
<tr><th>Implements</th>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">CodeIgniter\Validation\ValidationInterface</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validator
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
<th><a href="#ruleSetFiles"><strong>ruleSetFiles</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Files to load with validation functions.</td>
</tr>
<tr>
<th><a href="#ruleSetInstances"><strong>ruleSetInstances</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The loaded instances of our validation files.</td>
</tr>
<tr>
<th><a href="#rules"><strong>rules</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores the actual rules that should
be ran against $data.</td>
</tr>
<tr>
<th><a href="#data"><strong>data</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The data that should be validated,
where &#039;key&#039; is the alias, with value.</td>
</tr>
<tr>
<th><a href="#errors"><strong>errors</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Any generated errors during validation.</td>
</tr>
<tr>
<th><a href="#customErrors"><strong>customErrors</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores custom error message to use
during validation. Where &#039;key&#039; is the alias.</td>
</tr>
<tr>
<th><a href="#config"><strong>config</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Our configuration.</td>
</tr>
<tr>
<th><a href="#view"><strong>view</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The view renderer used to render validation messages.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Validation constructor.</td>
</tr>
<tr>
<th><a href="#run"><strong>run</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runs the validation process, returning true/false determining whether
validation was successful or not.</td>
</tr>
<tr>
<th><a href="#check"><strong>check</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Check; runs the validation process, returning true or false
determining whether validation was successful or not.</td>
</tr>
<tr>
<th><a href="#processRules"><strong>processRules</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Runs all of $rules against $field, until one fails, or
all of them have been processed. If one fails, it adds
the error to $this-&gt;errors and moves on to the next,
so that we can collect all of the first errors.</td>
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
<th><a href="#setRule"><strong>setRule</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets an individual rule and custom error messages for a single field.</td>
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
<th><a href="#getRules"><strong>getRules</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns all of the rules currently defined.</td>
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
<th><a href="#getRuleGroup"><strong>getRuleGroup</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get rule group.</td>
</tr>
<tr>
<th><a href="#setRuleGroup"><strong>setRuleGroup</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set rule group.</td>
</tr>
<tr>
<th><a href="#listErrors"><strong>listErrors</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the rendered HTML of the errors as defined in $template.</td>
</tr>
<tr>
<th><a href="#showError"><strong>showError</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Displays a single error in formatted HTML as defined in the $template view.</td>
</tr>
<tr>
<th><a href="#loadRuleSets"><strong>loadRuleSets</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Loads all of the rulesets classes that have been defined in the
Config\Validation and stores them locally so we can use them.</td>
</tr>
<tr>
<th><a href="#loadRuleGroup"><strong>loadRuleGroup</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Loads custom rule groups (if set) into the current rules.</td>
</tr>
<tr>
<th><a href="#fillPlaceholders"><strong>fillPlaceholders</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Replace any placeholders within the rules with the values that
match the &#039;key&#039; of any properties being set. For example, if
we had the following $data array:</td>
</tr>
<tr>
<th><a href="#hasError"><strong>hasError</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks to see if an error exists for the given field.</td>
</tr>
<tr>
<th><a href="#getError"><strong>getError</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the error(s) for a specified $field (or empty string if not
set).</td>
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
<th><a href="#getErrorMessage"><strong>getErrorMessage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Attempts to find the appropriate error message</td>
</tr>
<tr>
<th><a href="#splitRules"><strong>splitRules</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Split rules string by pipe operator.</td>
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





### Properties


<hr>

#### $ruleSetFiles

```php
protected $ruleSetFiles;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Files to load with validation functions.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
</tr>
</table>


<hr>

#### $ruleSetInstances

```php
protected $ruleSetInstances = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The loaded instances of our validation files.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
</tr>
</table>


<hr>

#### $rules

```php
protected $rules = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the actual rules that should
be ran against $data.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
</tr>
</table>


<hr>

#### $data

```php
protected $data = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The data that should be validated,
where 'key' is the alias, with value.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
</tr>
</table>


<hr>

#### $errors

```php
protected $errors = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Any generated errors during validation.
</td></tr>
</table>

<table>
<tr><td>
'key' is the alias, 'value' is the message.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
</tr>
</table>


<hr>

#### $customErrors

```php
protected $customErrors = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores custom error message to use
during validation. Where 'key' is the alias.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array
</td>
</tr>
</table>


<hr>

#### $config

```php
protected $config;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Our configuration.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Config\Validation
</td>
</tr>
</table>


<hr>

#### $view

```php
protected $view;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The view renderer used to render validation messages.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\RendererInterface
</td>
</tr>
</table>







### Methods


<hr>

#### __construct()

```php
public function __construct($config, RendererInterface $view)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validation constructor.
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
<td><code>$config</code></td>
<td><em>\Config\Validation
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$view</code></td>
<td><em>\RendererInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 8 lines (119 - 126)</small></summary>

```php
public function __construct($config, RendererInterface $view)
{
	$this->ruleSetFiles = $config->ruleSets;

	$this->config = $config;

	$this->view = $view;
}
```

</details>


<hr>

#### run()

```php
public function run(array $data = null, string $group = null, string $db_group = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs the validation process, returning true/false determining whether
validation was successful or not.
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

<tr>
<td>3.</td>
<td><code>$db_group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The database group to use.</td>
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
<summary><small>Source: 55 lines (140 - 194)</small></summary>

```php
public function run(array $data = null, string $group = null, string $db_group = null): bool
{
	$data = $data ?? $this->data;

	// i.e. is_unique
	$data['DBGroup'] = $db_group;

	$this->loadRuleSets();

	$this->loadRuleGroup($group);

	// If no rules exist, we return false to ensure
	// the developer didn't forget to set the rules.
	if (empty($this->rules))
	{
		return false;
	}

	// Replace any placeholders (i.e. {id}) in the rules with
	// the value found in $data, if exists.
	$this->rules = $this->fillPlaceholders($this->rules, $data);

	// Need this for searching arrays in validation.
	helper('array');

	// Run through each rule. If we have any field set for
	// this rule, then we need to run them through!
	foreach ($this->rules as $rField => $rSetup)
	{
		// Blast $rSetup apart, unless it's already an array.
		$rules = $rSetup['rules'] ?? $rSetup;

		if (is_string($rules))
		{
			$rules = $this->splitRules($rules);
		}

		$value          = dot_array_search($rField, $data);
		$fieldNameToken = explode('.', $rField);

		if (is_array($value) && end($fieldNameToken) === '*')
		{
			foreach ($value as $val)
			{
				$this->processRules($rField, $rSetup['label'] ?? $rField, $val ?? null, $rules, $data);
			}
		}
		else
		{
			$this->processRules($rField, $rSetup['label'] ?? $rField, $value ?? null, $rules, $data);
		}
	}

	return ! empty($this->getErrors()) ? false : true;
}
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
determining whether validation was successful or not.
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
<summary><small>Source: 9 lines (208 - 216)</small></summary>

```php
public function check($value, string $rule, array $errors = []): bool
{
	$this->reset();
	$this->setRule('check', null, $rule, $errors);

	return $this->run([
		'check' => $value,
	]);
}
```

</details>


<hr>

#### processRules()

```php
protected function processRules(string $field, string $label = null, $value, $rules = null, array $data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runs all of $rules against $field, until one fails, or
all of them have been processed. If one fails, it adds
the error to $this->errors and moves on to the next,
so that we can collect all of the first errors.
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

<tr>
<td>2.</td>
<td><code>$label</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$value</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Value to be validated, can be a string or an array</td>
</tr>

<tr>
<td>4.</td>
<td><code>$rules</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$data</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>// All of the fields to check.</td>
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
<summary><small>Source: 121 lines (234 - 354)</small></summary>

```php
protected function processRules(string $field, string $label = null, $value, $rules = null, array $data): bool
{
	// If the if_exist rule is defined...
	if (in_array('if_exist', $rules))
	{
		// and the current field does not exists in the input data
		// we can return true. Ignoring all other rules to this field.
		if (! array_key_exists($field, $data))
		{
			return true;
		}
		// Otherwise remove the if_exist rule and continue the process
		$rules = array_diff($rules, ['if_exist']);
	}

	if (in_array('permit_empty', $rules))
	{
		if (! in_array('required', $rules) && (is_array($value) ? empty($value) : (trim($value) === '')))
		{
			$passed = true;

			foreach ($rules as $rule)
			{
				if (preg_match('/(.*?)\[(.*)\]/', $rule, $match))
				{
					$rule  = $match[1];
					$param = $match[2];

					if (! in_array($rule, ['required_with', 'required_without']))
					{
						continue;
					}

					// Check in our rulesets
					foreach ($this->ruleSetInstances as $set)
					{
						if (! method_exists($set, $rule))
						{
							continue;
						}

						$passed = $passed && $set->$rule($value, $param, $data);
						break;
					}
				}
			}

			if ($passed === true)
			{
				return true;
			}
		}

		$rules = array_diff($rules, ['permit_empty']);
	}

	foreach ($rules as $rule)
	{
		$callable = is_callable($rule);
		$passed   = false;

		// Rules can contain parameters: max_length[5]
		$param = false;
		if (! $callable && preg_match('/(.*?)\[(.*)\]/', $rule, $match))
		{
			$rule  = $match[1];
			$param = $match[2];
		}

		// Placeholder for custom errors from the rules.
		$error = null;

		// If it's a callable, call and and get out of here.
		if ($callable)
		{
			$passed = $param === false ? $rule($value) : $rule($value, $param, $data);
		}
		else
		{
			$found = false;

			// Check in our rulesets
			foreach ($this->ruleSetInstances as $set)
			{
				if (! method_exists($set, $rule))
				{
					continue;
				}

				$found = true;

				$passed = $param === false ? $set->$rule($value, $error) : $set->$rule($value, $param, $data, $error);
				break;
			}

			// If the rule wasn't found anywhere, we
			// should throw an exception so the developer can find it.
			if (! $found)
			{
				throw ValidationException::forRuleNotFound($rule);
			}
		}

		// Set the error message if we didn't survive.
		if ($passed === false)
		{
			// if the $value is an array, convert it to as string representation
			if (is_array($value))
			{
				$value = '[' . implode(', ', $value) . ']';
			}

			$this->errors[$field] = is_null($error) ? $this->getErrorMessage($rule, $field, $label, $param, $value)
				: $error;

			return false;
		}
	}

	return true;
}
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
<td><em>\CodeIgniter\HTTP\RequestInterface<br>\CodeIgniter\HTTP\IncomingRequest
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
<summary><small>Source: 13 lines (366 - 378)</small></summary>

```php
public function withRequest(RequestInterface $request): ValidationInterface
{
	if (in_array($request->getMethod(), ['put', 'patch', 'delete']))
	{
		$this->data = $request->getRawInput();
	}
	else
	{
		$this->data = $request->getVar() ?? [];
	}

	return $this;
}
```

</details>


<hr>

#### setRule()

```php
public function setRule(string $field, string $label = null, string $rules, array $errors = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets an individual rule and custom error messages for a single field.
</td></tr>
</table>

<table>
<tr><td>
The custom error message should be just the messages that apply to
this field, like so:

   [
       'rule' => 'message',
       'rule' => 'message'
   ]
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

<tr>
<td>2.</td>
<td><code>$label</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$rules</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$errors</code></td>
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
<summary><small>Source: 12 lines (403 - 414)</small></summary>

```php
public function setRule(string $field, string $label = null, string $rules, array $errors = [])
{
	$this->rules[$field] = [
		'label' => $label,
		'rules' => $rules,
	];
	$this->customErrors  = array_merge($this->customErrors, [
		$field => $errors,
	]);

	return $this;
}
```

</details>


<hr>

#### setRules()

```php
public function setRules(array $rules, array $errors = array()) : ValidationInterface
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the rules that should be used to validate the items.
</td></tr>
</table>

<table>
<tr><td>
Rules should be an array formatted like:

   [
       'field' => 'rule1|rule2'
   ]

The $errors array should be formatted like:
   [
       'field' => [
           'rule' => 'message',
           'rule' => 'message
       ],
   ]
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
<td><code>$errors</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>// An array of custom error messages</td>
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
<summary><small>Source: 20 lines (439 - 458)</small></summary>

```php
public function setRules(array $rules, array $errors = []): ValidationInterface
{
	$this->customErrors = $errors;

	foreach ($rules as $field => &$rule)
	{
		if (is_array($rule))
		{
			if (array_key_exists('errors', $rule))
			{
				$this->customErrors[$field] = $rule['errors'];
				unset($rule['errors']);
			}
		}
	}

	$this->rules = $rules;

	return $this;
}
```

</details>


<hr>

#### getRules()

```php
public function getRules() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns all of the rules currently defined.
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
<summary><small>Source: 4 lines (467 - 470)</small></summary>

```php
public function getRules(): array
{
	return $this->rules;
}
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
<summary><small>Source: 4 lines (481 - 484)</small></summary>

```php
public function hasRule(string $field): bool
{
	return array_key_exists($field, $this->rules);
}
```

</details>


<hr>

#### getRuleGroup()

```php
public function getRuleGroup(string $group) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get rule group.
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
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Group.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string[]
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\InvalidArgumentException
</td>
</tr>
</table>



<details>
<summary><small>Source: 14 lines (497 - 510)</small></summary>

```php
public function getRuleGroup(string $group): array
{
	if (! isset($this->config->$group))
	{
		throw ValidationException::forGroupNotFound($group);
	}

	if (! is_array($this->config->$group))
	{
		throw ValidationException::forGroupNotArray($group);
	}

	return $this->config->$group;
}
```

</details>


<hr>

#### setRuleGroup()

```php
public function setRuleGroup(string $group)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set rule group.
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
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Group.</td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\InvalidArgumentException
</td>
</tr>
</table>



<details>
<summary><small>Source: 11 lines (521 - 531)</small></summary>

```php
public function setRuleGroup(string $group)
{
	$rules = $this->getRuleGroup($group);
	$this->setRules($rules);

	$errorName = $group . '_errors';
	if (isset($this->config->$errorName))
	{
		$this->customErrors = $this->config->$errorName;
	}
}
```

</details>


<hr>

#### listErrors()

```php
public function listErrors(string $template = 'list') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the rendered HTML of the errors as defined in $template.
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
<td><code>$template</code></td>
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
<summary><small>Source: 10 lines (540 - 549)</small></summary>

```php
public function listErrors(string $template = 'list'): string
{
	if (! array_key_exists($template, $this->config->templates))
	{
		throw ValidationException::forInvalidTemplate($template);
	}

	return $this->view->setVar('errors', $this->getErrors())
					->render($this->config->templates[$template]);
}
```

</details>


<hr>

#### showError()

```php
public function showError(string $field, string $template = 'single') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Displays a single error in formatted HTML as defined in the $template view.
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

<tr>
<td>2.</td>
<td><code>$template</code></td>
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
<summary><small>Source: 15 lines (561 - 575)</small></summary>

```php
public function showError(string $field, string $template = 'single'): string
{
	if (! array_key_exists($field, $this->getErrors()))
	{
		return '';
	}

	if (! array_key_exists($template, $this->config->templates))
	{
		throw ValidationException::forInvalidTemplate($template);
	}

	return $this->view->setVar('error', $this->getError($field))
					->render($this->config->templates[$template]);
}
```

</details>


<hr>

#### loadRuleSets()

```php
protected function loadRuleSets()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Loads all of the rulesets classes that have been defined in the
Config\Validation and stores them locally so we can use them.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 12 lines (583 - 594)</small></summary>

```php
protected function loadRuleSets()
{
	if (empty($this->ruleSetFiles))
	{
		throw ValidationException::forNoRuleSets();
	}

	foreach ($this->ruleSetFiles as $file)
	{
		$this->ruleSetInstances[] = new $file();
	}
}
```

</details>


<hr>

#### loadRuleGroup()

```php
public function loadRuleGroup(string $group = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Loads custom rule groups (if set) into the current rules.
</td></tr>
</table>

<table>
<tr><td>
Rules can be pre-defined in Config\Validation and can
be any name, but must all still be an array of the
same format used with setRules(). Additionally, check
for {group}_errors for an array of custom error messages.
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
<td><code>$group</code></td>
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
<td>array<br>\ValidationException<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 30 lines (610 - 639)</small></summary>

```php
public function loadRuleGroup(string $group = null)
{
	if (empty($group))
	{
		return null;
	}

	if (! isset($this->config->$group))
	{
		throw ValidationException::forGroupNotFound($group);
	}

	if (! is_array($this->config->$group))
	{
		throw ValidationException::forGroupNotArray($group);
	}

	$this->setRules($this->config->$group);

	// If {group}_errors exists in the config file,
	// then override our custom errors with them.
	$errorName = $group . '_errors';

	if (isset($this->config->$errorName))
	{
		$this->customErrors = $this->config->$errorName;
	}

	return $this->rules;
}
```

</details>


<hr>

#### fillPlaceholders()

```php
protected function fillPlaceholders(array $rules, array $data) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replace any placeholders within the rules with the values that
match the 'key' of any properties being set. For example, if
we had the following $data array:
</td></tr>
</table>

<table>
<tr><td>
[ 'id' => 13 ]

and the following rule:

 'required|is_unique[users,email,id,{id}]'

The value of {id} would be replaced with the actual id in the form data:

 'required|is_unique[users,email,id,13]'
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
<summary><small>Source: 35 lines (663 - 697)</small></summary>

```php
protected function fillPlaceholders(array $rules, array $data): array
{
	$replacements = [];

	foreach ($data as $key => $value)
	{
		$replacements["{{$key}}"] = $value;
	}

	if (! empty($replacements))
	{
		foreach ($rules as &$rule)
		{
			if (is_array($rule))
			{
				foreach ($rule as &$row)
				{
					// Should only be an `errors` array
					// which doesn't take placeholders.
					if (is_array($row))
					{
						continue;
					}

					$row = strtr($row, $replacements);
				}
				continue;
			}

			$rule = strtr($rule, $replacements);
		}
	}

	return $rules;
}
```

</details>


<hr>

#### hasError()

```php
public function hasError(string $field) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks to see if an error exists for the given field.
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
<summary><small>Source: 4 lines (711 - 714)</small></summary>

```php
public function hasError(string $field): bool
{
	return array_key_exists($field, $this->getErrors());
}
```

</details>


<hr>

#### getError()

```php
public function getError(string $field = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the error(s) for a specified $field (or empty string if not
set).
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
<td>Field.</td>
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
<summary><small>Source: 10 lines (726 - 735)</small></summary>

```php
public function getError(string $field = null): string
{
	if ($field === null && count($this->rules) === 1)
	{
		reset($this->rules);
		$field = key($this->rules);
	}

	return array_key_exists($field, $this->getErrors()) ? $this->errors[$field] : '';
}
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
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
</td>
</tr>
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (754 - 768)</small></summary>

```php
public function getErrors(): array
{
	// If we already have errors, we'll use those.
	// If we don't, check the session to see if any were
	// passed along from a redirect_with_input request.
	if (empty($this->errors) && ! is_cli())
	{
		if (isset($_SESSION, $_SESSION['_ci_validation_errors']))
		{
			$this->errors = unserialize($_SESSION['_ci_validation_errors']);
		}
	}

	return $this->errors ?? [];
}
```

</details>


<hr>

#### setError()

```php
public function setError(string $field, string $error) : ValidationInterface
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
<td><code>$field</code></td>
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
<summary><small>Source: 6 lines (780 - 785)</small></summary>

```php
public function setError(string $field, string $error): ValidationInterface
{
	$this->errors[$field] = $error;

	return $this;
}
```

</details>


<hr>

#### getErrorMessage()

```php
protected function getErrorMessage(string $rule, string $field, string $label = null, string $param = null, string $value = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to find the appropriate error message
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
<td><code>$rule</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$label</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$param</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>5.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The value that caused the validation to fail.</td>
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
<summary><small>Source: 20 lines (800 - 819)</small></summary>

```php
protected function getErrorMessage(string $rule, string $field, string $label = null, string $param = null, string $value = null): string
{
	// Check if custom message has been defined by user
	if (isset($this->customErrors[$field][$rule]))
	{
		$message = lang($this->customErrors[$field][$rule]);
	}
	else
	{
		// Try to grab a localized version of the message...
		// lang() will return the rule name back if not found,
		// so there will always be a string being returned.
		$message = lang('Validation.' . $rule);
	}

	$message = str_replace('{field}', empty($label) ? $field : lang($label), $message);
	$message = str_replace('{param}', empty($this->rules[$param]['label']) ? $param : lang($this->rules[$param]['label']), $message);

	return str_replace('{value}', $value, $message);
}
```

</details>


<hr>

#### splitRules()

```php
protected function splitRules(string $rules) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Split rules string by pipe operator.
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 17 lines (828 - 844)</small></summary>

```php
protected function splitRules(string $rules): array
{
	$non_escape_bracket  = '((?<!\\\\)(?:\\\\\\\\)*[\[\]])';
	$pipe_not_in_bracket = sprintf(
			'/\|(?=(?:[^\[\]]*%s[^\[\]]*%s)*(?![^\[\]]*%s))/',
			$non_escape_bracket,
			$non_escape_bracket,
			$non_escape_bracket
	);

	$_rules = preg_split(
			$pipe_not_in_bracket,
			$rules
	);

	return array_unique($_rules);
}
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
<summary><small>Source: 9 lines (857 - 865)</small></summary>

```php
public function reset(): ValidationInterface
{
	$this->data         = [];
	$this->rules        = [];
	$this->errors       = [];
	$this->customErrors = [];

	return $this;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/Validation.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Rules.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>