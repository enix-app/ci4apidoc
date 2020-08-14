


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/test_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCommon.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/security_helper.md">next</a></td>
</tr>
</table>




 



# Test Helper


<hr>

## fake()

```php
function fake($model, array $overrides = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Creates a single item using Fabricator.
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
<td><code>$model</code></td>
<td><em>\Model<br>object<br>string
</em></td>
<td>false</td>
<td>Instance or name of the model</td>
</tr>

<tr>
<td>2.</td>
<td><code>$overrides</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td>Overriding data to pass to Fabricator::setOverrides()</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>object<br>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 13 lines (60 - 72)</small></summary>

```php
function fake($model, array $overrides = null)
{
	// Get a model-appropriate Fabricator instance
	$fabricator = new Fabricator($model);

	// Set overriding data, if necessary
	if ($overrides)
	{
		$fabricator->setOverrides($overrides);
	}

	return $fabricator->create();
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/test_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCommon.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/security_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:24**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>