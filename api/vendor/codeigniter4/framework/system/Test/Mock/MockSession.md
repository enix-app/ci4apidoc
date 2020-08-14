


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockSession.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockServices.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockTable.md">next</a></td>
</tr>
</table>







# CodeIgniter\Test\Mock 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Test\Mock</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockAppConfig.md">CodeIgniter\Test\Mock\MockAppConfig</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockAutoload.md">CodeIgniter\Test\Mock\MockAutoload</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockBuilder.md">CodeIgniter\Test\Mock\MockBuilder</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCLIConfig.md">CodeIgniter\Test\Mock\MockCLIConfig</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCURLRequest.md">CodeIgniter\Test\Mock\MockCURLRequest</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCache.md">CodeIgniter\Test\Mock\MockCache</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCodeIgniter.md">CodeIgniter\Test\Mock\MockCodeIgniter</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockConnection.md">CodeIgniter\Test\Mock\MockConnection</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockEmail.md">CodeIgniter\Test\Mock\MockEmail</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockEvents.md">CodeIgniter\Test\Mock\MockEvents</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockFileLogger.md">CodeIgniter\Test\Mock\MockFileLogger</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockIncomingRequest.md">CodeIgniter\Test\Mock\MockIncomingRequest</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockLanguage.md">CodeIgniter\Test\Mock\MockLanguage</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockLogger.md">CodeIgniter\Test\Mock\MockLogger</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockQuery.md">CodeIgniter\Test\Mock\MockQuery</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockResourceController.md">CodeIgniter\Test\Mock\MockResourceController</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockResourcePresenter.md">CodeIgniter\Test\Mock\MockResourcePresenter</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockResponse.md">CodeIgniter\Test\Mock\MockResponse</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockResult.md">CodeIgniter\Test\Mock\MockResult</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockSecurity.md">CodeIgniter\Test\Mock\MockSecurity</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockServices.md">CodeIgniter\Test\Mock\MockServices</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockSession.md">CodeIgniter\Test\Mock\MockSession</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockTable.md">CodeIgniter\Test\Mock\MockTable</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Session.md"><strong>CodeIgniter\Session\Session</strong></a>
</td>
<td>Session</td>
</tr>
</table>



 
## CodeIgniter\Test\Mock\MockSession

<table style="text-align:left">
<tr><th>Class</th><td>MockSession</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Test\Mock\MockSession</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Session/Session.md">CodeIgniter\Session\Session</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class MockSession
</td></tr>
</table>

<table>
<tr><td>
Provides a safe way to test the Session class itself,
that doesn't interact with the session or cookies at all.
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
<th><a href="#cookies"><strong>cookies</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Holds our &quot;cookie&quot; data.</td>
</tr>
<tr>
<th><a href="#didRegenerate"><strong>didRegenerate</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td></td>
</tr>

<tr>
<th><a href="#setSaveHandler"><strong>setSaveHandler</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Sets the driver as the session handler in PHP.</td>
</tr>
<tr>
<th><a href="#startSession"><strong>startSession</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Starts the session.</td>
</tr>
<tr>
<th><a href="#setCookie"><strong>setCookie</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Takes care of setting the cookie on the client side.</td>
</tr>
<tr>
<th><a href="#regenerate"><strong>regenerate</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>

</table>





### Properties


<hr>

#### $cookies

```php
public $cookies = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Holds our "cookie" data.
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

#### $didRegenerate

```php
public $didRegenerate = false;
```











### Methods


<hr>

#### setSaveHandler()

```php
protected function setSaveHandler()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the driver as the session handler in PHP.
</td></tr>
</table>

<table>
<tr><td>
Extracted for easier testing.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (28 - 31)</small></summary>

```php
protected function setSaveHandler()
{
	//        session_set_save_handler($this->driver, true);
}
```

</details>


<hr>

#### startSession()

```php
protected function startSession()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Starts the session.
</td></tr>
</table>

<table>
<tr><td>
Extracted for testing reasons.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (39 - 42)</small></summary>

```php
protected function startSession()
{
	//        session_start();
}
```

</details>


<hr>

#### setCookie()

```php
protected function setCookie()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes care of setting the cookie on the client side.
</td></tr>
</table>

<table>
<tr><td>
Extracted for testing reasons.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 12 lines (50 - 61)</small></summary>

```php
protected function setCookie()
{
	$this->cookies[] = [
		$this->sessionCookieName,
		session_id(),
		(empty($this->sessionExpiration) ? 0 : time() + $this->sessionExpiration),
		$this->cookiePath,
		$this->cookieDomain,
		$this->cookieSecure,
		true,
	];
}
```

</details>


<hr>

#### regenerate()

```php
public function regenerate(bool $destroy = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


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
<td><code>$destroy</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 5 lines (65 - 69)</small></summary>

```php
public function regenerate(bool $destroy = false)
{
	$this->didRegenerate              = true;
	$_SESSION['__ci_last_regenerate'] = time();
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockSession.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockServices.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockTable.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>