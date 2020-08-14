


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/cookie_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/number_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/cookie_helper.md">next</a></td>
</tr>
</table>




 



# Cookie Helper


<hr>

## set_cookie()

```php
function set_cookie($name, string $value = '', string $expire = '', string $domain = '', string $path = '/', string $prefix = '', bool $secure = false, bool $httpOnly = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set cookie
</td></tr>
</table>

<table>
<tr><td>
Accepts seven parameters, or you can submit an associative
array in the first parameter containing all the values.
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
<td>Cookie name or array containing binds</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The value of the cookie</td>
</tr>

<tr>
<td>3.</td>
<td><code>$expire</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The number of seconds until expiration</td>
</tr>

<tr>
<td>4.</td>
<td><code>$domain</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>For site-wide cookie.
Usually: .yourdomain.com</td>
</tr>

<tr>
<td>5.</td>
<td><code>$path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The cookie path</td>
</tr>

<tr>
<td>6.</td>
<td><code>$prefix</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The cookie prefix</td>
</tr>

<tr>
<td>7.</td>
<td><code>$secure</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>True makes the cookie secure</td>
</tr>

<tr>
<td>8.</td>
<td><code>$httpOnly</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>True makes the cookie accessible via
http(s) only (no javascript)</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 7 lines (69 - 75)</small></summary>

```php
function set_cookie($name, string $value = '', string $expire = '', string $domain = '', string $path = '/', string $prefix = '', bool $secure = false, bool $httpOnly = false)
{
	// The following line shows as a syntax error in NetBeans IDE
	//(\Config\Services::response())->setcookie
	$response = \Config\Services::response();
	$response->setcookie($name, $value, $expire, $domain, $path, $prefix, $secure, $httpOnly);
}
```

</details>


<hr>

## get_cookie()

```php
function get_cookie($index, bool $xssClean = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetch an item from the COOKIE array
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
<td><code>$xssClean</code></td>
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





<details>
<summary><small>Source: 11 lines (93 - 103)</small></summary>

```php
function get_cookie($index, bool $xssClean = false)
{
	$app             = config(\Config\App::class);
	$appCookiePrefix = $app->cookiePrefix;
	$prefix          = isset($_COOKIE[$index]) ? '' : $appCookiePrefix;

	$request = \Config\Services::request();
	$filter  = true === $xssClean ? FILTER_SANITIZE_STRING : null;

	return $request->getCookie($prefix . $index, $filter);
}
```

</details>


<hr>

## delete_cookie()

```php
function delete_cookie($name, string $domain = '', string $path = '/', string $prefix = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Delete a COOKIE
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
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$domain</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the cookie domain. Usually: .yourdomain.com</td>
</tr>

<tr>
<td>3.</td>
<td><code>$path</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the cookie path</td>
</tr>

<tr>
<td>4.</td>
<td><code>$prefix</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>the cookie prefix</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (123 - 126)</small></summary>

```php
function delete_cookie($name, string $domain = '', string $path = '/', string $prefix = '')
{
	\Config\Services::response()->deleteCookie($name, $domain, $path, $prefix);
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/cookie_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/number_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/cookie_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:07**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>