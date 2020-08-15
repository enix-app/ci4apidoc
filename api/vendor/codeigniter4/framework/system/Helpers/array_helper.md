


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/array_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/xml_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/date_helper.md">next</a></td>
</tr>
</table>




 



# Array Helper


<hr>

## dot_array_search()

```php
function dot_array_search(string $index, array $array)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Searches an array through dot syntax. Supports
wildcard searches, like foo.*.bar
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
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>mixed<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (57 - 62)</small></summary>

```php
function dot_array_search(string $index, array $array)
{
	$segments = explode('.', rtrim(rtrim($index, '* '), '.'));

	return _array_search_dot($segments, $array);
}
```

</details>


<hr>

## _array_search_dot()

```php
function _array_search_dot(array $indexes, array $array)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used by dot_array_search to recursively search the
array with wildcards.
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
<td><code>$indexes</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>mixed<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 46 lines (76 - 121)</small></summary>

```php
function _array_search_dot(array $indexes, array $array)
{
	// Grab the current index
	$currentIndex = $indexes
		? array_shift($indexes)
		: null;

	if ((empty($currentIndex)  && intval($currentIndex) !== 0) || (! isset($array[$currentIndex]) && $currentIndex !== '*'))
	{
		return null;
	}

	// Handle Wildcard (*)
	if ($currentIndex === '*')
	{
		// If $array has more than 1 item, we have to loop over each.
		foreach ($array as $value)
		{
			$answer = _array_search_dot($indexes, $value);

			if ($answer !== null)
			{
				return $answer;
			}
		}

		// Still here after searching all child nodes?
		return null;
	}

	// If this is the last index, make sure to return it now,
	// and not try to recurse through things.
	if (empty($indexes))
	{
		return $array[$currentIndex];
	}

	// Do we need to recursively search this value?
	if (is_array($array[$currentIndex]) && $array[$currentIndex])
	{
		return _array_search_dot($indexes, $array[$currentIndex]);
	}

	// Otherwise we've found our match!
	return $array[$currentIndex];
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/array_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/xml_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/date_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:06**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>