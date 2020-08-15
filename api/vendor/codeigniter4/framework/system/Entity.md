


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Entity.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/OpenSSLHandler.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Events/Events.md">next</a></td>
</tr>
</table>







# CodeIgniter 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter</td></tr>
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
<td>framework/system/Entity.php
</td>
</tr>
</table>

 


 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Exceptions/CastException.md"><strong>CodeIgniter\Exceptions\CastException</strong></a>
</td>
<td>CastException</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/I18n/Time.md"><strong>CodeIgniter\I18n\Time</strong></a>
</td>
<td>Time</td>
</tr>
</table>



 
## CodeIgniter\Entity

<table style="text-align:left">
<tr><th>Class</th><td>Entity</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Entity</td></tr>
<tr><th>Implements</th>
<td>
<a href="">CodeIgniter\JsonSerializable</a><br>
</td>
</tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Entity encapsulation, for use with CodeIgniter\Model
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
<th><a href="#datamap"><strong>datamap</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Maps names used in sets and gets against unique
names within the class, allowing independence from
database column names.</td>
</tr>
<tr>
<th><a href="#dates"><strong>dates</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#casts"><strong>casts</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Array of field names and the type of value to cast them as
when they are accessed.</td>
</tr>
<tr>
<th><a href="#attributes"><strong>attributes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Holds the current values of all class vars.</td>
</tr>
<tr>
<th><a href="#original"><strong>original</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Holds original copies of all class vars so
we can determine what&#039;s actually been changed
and not accidentally write nulls where we shouldn&#039;t.</td>
</tr>
<tr>
<th><a href="#_cast"><strong>_cast</strong></a></th>
<td>prop</td>
<td>
private

</td>
<td>Holds info whenever properties have to be casted</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows filling in Entity parameters during construction.</td>
</tr>
<tr>
<th><a href="#fill"><strong>fill</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Takes an array of key/value pairs and sets them as
class properties, using any `setCamelCasedProperty()` methods
that may or may not exist.</td>
</tr>
<tr>
<th><a href="#toArray"><strong>toArray</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>General method that will return all public and protected
values of this entity as an array. All values are accessed
through the __get() magic method so will have any casts, etc
applied to them.</td>
</tr>
<tr>
<th><a href="#toRawArray"><strong>toRawArray</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the raw values of the current attributes.</td>
</tr>
<tr>
<th><a href="#syncOriginal"><strong>syncOriginal</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Ensures our &quot;original&quot; values match the current values.</td>
</tr>
<tr>
<th><a href="#hasChanged"><strong>hasChanged</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks a property to see if it has changed since the entity was created.</td>
</tr>
<tr>
<th><a href="#__get"><strong>__get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Magic method to allow retrieval of protected and private
class properties either by their name, or through a `getCamelCasedProperty()`
method.</td>
</tr>
<tr>
<th><a href="#__set"><strong>__set</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Magic method to all protected/private class properties to be easily set,
either through a direct access or a `setCamelCasedProperty()` method.</td>
</tr>
<tr>
<th><a href="#__unset"><strong>__unset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Unsets an attribute property.</td>
</tr>
<tr>
<th><a href="#__isset"><strong>__isset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns true if a property exists names $key, or a getter method
exists named like for __get().</td>
</tr>
<tr>
<th><a href="#setAttributes"><strong>setAttributes</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set raw data array without any mutations</td>
</tr>
<tr>
<th><a href="#mapProperty"><strong>mapProperty</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Checks the datamap to see if this column name is being mapped,
and returns the mapped name, if any, or the original name.</td>
</tr>
<tr>
<th><a href="#mutateDate"><strong>mutateDate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Converts the given string|timestamp|DateTime|Time instance
into a \CodeIgniter\I18n\Time object.</td>
</tr>
<tr>
<th><a href="#castAs"><strong>castAs</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Provides the ability to cast an item as a specific data type.</td>
</tr>
<tr>
<th><a href="#castAsJson"><strong>castAsJson</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Cast as JSON</td>
</tr>
<tr>
<th><a href="#jsonSerialize"><strong>jsonSerialize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Support for json_encode()</td>
</tr>

</table>





### Properties


<hr>

#### $datamap

