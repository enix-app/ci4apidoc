


 



<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/PSR/Log/NullLogger.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerTrait.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Common.md">next</a></td>
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



 

 
## Psr\Log\NullLogger

<table style="text-align:left">
<tr><th>Class</th><td>NullLogger</td></tr>
<tr><th>Fully Qualified Name</th><td>Psr\Log\NullLogger</td></tr>
<tr><th>Extends</th><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/AbstractLogger.md">Psr\Log\AbstractLogger</a></td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
This Logger can be used to avoid conditional log calls
</td></tr>
</table>

<table>
<tr><td>
Logging should always be optional, and if no logger is provided to your
library creating a NullLogger instance to have something to throw logs at
is a good way to avoid littering your code with `if ($this->logger) { }`
blocks.
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
<th><a href="#log"><strong>log</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Logs with an arbitrary level.</td>
</tr>

</table>






### Methods


<hr>

#### log()

```php
public function log($level, $message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Logs with an arbitrary level.
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
<td><code>$level</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$context</code></td>
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
<td>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (23 - 26)</small></summary>

```php
public function log($level, $message, array $context = [])
{
    // noop
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/PSR/Log/NullLogger.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerTrait.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/Common.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>