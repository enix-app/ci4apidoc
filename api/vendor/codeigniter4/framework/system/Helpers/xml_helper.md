


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/xml_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/text_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/array_helper.md">next</a></td>
</tr>
</table>




 



# XML Helper


<hr>

## xml_convert()

```php
function xml_convert(string $str, bool $protect_all = false) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Convert Reserved XML characters to Entities
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
<td><code>$protect_all</code></td>
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
<summary><small>Source: 43 lines (55 - 97)</small></summary>

```php
function xml_convert(string $str, bool $protect_all = false): string
{
	$temp = '__TEMP_AMPERSANDS__';

	// Replace entities to temporary markers so that
	// ampersands won't get messed up
	$str = preg_replace('/&#(\d+);/', $temp . '\\1;', $str);

	if ($protect_all === true)
	{
		$str = preg_replace('/&(\w+);/', $temp . '\\1;', $str);
	}

	$original = [
		'&',
		'<',
		'>',
		'"',
		"'",
		'-',
	];

	$replacement = [
		'&amp;',
		'&lt;',
		'&gt;',
		'&quot;',
		'&apos;',
		'&#45;',
	];

	$str = str_replace($original, $replacement, $str);

	// Decode the temp markers back to entities
	$str = preg_replace('/' . $temp . '(\d+);/', '&#\\1;', $str);

	if ($protect_all === true)
	{
		return preg_replace('/' . $temp . '(\w+);/', '&\\1;', $str);
	}

	return $str;
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/xml_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/text_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/array_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:06**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>