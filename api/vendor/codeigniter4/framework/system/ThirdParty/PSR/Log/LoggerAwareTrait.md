


 



<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/PSR/Log/LoggerAwareTrait.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerAwareInterface.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerInterface.md">next</a></td>
</tr>
</table>







# Psr\Log 
<table style="text-align:left">
<tr><th>namespace</th><td>Psr\Log</td></tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/AbstractLogger.md">Psr\Log\AbstractLogger</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/InvalidArgumentException.md">Psr\Log\InvalidArgumentException</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LogLevel.md">Psr\Log\LogLevel</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerAwareInterface.md">Psr\Log\LoggerAwareInterface</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerAwareTrait.md">Psr\Log\LoggerAwareTrait</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerInterface.md">Psr\Log\LoggerInterface</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerTrait.md">Psr\Log\LoggerTrait</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/NullLogger.md">Psr\Log\NullLogger</a></td></tr>
</table>
</details>



 

 
## Psr\Log\LoggerAwareTrait

<table style="text-align:left">
<tr><th>Trait</th><td>LoggerAwareTrait</td></tr>
<tr><th>Fully Qualified Name</th><td>Psr\Log\LoggerAwareTrait</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Basic Implementation of LoggerAwareInterface.
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
<th><a href="#logger"><strong>logger</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>

<tr>
<th><a href="#setLogger"><strong>setLogger</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets a logger.</td>
</tr>

</table>





### Properties


<hr>

#### $logger

```php
protected $logger;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\LoggerInterface
</td>
</tr>
</table>







### Methods


<hr>

#### setLogger()

```php
public function setLogger(LoggerInterface $logger)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets a logger.
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
<td><code>$logger</code></td>
<td><em>\LoggerInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (18 - 21)</small></summary>

```php
public function setLogger(LoggerInterface $logger)
{
    $this->logger = $logger;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/PSR/Log/LoggerAwareTrait.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerAwareInterface.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>