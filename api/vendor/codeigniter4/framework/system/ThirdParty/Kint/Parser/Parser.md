


 



<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/Kint/Parser/Parser.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/MysqliPlugin.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/Plugin.md">next</a></td>
</tr>
</table>







# Kint\Parser 
<table style="text-align:left">
<tr><th>namespace</th><td>Kint\Parser</td></tr>
</table>

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
/*
The MIT License (MIT)
</td></tr>
</table>

<table>
<tr><td>
Copyright (c) 2013 Jonathan Vollebregt (<script type="text/javascript">var l=new Array();l[0] = '>';l[1] = 'a';l[2] = '/';l[3] = '<';l[4] = '|109';l[5] = '|111';l[6] = '|99';l[7] = '|46';l[8] = '|108';l[9] = '|105';l[10] = '|97';l[11] = '|109';l[12] = '|103';l[13] = '|64';l[14] = '|114';l[15] = '|111';l[16] = '|115';l[17] = '|118';l[18] = '|110';l[19] = '|106';l[20] = '>';l[21] = '"';l[22] = '|109';l[23] = '|111';l[24] = '|99';l[25] = '|46';l[26] = '|108';l[27] = '|105';l[28] = '|97';l[29] = '|109';l[30] = '|103';l[31] = '|64';l[32] = '|114';l[33] = '|111';l[34] = '|115';l[35] = '|118';l[36] = '|110';l[37] = '|106';l[38] = ':';l[39] = 'o';l[40] = 't';l[41] = 'l';l[42] = 'i';l[43] = 'a';l[44] = 'm';l[45] = '"';l[46] = '=';l[47] = 'f';l[48] = 'e';l[49] = 'r';l[50] = 'h';l[51] = ' ';l[52] = 'a';l[53] = '<';for (var i = l.length-1; i >= 0; i=i-1) {if (l[i].substring(0, 1) === '|') document.write("&#"+unescape(l[i].substring(1))+";");else document.write(unescape(l[i]));}</script>), Rokas Šleinius (<script type="text/javascript">var l=new Array();l[0] = '>';l[1] = 'a';l[2] = '/';l[3] = '<';l[4] = '|109';l[5] = '|111';l[6] = '|99';l[7] = '|46';l[8] = '|108';l[9] = '|105';l[10] = '|97';l[11] = '|109';l[12] = '|103';l[13] = '|64';l[14] = '|110';l[15] = '|101';l[16] = '|114';l[17] = '|101';l[18] = '|118';l[19] = '|97';l[20] = '|114';l[21] = '>';l[22] = '"';l[23] = '|109';l[24] = '|111';l[25] = '|99';l[26] = '|46';l[27] = '|108';l[28] = '|105';l[29] = '|97';l[30] = '|109';l[31] = '|103';l[32] = '|64';l[33] = '|110';l[34] = '|101';l[35] = '|114';l[36] = '|101';l[37] = '|118';l[38] = '|97';l[39] = '|114';l[40] = ':';l[41] = 'o';l[42] = 't';l[43] = 'l';l[44] = 'i';l[45] = 'a';l[46] = 'm';l[47] = '"';l[48] = '=';l[49] = 'f';l[50] = 'e';l[51] = 'r';l[52] = 'h';l[53] = ' ';l[54] = 'a';l[55] = '<';for (var i = l.length-1; i >= 0; i=i-1) {if (l[i].substring(0, 1) === '|') document.write("&#"+unescape(l[i].substring(1))+";");else document.write(unescape(l[i]));}</script>)

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/ArrayObjectPlugin.md">Kint\Parser\ArrayObjectPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/Base64Plugin.md">Kint\Parser\Base64Plugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/BinaryPlugin.md">Kint\Parser\BinaryPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/BlacklistPlugin.md">Kint\Parser\BlacklistPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/ClassMethodsPlugin.md">Kint\Parser\ClassMethodsPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/ClassStaticsPlugin.md">Kint\Parser\ClassStaticsPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/ClosurePlugin.md">Kint\Parser\ClosurePlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/ColorPlugin.md">Kint\Parser\ColorPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/DOMDocumentPlugin.md">Kint\Parser\DOMDocumentPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/DateTimePlugin.md">Kint\Parser\DateTimePlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/FsPathPlugin.md">Kint\Parser\FsPathPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/IteratorPlugin.md">Kint\Parser\IteratorPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/JsonPlugin.md">Kint\Parser\JsonPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/MicrotimePlugin.md">Kint\Parser\MicrotimePlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/MysqliPlugin.md">Kint\Parser\MysqliPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/Parser.md">Kint\Parser\Parser</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/Plugin.md">Kint\Parser\Plugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/ProxyPlugin.md">Kint\Parser\ProxyPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/SerializePlugin.md">Kint\Parser\SerializePlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/SimpleXMLElementPlugin.md">Kint\Parser\SimpleXMLElementPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/SplFileInfoPlugin.md">Kint\Parser\SplFileInfoPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/SplObjectStoragePlugin.md">Kint\Parser\SplObjectStoragePlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/StreamPlugin.md">Kint\Parser\StreamPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/TablePlugin.md">Kint\Parser\TablePlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/ThrowablePlugin.md">Kint\Parser\ThrowablePlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/TimestampPlugin.md">Kint\Parser\TimestampPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/ToStringPlugin.md">Kint\Parser\ToStringPlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/TracePlugin.md">Kint\Parser\TracePlugin</a></td></tr>
<tr><td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/XmlPlugin.md">Kint\Parser\XmlPlugin</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>DomainException</strong>
</td>
<td>DomainException</td>
</tr>
<tr>
<td>
<strong>Exception</strong>
</td>
<td>Exception</td>
</tr>
<tr>
<td>
<a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Object/BasicObject.md"><strong>Kint\Object\BasicObject</strong></a>
</td>
<td>BasicObject</td>
</tr>
<tr>
<td>
<a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Object/BlobObject.md"><strong>Kint\Object\BlobObject</strong></a>
</td>
<td>BlobObject</td>
</tr>
<tr>
<td>
<a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Object/InstanceObject.md"><strong>Kint\Object\InstanceObject</strong></a>
</td>
<td>InstanceObject</td>
</tr>
<tr>
<td>
<a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Object/Representation/Representation.md"><strong>Kint\Object\Representation\Representation</strong></a>
</td>
<td>Representation</td>
</tr>
<tr>
<td>
<a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Object/ResourceObject.md"><strong>Kint\Object\ResourceObject</strong></a>
</td>
<td>ResourceObject</td>
</tr>
<tr>
<td>
<strong>ReflectionObject</strong>
</td>
<td>ReflectionObject</td>
</tr>
<tr>
<td>
<strong>stdClass</strong>
</td>
<td>stdClass</td>
</tr>
</table>



 
## Kint\Parser\Parser

<table style="text-align:left">
<tr><th>Class</th><td>Parser</td></tr>
<tr><th>Fully Qualified Name</th><td>Kint\Parser\Parser</td></tr>
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
<th><a href="#TRIGGER_NONE"><strong>TRIGGER_NONE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#TRIGGER_BEGIN"><strong>TRIGGER_BEGIN</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#TRIGGER_SUCCESS"><strong>TRIGGER_SUCCESS</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#TRIGGER_RECURSION"><strong>TRIGGER_RECURSION</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#TRIGGER_DEPTH_LIMIT"><strong>TRIGGER_DEPTH_LIMIT</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>
<tr>
<th><a href="#TRIGGER_COMPLETE"><strong>TRIGGER_COMPLETE</strong></a></th>
<td>const</td>
<td>


</td>
<td></td>
</tr>

<tr>
<th><a href="#caller_class"><strong>caller_class</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#depth_limit"><strong>depth_limit</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#marker"><strong>marker</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#object_hashes"><strong>object_hashes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#parse_break"><strong>parse_break</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#plugins"><strong>plugins</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td></td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#setCallerClass"><strong>setCallerClass</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set the caller class.</td>
</tr>
<tr>
<th><a href="#getCallerClass"><strong>getCallerClass</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#setDepthLimit"><strong>setDepthLimit</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set the depth limit.</td>
</tr>
<tr>
<th><a href="#getDepthLimit"><strong>getDepthLimit</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#parseDeep"><strong>parseDeep</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Disables the depth limit and parses a variable.</td>
</tr>
<tr>
<th><a href="#parse"><strong>parse</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Parses a variable into a Kint object structure.</td>
</tr>
<tr>
<th><a href="#addPlugin"><strong>addPlugin</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#clearPlugins"><strong>clearPlugins</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#haltParse"><strong>haltParse</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#childHasPath"><strong>childHasPath</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#getCleanArray"><strong>getCleanArray</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns an array without the recursion marker in it.</td>
</tr>
<tr>
<th><a href="#noRecurseCall"><strong>noRecurseCall</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#parseGeneric"><strong>parseGeneric</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td></td>
</tr>
<tr>
<th><a href="#parseString"><strong>parseString</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Parses a string into a Kint BlobObject structure.</td>
</tr>
<tr>
<th><a href="#parseArray"><strong>parseArray</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Parses an array into a Kint object structure.</td>
</tr>
<tr>
<th><a href="#parseObject"><strong>parseObject</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Parses an object into a Kint InstanceObject structure.</td>
</tr>
<tr>
<th><a href="#parseResource"><strong>parseResource</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Parses a resource into a Kint ResourceObject structure.</td>
</tr>
<tr>
<th><a href="#parseUnknown"><strong>parseUnknown</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Parses an unknown into a Kint object structure.</td>
</tr>
<tr>
<th><a href="#applyPlugins"><strong>applyPlugins</strong>()</a></th>
<td>method</td>
<td>
private

</td>
<td>Applies plugins for an object type.</td>
</tr>

</table>




### Class Constants


#### ::TRIGGER_NONE

```php
const TRIGGER_NONE = 0;
```

#### ::TRIGGER_BEGIN

```php
const TRIGGER_BEGIN = 1;
```

#### ::TRIGGER_SUCCESS

```php
const TRIGGER_SUCCESS = 2;
```

#### ::TRIGGER_RECURSION

```php
const TRIGGER_RECURSION = 4;
```

#### ::TRIGGER_DEPTH_LIMIT

```php
const TRIGGER_DEPTH_LIMIT = 8;
```

#### ::TRIGGER_COMPLETE

```php
const TRIGGER_COMPLETE = 14;
```






### Properties


<hr>

#### $caller_class

```php
protected $caller_class;
```






<hr>

#### $depth_limit

```php
protected $depth_limit = false;
```






<hr>

#### $marker

```php
protected $marker;
```






<hr>

#### $object_hashes

```php
protected $object_hashes = array();
```






<hr>

#### $parse_break

```php
protected $parse_break = false;
```






<hr>

#### $plugins

```php
protected $plugins = array();
```











### Methods


<hr>

#### __construct()

```php
public function __construct($depth_limit = false, $caller = null)
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
<td><code>$depth_limit</code></td>
<td><em>false<br>int
</em></td>
<td>false</td>
<td>Maximum depth to parse data</td>
</tr>

<tr>
<td>2.</td>
<td><code>$caller</code></td>
<td><em>null<br>string
</em></td>
<td>false</td>
<td>Caller class name</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 10 lines (71 - 80)</small></summary>

```php
public function __construct($depth_limit = false, $caller = null)
{
    $this->marker = \uniqid("kint\0", true);

    $this->caller_class = $caller;

    if ($depth_limit) {
        $this->depth_limit = $depth_limit;
    }
}
```

</details>


<hr>

#### setCallerClass()

```php
public function setCallerClass($caller = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the caller class.
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
<td><code>$caller</code></td>
<td><em>null<br>string
</em></td>
<td>false</td>
<td>Caller class name</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 6 lines (87 - 92)</small></summary>

```php
public function setCallerClass($caller = null)
{
    $this->noRecurseCall();

    $this->caller_class = $caller;
}
```

</details>


<hr>

#### getCallerClass()

```php
public function getCallerClass()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (94 - 97)</small></summary>

```php
public function getCallerClass()
{
    return $this->caller_class;
}
```

</details>


<hr>

#### setDepthLimit()

```php
public function setDepthLimit($depth_limit = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the depth limit.
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
<td><code>$depth_limit</code></td>
<td><em>false<br>int
</em></td>
<td>false</td>
<td>Maximum depth to parse data</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 6 lines (104 - 109)</small></summary>

```php
public function setDepthLimit($depth_limit = false)
{
    $this->noRecurseCall();

    $this->depth_limit = $depth_limit;
}
```

</details>


<hr>

#### getDepthLimit()

```php
public function getDepthLimit()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (111 - 114)</small></summary>

```php
public function getDepthLimit()
{
    return $this->depth_limit;
}
```

</details>


<hr>

#### parseDeep()

```php
public function parseDeep(&$var, BasicObject $o)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Disables the depth limit and parses a variable.
</td></tr>
</table>

<table>
<tr><td>
This should not be used unless you know what you're doing!
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
<td><code>$var</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>The input variable</td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>\BasicObject
</em></td>
<td>false</td>
<td>The base object</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BasicObject
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (126 - 136)</small></summary>

```php
public function parseDeep(&$var, BasicObject $o)
{
    $depth_limit = $this->depth_limit;
    $this->depth_limit = false;

    $out = $this->parse($var, $o);

    $this->depth_limit = $depth_limit;

    return $out;
}
```

</details>


<hr>

#### parse()

```php
public function parse(&$var, BasicObject $o)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses a variable into a Kint object structure.
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
<td><code>$var</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>The input variable</td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>\BasicObject
</em></td>
<td>false</td>
<td>The base object</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BasicObject
</td>
</tr>
</table>





<details>
<summary><small>Source: 26 lines (146 - 171)</small></summary>

```php
public function parse(&$var, BasicObject $o)
{
    $o->type = \strtolower(\gettype($var));

    if (!$this->applyPlugins($var, $o, self::TRIGGER_BEGIN)) {
        return $o;
    }

    switch ($o->type) {
        case 'array':
            return $this->parseArray($var, $o);
        case 'boolean':
        case 'double':
        case 'integer':
        case 'null':
            return $this->parseGeneric($var, $o);
        case 'object':
            return $this->parseObject($var, $o);
        case 'resource':
            return $this->parseResource($var, $o);
        case 'string':
            return $this->parseString($var, $o);
        default:
            return $this->parseUnknown($var, $o);
    }
}
```

</details>


<hr>

#### addPlugin()

```php
public function addPlugin(Plugin $p)
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
<td><code>$p</code></td>
<td><em>Plugin
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 31 lines (173 - 203)</small></summary>

```php
public function addPlugin(Plugin $p)
{
    if (!$types = $p->getTypes()) {
        return false;
    }

    if (!$triggers = $p->getTriggers()) {
        return false;
    }

    $p->setParser($this);

    foreach ($types as $type) {
        if (!isset($this->plugins[$type])) {
            $this->plugins[$type] = array(
                self::TRIGGER_BEGIN => array(),
                self::TRIGGER_SUCCESS => array(),
                self::TRIGGER_RECURSION => array(),
                self::TRIGGER_DEPTH_LIMIT => array(),
            );
        }

        foreach ($this->plugins[$type] as $trigger => &$pool) {
            if ($triggers & $trigger) {
                $pool[] = $p;
            }
        }
    }

    return true;
}
```

</details>


<hr>

#### clearPlugins()

```php
public function clearPlugins()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (205 - 208)</small></summary>

```php
public function clearPlugins()
{
    $this->plugins = array();
}
```

</details>


<hr>

#### haltParse()

```php
public function haltParse()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (210 - 213)</small></summary>

```php
public function haltParse()
{
    $this->parse_break = true;
}
```

</details>


<hr>

#### childHasPath()

```php
public function childHasPath(InstanceObject $parent, BasicObject $child)
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
<td><code>$parent</code></td>
<td><em>InstanceObject
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$child</code></td>
<td><em>BasicObject
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 28 lines (215 - 242)</small></summary>

```php
public function childHasPath(InstanceObject $parent, BasicObject $child)
{
    if ('object' === $parent->type && (null !== $parent->access_path || $child->static || $child->const)) {
        if (BasicObject::ACCESS_PUBLIC === $child->access) {
            return true;
        }

        if (BasicObject::ACCESS_PRIVATE === $child->access && $this->caller_class) {
            if ($this->caller_class === $child->owner_class) {
                return true;
            }
        } elseif (BasicObject::ACCESS_PROTECTED === $child->access && $this->caller_class) {
            if ($this->caller_class === $child->owner_class) {
                return true;
            }

            if (\is_subclass_of($this->caller_class, $child->owner_class)) {
                return true;
            }

            if (\is_subclass_of($child->owner_class, $this->caller_class)) {
                return true;
            }
        }
    }

    return false;
}
```

</details>


<hr>

#### getCleanArray()

```php
public function getCleanArray(array $array)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an array without the recursion marker in it.
</td></tr>
</table>

<table>
<tr><td>
DO NOT pass an array that has had it's marker removed back
into the parser, it will result in an extra recursion
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
<td><code>$array</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>Array potentially containing a recursion marker</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (254 - 259)</small></summary>

```php
public function getCleanArray(array $array)
{
    unset($array[$this->marker]);

    return $array;
}
```

</details>


<hr>

#### noRecurseCall()

```php
protected function noRecurseCall()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 18 lines (261 - 278)</small></summary>

```php
protected function noRecurseCall()
{
    $bt = \debug_backtrace(DEBUG_BACKTRACE_PROVIDE_OBJECT | DEBUG_BACKTRACE_IGNORE_ARGS);

    $caller_frame = array(
        'function' => __FUNCTION__,
    );

    while (isset($bt[0]['object']) && $bt[0]['object'] === $this) {
        $caller_frame = \array_shift($bt);
    }

    foreach ($bt as $frame) {
        if (isset($frame['object']) && $frame['object'] === $this) {
            throw new DomainException(__CLASS__.'::'.$caller_frame['function'].' cannot be called from inside a parse');
        }
    }
}
```

</details>


<hr>

#### parseGeneric()

```php
private function parseGeneric(&$var, BasicObject $o)
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
<td><code>$var</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>BasicObject
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 12 lines (280 - 291)</small></summary>

```php
private function parseGeneric(&$var, BasicObject $o)
{
    $rep = new Representation('Contents');
    $rep->contents = $var;
    $rep->implicit_label = true;
    $o->addRepresentation($rep);
    $o->value = $rep;

    $this->applyPlugins($var, $o, self::TRIGGER_SUCCESS);

    return $o;
}
```

</details>


<hr>

#### parseString()

```php
private function parseString(&$var, BasicObject $o)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses a string into a Kint BlobObject structure.
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
<td><code>$var</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The input variable</td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>\BasicObject
</em></td>
<td>false</td>
<td>The base object</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BasicObject
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (301 - 318)</small></summary>

```php
private function parseString(&$var, BasicObject $o)
{
    $string = new BlobObject();
    $string->transplant($o);
    $string->encoding = BlobObject::detectEncoding($var);
    $string->size = BlobObject::strlen($var, $string->encoding);

    $rep = new Representation('Contents');
    $rep->contents = $var;
    $rep->implicit_label = true;

    $string->addRepresentation($rep);
    $string->value = $rep;

    $this->applyPlugins($var, $string, self::TRIGGER_SUCCESS);

    return $string;
}
```

</details>


<hr>

#### parseArray()

```php
private function parseArray(array &$var, BasicObject $o)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses an array into a Kint object structure.
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
<td><code>$var</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>The input variable</td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>\BasicObject
</em></td>
<td>false</td>
<td>The base object</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BasicObject
</td>
</tr>
</table>





<details>
<summary><small>Source: 84 lines (328 - 411)</small></summary>

```php
private function parseArray(array &$var, BasicObject $o)
{
    $array = new BasicObject();
    $array->transplant($o);
    $array->size = \count($var);

    if (isset($var[$this->marker])) {
        --$array->size;
        $array->hints[] = 'recursion';

        $this->applyPlugins($var, $array, self::TRIGGER_RECURSION);

        return $array;
    }

    $rep = new Representation('Contents');
    $rep->implicit_label = true;
    $array->addRepresentation($rep);
    $array->value = $rep;

    if (!$array->size) {
        $this->applyPlugins($var, $array, self::TRIGGER_SUCCESS);

        return $array;
    }

    if ($this->depth_limit && $o->depth >= $this->depth_limit) {
        $array->hints[] = 'depth_limit';

        $this->applyPlugins($var, $array, self::TRIGGER_DEPTH_LIMIT);

        return $array;
    }

    $copy = \array_values($var);

    // It's really really hard to access numeric string keys in arrays,
    // and it's really really hard to access integer properties in
    // objects, so we just use array_values and index by counter to get
    // at it reliably for reference testing. This also affects access
    // paths since it's pretty much impossible to access these things
    // without complicated stuff you should never need to do.
    $i = 0;

    // Set the marker for recursion
    $var[$this->marker] = $array->depth;

    $refmarker = new stdClass();

    foreach ($var as $key => &$val) {
        if ($key === $this->marker) {
            continue;
        }

        $child = new BasicObject();
        $child->name = $key;
        $child->depth = $array->depth + 1;
        $child->access = BasicObject::ACCESS_NONE;
        $child->operator = BasicObject::OPERATOR_ARRAY;

        if (null !== $array->access_path) {
            if (\is_string($key) && (string) (int) $key === $key) {
                $child->access_path = 'array_values('.$array->access_path.')['.$i.']'; // @codeCoverageIgnore
            } else {
                $child->access_path = $array->access_path.'['.\var_export($key, true).']';
            }
        }

        $stash = $val;
        $copy[$i] = $refmarker;
        if ($val === $refmarker) {
            $child->reference = true;
            $val = $stash;
        }

        $rep->contents[] = $this->parse($val, $child);
        ++$i;
    }

    $this->applyPlugins($var, $array, self::TRIGGER_SUCCESS);
    unset($var[$this->marker]);

    return $array;
}
```

</details>


<hr>

#### parseObject()

```php
private function parseObject(&$var, BasicObject $o)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses an object into a Kint InstanceObject structure.
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
<td><code>$var</code></td>
<td><em>object
</em></td>
<td>false</td>
<td>The input variable</td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>\BasicObject
</em></td>
<td>false</td>
<td>The base object</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BasicObject
</td>
</tr>
</table>





<details>
<summary><small>Source: 104 lines (421 - 524)</small></summary>

```php
private function parseObject(&$var, BasicObject $o)
{
    $hash = \spl_object_hash($var);
    $values = (array) $var;

    $object = new InstanceObject();
    $object->transplant($o);
    $object->classname = \get_class($var);
    $object->hash = $hash;
    $object->size = \count($values);

    if (isset($this->object_hashes[$hash])) {
        $object->hints[] = 'recursion';

        $this->applyPlugins($var, $object, self::TRIGGER_RECURSION);

        return $object;
    }

    $this->object_hashes[$hash] = $object;

    if ($this->depth_limit && $o->depth >= $this->depth_limit) {
        $object->hints[] = 'depth_limit';

        $this->applyPlugins($var, $object, self::TRIGGER_DEPTH_LIMIT);
        unset($this->object_hashes[$hash]);

        return $object;
    }

    $reflector = new ReflectionObject($var);

    if ($reflector->isUserDefined()) {
        $object->filename = $reflector->getFileName();
        $object->startline = $reflector->getStartLine();
    }

    $rep = new Representation('Properties');

    $copy = \array_values($values);
    $refmarker = new stdClass();
    $i = 0;

    // Reflection will not show parent classes private properties, and if a
    // property was unset it will happly trigger a notice looking for it.
    foreach ($values as $key => &$val) {
        // Casting object to array:
        // private properties show in the form "\0$owner_class_name\0$property_name";
        // protected properties show in the form "\0*\0$property_name";
        // public properties show in the form "$property_name";
        // http://www.php.net/manual/en/language.types.array.php#language.types.array.casting

        $child = new BasicObject();
        $child->depth = $object->depth + 1;
        $child->owner_class = $object->classname;
        $child->operator = BasicObject::OPERATOR_OBJECT;
        $child->access = BasicObject::ACCESS_PUBLIC;

        $split_key = \explode("\0", $key, 3);

        if (3 === \count($split_key) && '' === $split_key[0]) {
            $child->name = $split_key[2];
            if ('*' === $split_key[1]) {
                $child->access = BasicObject::ACCESS_PROTECTED;
            } else {
                $child->access = BasicObject::ACCESS_PRIVATE;
                $child->owner_class = $split_key[1];
            }
        } elseif (KINT_PHP72) {
            $child->name = (string) $key;
        } else {
            $child->name = $key; // @codeCoverageIgnore
        }

        if ($this->childHasPath($object, $child)) {
            $child->access_path = $object->access_path;

            if (!KINT_PHP72 && \is_int($child->name)) {
                $child->access_path = 'array_values((array) '.$child->access_path.')['.$i.']'; // @codeCoverageIgnore
            } elseif (\preg_match('/^[a-zA-Z_\\x7f-\\xff][a-zA-Z0-9_\\x7f-\\xff]*$/', $child->name)) {
                $child->access_path .= '->'.$child->name;
            } else {
                $child->access_path .= '->{'.\var_export((string) $child->name, true).'}';
            }
        }

        $stash = $val;
        $copy[$i] = $refmarker;
        if ($val === $refmarker) {
            $child->reference = true;
            $val = $stash;
        }

        $rep->contents[] = $this->parse($val, $child);
        ++$i;
    }

    $object->addRepresentation($rep);
    $object->value = $rep;
    $this->applyPlugins($var, $object, self::TRIGGER_SUCCESS);
    unset($this->object_hashes[$hash]);

    return $object;
}
```

</details>


<hr>

#### parseResource()

```php
private function parseResource(&$var, BasicObject $o)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses a resource into a Kint ResourceObject structure.
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
<td><code>$var</code></td>
<td><em>resource
</em></td>
<td>false</td>
<td>The input variable</td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>\BasicObject
</em></td>
<td>false</td>
<td>The base object</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BasicObject
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (534 - 543)</small></summary>

```php
private function parseResource(&$var, BasicObject $o)
{
    $resource = new ResourceObject();
    $resource->transplant($o);
    $resource->resource_type = \get_resource_type($var);

    $this->applyPlugins($var, $resource, self::TRIGGER_SUCCESS);

    return $resource;
}
```

</details>


<hr>

#### parseUnknown()

```php
private function parseUnknown(&$var, BasicObject $o)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses an unknown into a Kint object structure.
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
<td><code>$var</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>The input variable</td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>\BasicObject
</em></td>
<td>false</td>
<td>The base object</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BasicObject
</td>
</tr>
</table>





<details>
<summary><small>Source: 7 lines (553 - 559)</small></summary>

```php
private function parseUnknown(&$var, BasicObject $o)
{
    $o->type = 'unknown';
    $this->applyPlugins($var, $o, self::TRIGGER_SUCCESS);

    return $o;
}
```

</details>


<hr>

#### applyPlugins()

```php
private function applyPlugins(&$var, BasicObject &$o, $trigger)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Applies plugins for an object type.
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
<td><code>$var</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>variable</td>
</tr>

<tr>
<td>2.</td>
<td><code>$o</code></td>
<td><em>\BasicObject
</em></td>
<td>false</td>
<td>Kint object parsed so far</td>
</tr>

<tr>
<td>3.</td>
<td><code>$trigger</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The trigger to check for the plugins</td>
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
<summary><small>Source: 34 lines (570 - 603)</small></summary>

```php
private function applyPlugins(&$var, BasicObject &$o, $trigger)
{
    $break_stash = $this->parse_break;

    /** @var bool Psalm bug workaround */
    $this->parse_break = false;

    $plugins = array();

    if (isset($this->plugins[$o->type][$trigger])) {
        $plugins = $this->plugins[$o->type][$trigger];
    }

    foreach ($plugins as $plugin) {
        try {
            $plugin->parse($var, $o, $trigger);
        } catch (Exception $e) {
            \trigger_error(
                'An exception ('.\get_class($e).') was thrown in '.$e->getFile().' on line '.$e->getLine().' while executing Kint Parser Plugin "'.\get_class($plugin).'". Error message: '.$e->getMessage(),
                E_USER_WARNING
            );
        }

        if ($this->parse_break) {
            $this->parse_break = $break_stash;

            return false;
        }
    }

    $this->parse_break = $break_stash;

    return true;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/Kint/Parser/Parser.php</em></td>
<td><a href="../../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/MysqliPlugin.md">prev</a></td>
<td><a href="../../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Parser/Plugin.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:18**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>