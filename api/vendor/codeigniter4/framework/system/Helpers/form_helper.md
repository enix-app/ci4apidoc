


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/form_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/filesystem_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/html_helper.md">next</a></td>
</tr>
</table>




 



# Form Helper


<hr>

## form_open()

```php
function form_open(string $action = '', $attributes = array(), array $hidden = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Form Declaration
</td></tr>
</table>

<table>
<tr><td>
Creates the opening portion of the form.
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
<td><code>$action</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the URI segments of the form destination</td>
</tr>

<tr>
<td>2.</td>
<td><code>$attributes</code></td>
<td><em>array<br>string
</em></td>
<td>false</td>
<td>a key/value pair of attributes, or string representation</td>
</tr>

<tr>
<td>3.</td>
<td><code>$hidden</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>a key/value pair hidden data</td>
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
<summary><small>Source: 57 lines (63 - 119)</small></summary>

```php
function form_open(string $action = '', $attributes = [], array $hidden = []): string
{
	// If no action is provided then set to the current url
	if (! $action)
	{
		$action = current_url(true);
	} // If an action is not a full URL then turn it into one
	elseif (strpos($action, '://') === false)
	{
		// If an action has {locale}
		if (strpos($action, '{locale}') !== false)
		{
			$action = str_replace('{locale}', Services::request()->getLocale(), $action);
		}

		$action = site_url($action);
	}

	if (is_array($attributes) && array_key_exists('csrf_id', $attributes))
	{
		$csrfId = $attributes['csrf_id'];
		unset($attributes['csrf_id']);
	}

	$attributes = stringify_attributes($attributes);

	if (stripos($attributes, 'method=') === false)
	{
		$attributes .= ' method="post"';
	}
	if (stripos($attributes, 'accept-charset=') === false)
	{
		$config      = config(\Config\App::class);
		$attributes .= ' accept-charset="' . strtolower($config->charset) . '"';
	}

	$form = '<form action="' . $action . '"' . $attributes . ">\n";

	// Add CSRF field if enabled, but leave it out for GET requests and requests to external websites
	$before = Services::filters()
					  ->getFilters()['before'];

	if ((in_array('csrf', $before) || array_key_exists('csrf', $before)) && strpos($action, base_url()) !== false && ! stripos($form, 'method="get"'))
	{
		$form .= csrf_field($csrfId ?? null);
	}

	if (is_array($hidden))
	{
		foreach ($hidden as $name => $value)
		{
			$form .= form_hidden($name, $value);
		}
	}

	return $form;
}
```

</details>


<hr>

## form_open_multipart()

```php
function form_open_multipart(string $action = '', $attributes = array(), array $hidden = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Form Declaration - Multipart type
</td></tr>
</table>

<table>
<tr><td>
Creates the opening portion of the form, but with "multipart/form-data".
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
<td><code>$action</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The URI segments of the form destination</td>
</tr>

<tr>
<td>2.</td>
<td><code>$attributes</code></td>
<td><em>array<br>string
</em></td>
<td>false</td>
<td>A key/value pair of attributes, or the same as a string</td>
</tr>

<tr>
<td>3.</td>
<td><code>$hidden</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>A key/value pair hidden data</td>
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
<summary><small>Source: 13 lines (137 - 149)</small></summary>

```php
function form_open_multipart(string $action = '', $attributes = [], array $hidden = []): string
{
	if (is_string($attributes))
	{
		$attributes .= ' enctype="' . esc('multipart/form-data', 'attr') . '"';
	}
	else
	{
		$attributes['enctype'] = 'multipart/form-data';
	}

	return form_open($action, $attributes, $hidden);
}
```

</details>


<hr>

## form_hidden()

```php
function form_hidden($name, $value = '', bool $recursing = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Hidden Input Field
</td></tr>
</table>

<table>
<tr><td>
Generates hidden fields. You can pass a simple key/value string or
an associative array with multiple values.
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
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Field name or associative array to create multiple fields</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>Field value</td>
</tr>

<tr>
<td>3.</td>
<td><code>$recursing</code></td>
<td><em>bool
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
<summary><small>Source: 34 lines (168 - 201)</small></summary>

```php
function form_hidden($name, $value = '', bool $recursing = false): string
{
	static $form;

	if ($recursing === false)
	{
		$form = "\n";
	}

	if (is_array($name))
	{
		foreach ($name as $key => $val)
		{
			form_hidden($key, $val, true);
		}

		return $form;
	}

	if (! is_array($value))
	{
		$form .= '<input type="hidden" name="' . $name . '" value="' . esc($value) . "\" style=\"display:none;\" />\n";
	}
	else
	{
		foreach ($value as $k => $v)
		{
			$k = is_int($k) ? '' : $k;
			form_hidden($name . '[' . $k . ']', $v, true);
		}
	}

	return $form;
}
```

</details>


<hr>

## form_input()

```php
function form_input($data = '', string $value = '', $extra = '', string $type = 'text') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Text Input Field. If 'type' is passed in the $type field, it will be
used as the input type, for making 'email', 'phone', etc input fields.
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$extra</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$type</code></td>
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
<summary><small>Source: 10 lines (219 - 228)</small></summary>

```php
function form_input($data = '', string $value = '', $extra = '', string $type = 'text'): string
{
	$defaults = [
		'type'  => $type,
		'name'  => is_array($data) ? '' : $data,
		'value' => $value,
	];

	return '<input ' . parse_form_attributes($data, $defaults) . stringify_attributes($extra) . " />\n";
}
```

</details>


<hr>

## form_password()

```php
function form_password($data = '', string $value = '', $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Password Field
</td></tr>
</table>

<table>
<tr><td>
Identical to the input function but adds the "password" type
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 7 lines (246 - 252)</small></summary>

```php
function form_password($data = '', string $value = '', $extra = ''): string
{
	is_array($data) || $data = ['name' => $data];
	$data['type']            = 'password';

	return form_input($data, $value, $extra);
}
```

</details>


<hr>

## form_upload()

```php
function form_upload($data = '', string $value = '', $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Upload Field
</td></tr>
</table>

<table>
<tr><td>
Identical to the input function but adds the "file" type
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 11 lines (270 - 280)</small></summary>

```php
function form_upload($data = '', string $value = '', $extra = ''): string
{
	$defaults                = [
		'type' => 'file',
		'name' => '',
	];
	is_array($data) || $data = ['name' => $data];
	$data['type']            = 'file';

	return '<input ' . parse_form_attributes($data, $defaults) . stringify_attributes($extra) . " />\n";
}
```

</details>


<hr>

## form_textarea()

```php
function form_textarea($data = '', string $value = '', $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Textarea field
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 32 lines (296 - 327)</small></summary>

```php
function form_textarea($data = '', string $value = '', $extra = ''): string
{
	$defaults = [
		'name' => is_array($data) ? '' : $data,
		'cols' => '40',
		'rows' => '10',
	];
	if (! is_array($data) || ! isset($data['value']))
	{
		$val = $value;
	}
	else
	{
		$val = $data['value'];
		unset($data['value']); // textareas don't use the value attribute
	}

	// Unsets default rows and cols if defined in extra field as array or string.
	if ((is_array($extra) && array_key_exists('rows', $extra)) || (is_string($extra) && strpos(strtolower(preg_replace('/\s+/', '', $extra)), 'rows=') !== false))
	{
		unset($defaults['rows']);
	}

	if ((is_array($extra) && array_key_exists('cols', $extra)) || (is_string($extra) && strpos(strtolower(preg_replace('/\s+/', '', $extra)), 'cols=') !== false))
	{
		unset($defaults['cols']);
	}

	return '<textarea ' . rtrim(parse_form_attributes($data, $defaults)) . stringify_attributes($extra) . '>'
			. htmlspecialchars($val)
			. "</textarea>\n";
}
```

</details>


<hr>

## form_multiselect()

```php
function form_multiselect(string $name = '', array $options = array(), array $selected = array(), $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Multi-select menu
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

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$selected</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 11 lines (344 - 354)</small></summary>

```php
function form_multiselect(string $name = '', array $options = [], array $selected = [], $extra = ''): string
{
	$extra = stringify_attributes($extra);

	if (stripos($extra, 'multiple') === false)
	{
		$extra .= ' multiple="multiple"';
	}

	return form_dropdown($name, $options, $selected, $extra);
}
```

</details>


<hr>

## form_dropdown()

```php
function form_dropdown($data = '', $options = array(), $selected = array(), $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Drop-down Menu
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$selected</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 71 lines (371 - 441)</small></summary>

```php
function form_dropdown($data = '', $options = [], $selected = [], $extra = ''): string
{
	$defaults = [];
	if (is_array($data))
	{
		if (isset($data['selected']))
		{
			$selected = $data['selected'];
			unset($data['selected']); // select tags don't have a selected attribute
		}
		if (isset($data['options']))
		{
			$options = $data['options'];
			unset($data['options']); // select tags don't use an options attribute
		}
	}
	else
	{
		$defaults = ['name' => $data];
	}

	is_array($selected) || $selected = [$selected];
	is_array($options) || $options   = [$options];

	// If no selected state was submitted we will attempt to set it automatically
	if (empty($selected))
	{
		if (is_array($data))
		{
			if (isset($data['name'], $_POST[$data['name']]))
			{
				$selected = [$_POST[$data['name']]];
			}
		}
		elseif (isset($_POST[$data]))
		{
			$selected = [$_POST[$data]];
		}
	}

	$extra    = stringify_attributes($extra);
	$multiple = (count($selected) > 1 && stripos($extra, 'multiple') === false) ? ' multiple="multiple"' : '';
	$form     = '<select ' . rtrim(parse_form_attributes($data, $defaults)) . $extra . $multiple . ">\n";
	foreach ($options as $key => $val)
	{
		$key = (string) $key;
		if (is_array($val))
		{
			if (empty($val))
			{
				continue;
			}
			$form .= '<optgroup label="' . $key . "\">\n";
			foreach ($val as $optgroup_key => $optgroup_val)
			{
				$sel   = in_array($optgroup_key, $selected) ? ' selected="selected"' : '';
				$form .= '<option value="' . htmlspecialchars($optgroup_key) . '"' . $sel . '>'
						. $optgroup_val . "</option>\n";
			}
			$form .= "</optgroup>\n";
		}
		else
		{
			$form .= '<option value="' . htmlspecialchars($key) . '"'
					. (in_array($key, $selected) ? ' selected="selected"' : '') . '>'
					. $val . "</option>\n";
		}
	}

	return $form . "</select>\n";
}
```

</details>


<hr>

## form_checkbox()

```php
function form_checkbox($data = '', string $value = '', bool $checked = false, $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checkbox Field
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$checked</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 32 lines (458 - 489)</small></summary>

```php
function form_checkbox($data = '', string $value = '', bool $checked = false, $extra = ''): string
{
	$defaults = [
		'type'  => 'checkbox',
		'name'  => ( ! is_array($data) ? $data : ''),
		'value' => $value,
	];

	if (is_array($data) && array_key_exists('checked', $data))
	{
		$checked = $data['checked'];
		if ($checked === false)
		{
			unset($data['checked']);
		}
		else
		{
			$data['checked'] = 'checked';
		}
	}

	if ($checked === true)
	{
		$defaults['checked'] = 'checked';
	}
	else
	{
		unset($defaults['checked']);
	}

	return '<input ' . parse_form_attributes($data, $defaults) . stringify_attributes($extra) . " />\n";
}
```

</details>


<hr>

## form_radio()

```php
function form_radio($data = '', string $value = '', bool $checked = false, $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Radio Button
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$checked</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 7 lines (506 - 512)</small></summary>

```php
function form_radio($data = '', string $value = '', bool $checked = false, $extra = ''): string
{
	is_array($data) || $data = ['name' => $data];
	$data['type']            = 'radio';

	return form_checkbox($data, $value, $checked, $extra);
}
```

</details>


<hr>

## form_submit()

```php
function form_submit($data = '', string $value = '', $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Submit Button
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 10 lines (528 - 537)</small></summary>

```php
function form_submit($data = '', string $value = '', $extra = ''): string
{
	$defaults = [
		'type'  => 'submit',
		'name'  => is_array($data) ? '' : $data,
		'value' => $value,
	];

	return '<input ' . parse_form_attributes($data, $defaults) . stringify_attributes($extra) . " />\n";
}
```

</details>


<hr>

## form_reset()

```php
function form_reset($data = '', string $value = '', $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Reset Button
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 10 lines (553 - 562)</small></summary>

```php
function form_reset($data = '', string $value = '', $extra = ''): string
{
	$defaults = [
		'type'  => 'reset',
		'name'  => is_array($data) ? '' : $data,
		'value' => $value,
	];

	return '<input ' . parse_form_attributes($data, $defaults) . stringify_attributes($extra) . " />\n";
}
```

</details>


<hr>

## form_button()

```php
function form_button($data = '', string $content = '', $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Form Button
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$content</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$extra</code></td>
<td><em>mixed
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
<summary><small>Source: 17 lines (578 - 594)</small></summary>

```php
function form_button($data = '', string $content = '', $extra = ''): string
{
	$defaults = [
		'name' => is_array($data) ? '' : $data,
		'type' => 'button',
	];

	if (is_array($data) && isset($data['content']))
	{
		$content = $data['content'];
		unset($data['content']); // content is not an attribute
	}

	return '<button ' . parse_form_attributes($data, $defaults) . stringify_attributes($extra) . '>'
			. $content
			. "</button>\n";
}
```

</details>


<hr>

## form_label()

```php
function form_label(string $label_text = '', string $id = '', array $attributes = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Form Label Tag
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
<td><code>$label_text</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The text to appear onscreen</td>
</tr>

<tr>
<td>2.</td>
<td><code>$id</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The id the label applies to</td>
</tr>

<tr>
<td>3.</td>
<td><code>$attributes</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Additional attributes</td>
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
<summary><small>Source: 19 lines (610 - 628)</small></summary>

```php
function form_label(string $label_text = '', string $id = '', array $attributes = []): string
{
	$label = '<label';

	if ($id !== '')
	{
		$label .= ' for="' . $id . '"';
	}

	if (is_array($attributes) && $attributes)
	{
		foreach ($attributes as $key => $val)
		{
			$label .= ' ' . $key . '="' . $val . '"';
		}
	}

	return $label . '>' . $label_text . '</label>';
}
```

</details>


<hr>

## form_datalist()

```php
function form_datalist(string $name, string $value, array $options) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Datalist
</td></tr>
</table>

<table>
<tr><td>
The <datalist> element specifies a list of pre-defined options for an <input> element.
Users will see a drop-down list of pre-defined options as they input data.
The list attribute of the <input> element, must refer to the id attribute of the <datalist> element.
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

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$options</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 19 lines (648 - 666)</small></summary>

```php
function form_datalist(string $name, string $value, array $options): string
{
	$data = [
		'type'  => 'text',
		'name'  => $name,
		'list'  => $name . '_list',
		'value' => $value,
	];

	$out  = form_input($data) . "\n";
	$out .= "<datalist id='" . $name . '_list' . "'>";

	foreach ($options as $option)
	{
		$out .= "<option value='$option'>" . "\n";
	}

	return $out . ('</datalist>' . "\n");
}
```

</details>


<hr>

## form_fieldset()

```php
function form_fieldset(string $legend_text = '', array $attributes = array()) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fieldset Tag
</td></tr>
</table>

<table>
<tr><td>
Used to produce <fieldset><legend>text</legend>.  To close fieldset
use form_fieldset_close()
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
<td><code>$legend_text</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The legend text</td>
</tr>

<tr>
<td>2.</td>
<td><code>$attributes</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Additional attributes</td>
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
<summary><small>Source: 11 lines (684 - 694)</small></summary>

```php
function form_fieldset(string $legend_text = '', array $attributes = []): string
{
	$fieldset = '<fieldset' . stringify_attributes($attributes) . ">\n";

	if ($legend_text !== '')
	{
		return $fieldset . '<legend>' . $legend_text . "</legend>\n";
	}

	return $fieldset;
}
```

</details>


<hr>

## form_fieldset_close()

```php
function form_fieldset_close(string $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fieldset Close Tag
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
<td><code>$extra</code></td>
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
<summary><small>Source: 4 lines (708 - 711)</small></summary>

```php
function form_fieldset_close(string $extra = ''): string
{
	return '</fieldset>' . $extra;
}
```

</details>


<hr>

## form_close()

```php
function form_close(string $extra = '') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Form Close Tag
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
<td><code>$extra</code></td>
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
<summary><small>Source: 4 lines (725 - 728)</small></summary>

```php
function form_close(string $extra = ''): string
{
	return '</form>' . $extra;
}
```

</details>


<hr>

## set_value()

```php
function set_value(string $field, string $default = '', bool $html_escape = true) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Form Value
</td></tr>
</table>

<table>
<tr><td>
Grabs a value from the POST array for the specified field so you can
re-populate an input field or textarea
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
<td>Field name</td>
</tr>

<tr>
<td>2.</td>
<td><code>$default</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Default value</td>
</tr>

<tr>
<td>3.</td>
<td><code>$html_escape</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to escape HTML special characters or not</td>
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
<summary><small>Source: 14 lines (747 - 760)</small></summary>

```php
function set_value(string $field, string $default = '', bool $html_escape = true): string
{
	$request = Services::request();

	// Try any old input data we may have first
	$value = $request->getOldInput($field);

	if ($value === null)
	{
		$value = $request->getPost($field) ?? $default;
	}

	return ($html_escape) ? esc($value) : $value;
}
```

</details>


<hr>

## set_select()

```php
function set_select(string $field, string $value = '', bool $default = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Select
</td></tr>
</table>

<table>
<tr><td>
Let's you set the selected value of a <select> menu via data in the POST array.
If Form Validation is active it retrieves the info from the validation class
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
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$default</code></td>
<td><em>bool
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
<summary><small>Source: 33 lines (779 - 811)</small></summary>

```php
function set_select(string $field, string $value = '', bool $default = false): string
{
	$request = Services::request();

	// Try any old input data we may have first
	$input = $request->getOldInput($field);

	if ($input === null)
	{
		$input = $request->getPost($field);
	}

	if ($input === null)
	{
		return ($default === true) ? ' selected="selected"' : '';
	}

	if (is_array($input))
	{
		// Note: in_array('', array(0)) returns TRUE, do not use it
		foreach ($input as &$v)
		{
			if ($value === $v)
			{
				return ' selected="selected"';
			}
		}

		return '';
	}

	return ($input === $value) ? ' selected="selected"' : '';
}
```

</details>


<hr>

## set_checkbox()

```php
function set_checkbox(string $field, string $value = '', bool $default = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Checkbox
</td></tr>
</table>

<table>
<tr><td>
Let's you set the selected value of a checkbox via the value in the POST array.
If Form Validation is active it retrieves the info from the validation class
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
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$default</code></td>
<td><em>bool
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
<summary><small>Source: 34 lines (830 - 863)</small></summary>

```php
function set_checkbox(string $field, string $value = '', bool $default = false): string
{
	$request = Services::request();

	// Try any old input data we may have first
	$input = $request->getOldInput($field);

	if ($input === null)
	{
		$input = $request->getPost($field);
	}

	if (is_array($input))
	{
		// Note: in_array('', array(0)) returns TRUE, do not use it
		foreach ($input as &$v)
		{
			if ($value === $v)
			{
				return ' checked="checked"';
			}
		}

		return '';
	}

	// Unchecked checkbox and radio inputs are not even submitted by browsers ...
	if ((string) $input === '0' || ! empty($request->getPost()) || ! empty(old($field)))
	{
		return ($input === $value) ? ' checked="checked"' : '';
	}

	return ($default === true) ? ' checked="checked"' : '';
}
```

</details>


<hr>

## set_radio()

```php
function set_radio(string $field, string $value = '', bool $default = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Radio
</td></tr>
</table>

<table>
<tr><td>
Let's you set the selected value of a radio field via info in the POST array.
If Form Validation is active it retrieves the info from the validation class
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
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$default</code></td>
<td><em>bool
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
<summary><small>Source: 38 lines (882 - 919)</small></summary>

```php
function set_radio(string $field, string $value = '', bool $default = false): string
{
	$request = Services::request();

	// Try any old input data we may have first
	$input = $request->getOldInput($field);
	if ($input === null)
	{
		$input = $request->getPost($field) ?? $default;
	}

	if (is_array($input))
	{
		// Note: in_array('', array(0)) returns TRUE, do not use it
		foreach ($input as &$v)
		{
			if ($value === $v)
			{
				return ' checked="checked"';
			}
		}

		return '';
	}

	// Unchecked checkbox and radio inputs are not even submitted by browsers ...
	$result = '';
	if ((string) $input === '0' || ! empty($input = $request->getPost($field)) || ! empty($input = old($field)))
	{
		$result = ($input === $value) ? ' checked="checked"' : '';
	}

	if (empty($result))
	{
		$result = ($default === true) ? ' checked="checked"' : '';
	}
	return $result;
}
```

</details>


<hr>

## parse_form_attributes()

```php
function parse_form_attributes($attributes, array $default) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parse the form attributes
</td></tr>
</table>

<table>
<tr><td>
Helper function used by some of the form helpers
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
<td><code>$attributes</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>List of attributes</td>
</tr>

<tr>
<td>2.</td>
<td><code>$default</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Default values</td>
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
<summary><small>Source: 42 lines (936 - 977)</small></summary>

```php
function parse_form_attributes($attributes, array $default): string
{
	if (is_array($attributes))
	{
		foreach ($default as $key => $val)
		{
			if (isset($attributes[$key]))
			{
				$default[$key] = $attributes[$key];
				unset($attributes[$key]);
			}
		}
		if (! empty($attributes))
		{
			$default = array_merge($default, $attributes);
		}
	}

	$att = '';

	foreach ($default as $key => $val)
	{
		if (! is_bool($val))
		{
			if ($key === 'value')
			{
				$val = esc($val);
			}
			elseif ($key === 'name' && ! strlen($default['name']))
			{
				continue;
			}
			$att .= $key . '="' . $val . '" ';
		}
		else
		{
			$att .= $key . ' ';
		}
	}

	return $att;
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/form_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/filesystem_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/html_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:30**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>