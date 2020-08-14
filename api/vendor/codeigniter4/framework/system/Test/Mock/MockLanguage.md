


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockLanguage.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockIncomingRequest.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockLogger.md">next</a></td>
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
<a href="../../../../../../../api/vendor/codeigniter4/framework/system/Language/Language.md"><strong>CodeIgniter\Language\Language</strong></a>
</td>
<td>Language</td>
</tr>
</table>



 
## CodeIgniter\Test\Mock\MockLanguage

<table style="text-align:left">
<tr><th>Class</th><td>MockLanguage</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Test\Mock\MockLanguage</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Language/Language.md">CodeIgniter\Language\Language</a></td></tr>
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
<th><a href="#data"><strong>data</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Stores the data that should be
returned by the &#039;requireFile()&#039; method.</td>
</tr>

<tr>
<th><a href="#setData"><strong>setData</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the data that should be returned by the
&#039;requireFile()&#039; method to allow easy overrides
during testing.</td>
</tr>
<tr>
<th><a href="#requireFile"><strong>requireFile</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Provides an override that allows us to set custom
data to be returned easily during testing.</td>
</tr>
<tr>
<th><a href="#disableIntlSupport"><strong>disableIntlSupport</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Arbitrarily turnoff internationalization support for testing</td>
</tr>

</table>





### Properties


<hr>

#### $data

```php
protected $data;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Stores the data that should be
returned by the 'requireFile()' method.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>mixed
</td>
</tr>
</table>







### Methods


<hr>

#### setData()

```php
public function setData(string $file, array $data, string $locale = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the data that should be returned by the
'requireFile()' method to allow easy overrides
during testing.
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

<tr>
<td>2.</td>
<td><code>$file</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$locale</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (29 - 34)</small></summary>

```php
public function setData(string $file, array $data, string $locale = null)
{
	$this->language[$locale ?? $this->locale][$file] = $data;

	return $this;
}
```

</details>


<hr>

#### requireFile()

```php
protected function requireFile(string $path) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides an override that allows us to set custom
data to be returned easily during testing.
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
<td><code>$path</code></td>
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
<td>array<br>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (46 - 49)</small></summary>

```php
protected function requireFile(string $path): array
{
	return $this->data ?? [];
}
```

</details>


<hr>

#### disableIntlSupport()

```php
public function disableIntlSupport()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Arbitrarily turnoff internationalization support for testing
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (56 - 59)</small></summary>

```php
public function disableIntlSupport()
{
	$this->intlSupport = false;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockLanguage.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockIncomingRequest.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockLogger.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>