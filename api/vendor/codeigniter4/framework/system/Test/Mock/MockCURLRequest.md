


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockCURLRequest.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCLIConfig.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCache.md">next</a></td>
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/CURLRequest.md"><strong>CodeIgniter\HTTP\CURLRequest</strong></a>
</td>
<td>CURLRequest</td>
</tr>
</table>



 
## CodeIgniter\Test\Mock\MockCURLRequest

<table style="text-align:left">
<tr><th>Class</th><td>MockCURLRequest</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Test\Mock\MockCURLRequest</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/HTTP/CURLRequest.md">CodeIgniter\HTTP\CURLRequest</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class MockCURLRequest
</td></tr>
</table>

<table>
<tr><td>
Simply allows us to not actually call cURL during the
test runs. Instead, we can set the desired output
and get back the set options.
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
<th><a href="#curl_options"><strong>curl_options</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#output"><strong>output</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>

<tr>
<th><a href="#setOutput"><strong>setOutput</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#sendRequest"><strong>sendRequest</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#getBaseURI"><strong>getBaseURI</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#getDelay"><strong>getDelay</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>

</table>





### Properties


<hr>

#### $curl_options

```php
public $curl_options;
```






<hr>

#### $output

```php
protected $output = '';
```











### Methods


<hr>

#### setOutput()

```php
public function setOutput($output)
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
<td><code>$output</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 6 lines (20 - 25)</small></summary>

```php
public function setOutput($output)
{
	$this->output = $output;

	return $this;
}
```

</details>


<hr>

#### sendRequest()

```php
protected function sendRequest(array $curl_options = array()) : string
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
<td><code>$curl_options</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 7 lines (29 - 35)</small></summary>

```php
protected function sendRequest(array $curl_options = []): string
{
	// Save so we can access later.
	$this->curl_options = $curl_options;

	return $this->output;
}
```

</details>


<hr>

#### getBaseURI()

```php
public function getBaseURI()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (39 - 42)</small></summary>

```php
public function getBaseURI()
{
	return $this->baseURI;
}
```

</details>


<hr>

#### getDelay()

```php
public function getDelay()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (45 - 48)</small></summary>

```php
public function getDelay()
{
	return $this->delay;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockCURLRequest.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCLIConfig.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockCache.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:15**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>