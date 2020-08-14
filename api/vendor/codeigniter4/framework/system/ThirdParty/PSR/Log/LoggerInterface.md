


 



<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/PSR/Log/LoggerInterface.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerAwareTrait.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerTrait.md">next</a></td>
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



 

 
## Psr\Log\LoggerInterface

<table style="text-align:left">
<tr><th>Interface</th><td>LoggerInterface</td></tr>
<tr><th>Fully Qualified Name</th><td>Psr\Log\LoggerInterface</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Describes a logger instance
</td></tr>
</table>

<table>
<tr><td>
The message MUST be a string or object implementing __toString().

The message MAY contain placeholders in the form: {foo} where foo
will be replaced by the context data in key "foo".

The context array can contain arbitrary data, the only assumption that
can be made by implementors is that if an Exception instance is given
to produce a stack trace, it MUST be in a key named "exception".

See <a href="https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-3-logger-interface.md">https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-3-logger-interface.md</a>
for the full interface specification.
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
<th><a href="#emergency"><strong>emergency</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>System is unusable.</td>
</tr>
<tr>
<th><a href="#alert"><strong>alert</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Action must be taken immediately.</td>
</tr>
<tr>
<th><a href="#critical"><strong>critical</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Critical conditions.</td>
</tr>
<tr>
<th><a href="#error"><strong>error</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Runtime errors that do not require immediate action but should typically
be logged and monitored.</td>
</tr>
<tr>
<th><a href="#warning"><strong>warning</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Exceptional occurrences that are not errors.</td>
</tr>
<tr>
<th><a href="#notice"><strong>notice</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Normal but significant events.</td>
</tr>
<tr>
<th><a href="#info"><strong>info</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Interesting events.</td>
</tr>
<tr>
<th><a href="#debug"><strong>debug</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Detailed debug information.</td>
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

#### emergency()

```php
public function emergency($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
System is unusable.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<summary><small>Source: line 27</small></summary>

```php
public function emergency($message, array $context = []);
```

</details>


<hr>

#### alert()

```php
public function alert($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Action must be taken immediately.
</td></tr>
</table>

<table>
<tr><td>
Example: Entire website down, database unavailable, etc. This should
trigger the SMS alerts and wake you up.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<summary><small>Source: line 39</small></summary>

```php
public function alert($message, array $context = []);
```

</details>


<hr>

#### critical()

```php
public function critical($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Critical conditions.
</td></tr>
</table>

<table>
<tr><td>
Example: Application component unavailable, unexpected exception.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<summary><small>Source: line 50</small></summary>

```php
public function critical($message, array $context = []);
```

</details>


<hr>

#### error()

```php
public function error($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Runtime errors that do not require immediate action but should typically
be logged and monitored.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<summary><small>Source: line 60</small></summary>

```php
public function error($message, array $context = []);
```

</details>


<hr>

#### warning()

```php
public function warning($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Exceptional occurrences that are not errors.
</td></tr>
</table>

<table>
<tr><td>
Example: Use of deprecated APIs, poor use of an API, undesirable things
that are not necessarily wrong.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<summary><small>Source: line 72</small></summary>

```php
public function warning($message, array $context = []);
```

</details>


<hr>

#### notice()

```php
public function notice($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Normal but significant events.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<summary><small>Source: line 81</small></summary>

```php
public function notice($message, array $context = []);
```

</details>


<hr>

#### info()

```php
public function info($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Interesting events.
</td></tr>
</table>

<table>
<tr><td>
Example: User logs in, SQL logs.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<summary><small>Source: line 92</small></summary>

```php
public function info($message, array $context = []);
```

</details>


<hr>

#### debug()

```php
public function debug($message, array $context = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Detailed debug information.
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
<td><code>$message</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<summary><small>Source: line 101</small></summary>

```php
public function debug($message, array $context = []);
```

</details>


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
<summary><small>Source: line 111</small></summary>

```php
public function log($level, $message, array $context = []);
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/PSR/Log/LoggerInterface.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerAwareTrait.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/PSR/Log/LoggerTrait.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>