```php
protected $datamap = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Maps names used in sets and gets against unique
names within the class, allowing independence from
database column names.
</td></tr>
</table>

<table>
<tr><td>
Example:
$datamap = [
    'db_name' => 'class_name'
];
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>






<hr>

#### $dates

```php
protected $dates = [
	'created_at',
	'updated_at',
	'deleted_at',
];
```






<hr>

#### $casts

```php
protected $casts = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Array of field names and the type of value to cast them as
when they are accessed.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>






<hr>

#### $attributes

```php
protected $attributes = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Holds the current values of all class vars.
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

#### $original

```php
protected $original = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Holds original copies of all class vars so
we can determine what's actually been changed
and not accidentally write nulls where we shouldn't.
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

#### $_cast

```php
private $_cast = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Holds info whenever properties have to be casted
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
public function __construct(array $data = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows filling in Entity parameters during construction.
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
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 6 lines (102 - 107)</small></summary>

```php
public function __construct(array $data = null)
{
	$this->syncOriginal();

	$this->fill($data);
}
```

</details>


<hr>

#### fill()

```php
public function fill(array $data = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes an array of key/value pairs and sets them as
class properties, using any `setCamelCasedProperty()` methods
that may or may not exist.
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
<td>\CodeIgniter\Entity
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (118 - 131)</small></summary>

```php
public function fill(array $data = null)
{
	if (! is_array($data))
	{
		return $this;
	}

	foreach ($data as $key => $value)
	{
		$this->__set($key, $value);
	}

	return $this;
}
```

</details>


<hr>

#### toArray()

```php
public function toArray(bool $onlyChanged = false, bool $cast = true) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
General method that will return all public and protected
values of this entity as an array. All values are accessed
through the __get() magic method so will have any casts, etc
applied to them.
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
<td><code>$onlyChanged</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>If true, only return values that have changed since object creation</td>
</tr>

<tr>
<td>2.</td>
<td><code>$cast</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>If true, properties will be casted.</td>
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 37 lines (147 - 183)</small></summary>

```php
public function toArray(bool $onlyChanged = false, bool $cast = true): array
{
	$this->_cast = $cast;
	$return      = [];

	// we need to loop over our properties so that we
	// allow our magic methods a chance to do their thing.
	foreach ($this->attributes as $key => $value)
	{
		if (strpos($key, '_') === 0)
		{
			continue;
		}

		if ($onlyChanged && ! $this->hasChanged($key))
		{
			continue;
		}

		$return[$key] = $this->__get($key);
	}

	// Loop over our mapped properties and add them to the list...
	if (is_array($this->datamap))
	{
		foreach ($this->datamap as $from => $to)
		{
			if (array_key_exists($to, $return))
			{
				$return[$from] = $this->__get($to);
			}
		}
	}

	$this->_cast = true;
	return $return;
}
```

</details>


<hr>

#### toRawArray()

```php
public function toRawArray(bool $onlyChanged = false) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the raw values of the current attributes.
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
<td><code>$onlyChanged</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 21 lines (194 - 214)</small></summary>

```php
public function toRawArray(bool $onlyChanged = false): array
{
	$return = [];

	if (! $onlyChanged)
	{
		return $this->attributes;
	}

	foreach ($this->attributes as $key => $value)
	{
		if (! $this->hasChanged($key))
		{
			continue;
		}

		$return[$key] = $this->attributes[$key];
	}

	return $return;
}
```

</details>


<hr>

#### syncOriginal()

```php
public function syncOriginal()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ensures our "original" values match the current values.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (223 - 228)</small></summary>

```php
public function syncOriginal()
{
	$this->original = $this->attributes;

	return $this;
}
```

</details>


<hr>

#### hasChanged()

```php
public function hasChanged(string $key = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks a property to see if it has changed since the entity was created.
</td></tr>
</table>

<table>
<tr><td>
Or, without a parameter, checks if any properties have changed.
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
<td><code>$key</code></td>
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
<summary><small>Source: 22 lines (238 - 259)</small></summary>

```php
public function hasChanged(string $key = null): bool
{
	// If no parameter was given then check all attributes
	if ($key === null)
	{
		return     $this->original !== $this->attributes;
	}

	// Key doesn't exist in either
	if (! array_key_exists($key, $this->original) && ! array_key_exists($key, $this->attributes))
	{
		return false;
	}

	// It's a new element
	if (! array_key_exists($key, $this->original) && array_key_exists($key, $this->attributes))
	{
		return true;
	}

	return $this->original[$key] !== $this->attributes[$key];
}
```

</details>


<hr>

#### __get()

```php
public function __get(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Magic method to allow retrieval of protected and private
class properties either by their name, or through a `getCamelCasedProperty()`
method.
</td></tr>
</table>

<table>
<tr><td>
Examples:

$p = $this->my_property
$p = $this->getMyProperty()
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
<td><code>$key</code></td>
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
<td>mixed
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
<summary><small>Source: 35 lines (276 - 310)</small></summary>

```php
public function __get(string $key)
{
	$key    = $this->mapProperty($key);
	$result = null;

	// Convert to CamelCase for the method
	$method = 'get' . str_replace(' ', '', ucwords(str_replace(['-', '_'], ' ', $key)));

	// if a set* method exists for this key,
	// use that method to insert this value.
	if (method_exists($this, $method))
	{
		$result = $this->$method();
	}

	// Otherwise return the protected property
	// if it exists.
	else if (array_key_exists($key, $this->attributes))
	{
		$result = $this->attributes[$key];
	}

	// Do we need to mutate this into a date?
	if (in_array($key, $this->dates))
	{
		$result = $this->mutateDate($result);
	}
	// Or cast it as something?
	else if ($this->_cast && ! empty($this->casts[$key]))
	{
		$result = $this->castAs($result, $this->casts[$key]);
	}

	return $result;
}
```

</details>


<hr>

#### __set()

```php
public function __set(string $key, $value = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Magic method to all protected/private class properties to be easily set,
either through a direct access or a `setCamelCasedProperty()` method.
</td></tr>
</table>

<table>
<tr><td>
Examples:

$this->my_property = $p;
$this->setMyProperty() = $p;
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
<td><code>$key</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>null
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception
</td>
</tr>
</table>



<details>
<summary><small>Source: 64 lines (329 - 392)</small></summary>

```php
public function __set(string $key, $value = null)
{
	$key = $this->mapProperty($key);

	// Check if the field should be mutated into a date
	if (in_array($key, $this->dates))
	{
		$value = $this->mutateDate($value);
	}

	$isNullable = false;
	$castTo     = false;

	if (array_key_exists($key, $this->casts))
	{
		$isNullable = strpos($this->casts[$key], '?') === 0;
		$castTo     = $isNullable ? substr($this->casts[$key], 1) : $this->casts[$key];
	}

	if (! $isNullable || ! is_null($value))
	{
		// Array casting requires that we serialize the value
		// when setting it so that it can easily be stored
		// back to the database.
		if ($castTo === 'array')
		{
			$value = serialize($value);
		}

		// JSON casting requires that we JSONize the value
		// when setting it so that it can easily be stored
		// back to the database.
		if (($castTo === 'json' || $castTo === 'json-array') && function_exists('json_encode'))
		{
			$value = json_encode($value, JSON_UNESCAPED_UNICODE);

			if (json_last_error() !== JSON_ERROR_NONE)
			{
				throw CastException::forInvalidJsonFormatException(json_last_error());
			}
		}
	}

	// if a set* method exists for this key,
	// use that method to insert this value.
	// *) should be outside $isNullable check - SO maybe wants to do sth with null value automatically
	$method = 'set' . str_replace(' ', '', ucwords(str_replace(['-', '_'], ' ', $key)));
	if (method_exists($this, $method))
	{
		$this->$method($value);

		return $this;
	}

	// Otherwise, just the value.
	// This allows for creation of new class
	// properties that are undefined, though
	// they cannot be saved. Useful for
	// grabbing values through joins,
	// assigning relationships, etc.
	$this->attributes[$key] = $value;

	return $this;
}
```

</details>


<hr>

#### __unset()

```php
public function __unset(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Unsets an attribute property.
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
<td><code>$key</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 4 lines (403 - 406)</small></summary>

```php
public function __unset(string $key)
{
	unset($this->attributes[$key]);
}
```

</details>


<hr>

#### __isset()

```php
public function __isset(string $key) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns true if a property exists names $key, or a getter method
exists named like for __get().
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
<td><code>$key</code></td>
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
<summary><small>Source: 13 lines (418 - 430)</small></summary>

```php
public function __isset(string $key): bool
{
	$key = $this->mapProperty($key);

	$method = 'get' . str_replace(' ', '', ucwords(str_replace(['-', '_'], ' ', $key)));

	if (method_exists($this, $method))
	{
		return true;
	}

	return isset($this->attributes[$key]);
}
```

</details>


<hr>

#### setAttributes()

```php
public function setAttributes(array $data)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set raw data array without any mutations
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (438 - 443)</small></summary>

```php
public function setAttributes(array $data)
{
	$this->attributes = $data;
	$this->syncOriginal();
	return $this;
}
```

</details>


<hr>

#### mapProperty()

```php
protected function mapProperty(string $key)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks the datamap to see if this column name is being mapped,
and returns the mapped name, if any, or the original name.
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
<td><code>$key</code></td>
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
<td>mixed<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 14 lines (455 - 468)</small></summary>

```php
protected function mapProperty(string $key)
{
	if (empty($this->datamap))
	{
		return $key;
	}

	if (! empty($this->datamap[$key]))
	{
		return $this->datamap[$key];
	}

	return $key;
}
```

</details>


<hr>

#### mutateDate()

```php
protected function mutateDate($value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts the given string|timestamp|DateTime|Time instance
into a \CodeIgniter\I18n\Time object.
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
<td>\CodeIgniter\I18n\Time
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
<summary><small>Source: 24 lines (481 - 504)</small></summary>

```php
protected function mutateDate($value)
{
	if ($value instanceof Time)
	{
		return $value;
	}

	if ($value instanceof \DateTime)
	{
		return Time::instance($value);
	}

	if (is_numeric($value))
	{
		return Time::createFromTimestamp($value);
	}

	if (is_string($value))
	{
		return Time::parse($value);
	}

	return $value;
}
```

</details>


<hr>

#### castAs()

```php
protected function castAs($value, string $type)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides the ability to cast an item as a specific data type.
</td></tr>
</table>

<table>
<tr><td>
Add ? at the beginning of $type  (i.e. ?string) to get NULL instead of casting $value if $value === null
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
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>mixed
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
<summary><small>Source: 55 lines (519 - 573)</small></summary>

```php
protected function castAs($value, string $type)
{
	if (strpos($type, '?') === 0)
	{
		if ($value === null)
		{
			return null;
		}
		$type = substr($type, 1);
	}

	switch($type)
	{
		case 'int':
		case 'integer': //alias for 'integer'
			$value = (int)$value;
			break;
		case 'float':
			$value = (float)$value;
			break;
		case 'double':
			$value = (double)$value;
			break;
		case 'string':
			$value = (string)$value;
			break;
		case 'bool':
		case 'boolean': //alias for 'boolean'
			$value = (bool)$value;
			break;
		case 'object':
			$value = (object)$value;
			break;
		case 'array':
			if (is_string($value) && (strpos($value, 'a:') === 0 || strpos($value, 's:') === 0))
			{
				$value = unserialize($value);
			}

			$value = (array)$value;
			break;
		case 'json':
			$value = $this->castAsJson($value);
			break;
		case 'json-array':
			$value = $this->castAsJson($value, true);
			break;
		case 'datetime':
			return $this->mutateDate($value);
		case 'timestamp':
			return strtotime($value);
	}

	return $value;
}
```

</details>


<hr>

#### castAsJson()

```php
private function castAsJson($value, bool $asArray = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Cast as JSON
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
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$asArray</code></td>
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
<td>mixed
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Exceptions\CastException
</td>
</tr>
</table>



<details>
<summary><small>Source: 17 lines (586 - 602)</small></summary>

```php
private function castAsJson($value, bool $asArray = false)
{
	$tmp = ! is_null($value) ? ($asArray ? [] : new \stdClass) : null;
	if (function_exists('json_decode'))
	{
		if ((is_string($value) && strlen($value) > 1 && in_array($value[0], ['[', '{', '"'])) || is_numeric($value))
		{
			$tmp = json_decode($value, $asArray);

			if (json_last_error() !== JSON_ERROR_NONE)
			{
				throw CastException::forInvalidJsonFormatException(json_last_error());
			}
		}
	}
	return $tmp;
}
```

</details>


<hr>

#### jsonSerialize()

```php
public function jsonSerialize()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Support for json_encode()
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>mixed
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
<summary><small>Source: 4 lines (610 - 613)</small></summary>

```php
public function jsonSerialize()
{
	return $this->toArray();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Entity.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Encryption/Handlers/OpenSSLHandler.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Events/Events.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>