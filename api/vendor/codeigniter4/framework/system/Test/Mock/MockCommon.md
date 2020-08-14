


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockCommon.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Common.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Helpers/test_helper.md">next</a></td>
</tr>
</table>




 



# MockCommon


<hr>

## is_cli()

```php
function is_cli(bool $new_return = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Is CLI?
</td></tr>
</table>

<table>
<tr><td>
Test to see if a request was made from the command line.
You can set the return value for testing.
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
<td><code>$new_return</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>return value to set</td>
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
<summary><small>Source: 12 lines (23 - 34)</small></summary>

```php
function is_cli(bool $new_return = null): bool
{
	// PHPUnit always runs via CLI.
	static $return_value = true;

	if ($new_return !== null)
	{
		$return_value = $new_return;
	}

	return $return_value;
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockCommon.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Common.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Helpers/test_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:24**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>