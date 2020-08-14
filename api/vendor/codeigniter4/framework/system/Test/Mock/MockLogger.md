


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockLogger.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockLanguage.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockQuery.md">next</a></td>
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



 

 
## CodeIgniter\Test\Mock\MockLogger

<table style="text-align:left">
<tr><th>Class</th><td>MockLogger</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Test\Mock\MockLogger</td></tr>
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
<th><a href="#threshold"><strong>threshold</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>/*
|--------------------------------------------------------------------------
| Error Logging Threshold
|--------------------------------------------------------------------------
|
| You can enable error logging by setting a threshold over zero. The
| threshold determines what gets logged. Any values below or equal to the
| threshold will be logged. Threshold options are:
|
|	0 = Disables logging, Error logging TURNED OFF
|	1 = Emergency Messages  - System is unusable
|	2 = Alert Messages      - Action Must Be Taken Immediately
|   3 = Critical Messages   - Application component unavailable, unexpected exception.</td>
</tr>
<tr>
<th><a href="#dateFormat"><strong>dateFormat</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>/*
|--------------------------------------------------------------------------
| Date Format for Logs
|--------------------------------------------------------------------------
|
| Each item that is logged has an associated date. You can use PHP date
| codes to set your own date formatting
|</td>
</tr>
<tr>
<th><a href="#handlers"><strong>handlers</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>/*
|--------------------------------------------------------------------------
| Log Handlers
|--------------------------------------------------------------------------
|
| The logging system supports multiple actions to be taken when something
| is logged. This is done by allowing for multiple Handlers, special classes
| designed to write the log to their chosen destinations, whether that is
| a file on the getServer, a cloud-based service, or even taking actions such
| as emailing the dev team.</td>
</tr>


</table>





### Properties


<hr>

#### $threshold

```php
public $threshold = 9;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
/*
|--------------------------------------------------------------------------
| Error Logging Threshold
|--------------------------------------------------------------------------
|
| You can enable error logging by setting a threshold over zero. The
| threshold determines what gets logged. Any values below or equal to the
| threshold will be logged. Threshold options are:
|
|	0 = Disables logging, Error logging TURNED OFF
|	1 = Emergency Messages  - System is unusable
|	2 = Alert Messages      - Action Must Be Taken Immediately
|   3 = Critical Messages   - Application component unavailable, unexpected exception.
</td></tr>
</table>

<table>
<tr><td>
|   4 = Runtime Errors      - Don't need immediate action, but should be monitored.
|   5 = Warnings            - Exceptional occurrences that are not errors.
|   6 = Notices             - Normal but significant events.
|   7 = Info                - Interesting events, like user logging in, etc.
|   8 = Debug               - Detailed debug information.
|   9 = All Messages
|
| You can also pass an array with threshold levels to show individual error types
|
| 	array(1, 2, 3, 8) = Emergency, Alert, Critical, and Debug messages
|
| For a live site you'll usually enable Critical or higher (3) to be logged otherwise
| your log files will fill up very fast.
|
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>






<hr>

#### $dateFormat

```php
public $dateFormat = 'Y-m-d';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
/*
|--------------------------------------------------------------------------
| Date Format for Logs
|--------------------------------------------------------------------------
|
| Each item that is logged has an associated date. You can use PHP date
| codes to set your own date formatting
|
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>






<hr>

#### $handlers

```php
public $handlers = [
	//--------------------------------------------------------------------
	// File Handler
	//--------------------------------------------------------------------

	'Tests\Support\Log\Handlers\TestHandler' => [
		/*
		 * The log levels that this handler will handle.
		 */
		'handles' => [
			'critical',
			'alert',
			'emergency',
			'debug',
			'error',
			'info',
			'notice',
			'warning',
		],

		/*
		 * Logging Directory Path
		 */
		'path'    => '',
	],
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
/*
|--------------------------------------------------------------------------
| Log Handlers
|--------------------------------------------------------------------------
|
| The logging system supports multiple actions to be taken when something
| is logged. This is done by allowing for multiple Handlers, special classes
| designed to write the log to their chosen destinations, whether that is
| a file on the getServer, a cloud-based service, or even taking actions such
| as emailing the dev team.
</td></tr>
</table>

<table>
<tr><td>
|
| Each handler is defined by the class name used for that handler, and it
| MUST implement the CodeIgniter\Log\Handlers\HandlerInterface interface.
|
| The value of each key is an array of configuration items that are sent
| to the constructor of each handler. The only required configuration item
| is the 'handles' element, which must be an array of integer log levels.
| This is most easily handled by using the constants defined in the
| Psr\Log\LogLevel class.
|
| Handlers are executed in the order defined in this array, starting with
| the handler on top and continuing down.
|
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Test/Mock/MockLogger.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockLanguage.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Test/Mock/MockQuery.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:16**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>