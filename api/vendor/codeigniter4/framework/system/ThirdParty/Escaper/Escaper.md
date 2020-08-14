


 



<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/Escaper/Escaper.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Utils.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Escaper/Exception/ExceptionInterface.md">next</a></td>
</tr>
</table>







# Laminas\Escaper 
<table style="text-align:left">
<tr><th>namespace</th><td>Laminas\Escaper</td></tr>
</table>

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

*No description.*


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>copyright</th>
<td><a href="https://github.com/laminas/laminas-escaper/blob/master/COPYRIGHT.md">https://github.com/laminas/laminas-escaper/blob/master/COPYRIGHT.md</a>
</td>
</tr>
<tr style="vertical-align:top;">
<th>license</th>
<td><a href="https://github.com/laminas/laminas-escaper/blob/master/LICENSE.md">https://github.com/laminas/laminas-escaper/blob/master/LICENSE.md</a> New BSD License
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Escaper/Escaper.md">Laminas\Escaper\Escaper</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Escaper/Exception/ExceptionInterface.md">Laminas\Escaper\Exception\ExceptionInterface</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Escaper/Exception/InvalidArgumentException.md">Laminas\Escaper\Exception\InvalidArgumentException</a></td></tr>
<tr><td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Escaper/Exception/RuntimeException.md">Laminas\Escaper\Exception\RuntimeException</a></td></tr>
</table>
</details>



 

 
## Laminas\Escaper\Escaper

<table style="text-align:left">
<tr><th>Class</th><td>Escaper</td></tr>
<tr><th>Fully Qualified Name</th><td>Laminas\Escaper\Escaper</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Context specific methods for use in secure output escaping
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
<th><a href="#htmlNamedEntityMap"><strong>htmlNamedEntityMap</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Entity Map mapping Unicode codepoints to any available named HTML entities.</td>
</tr>
<tr>
<th><a href="#encoding"><strong>encoding</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Current encoding for escaping. If not UTF-8, we convert strings from this encoding
pre-escaping and back to this encoding post-escaping.</td>
</tr>
<tr>
<th><a href="#htmlSpecialCharsFlags"><strong>htmlSpecialCharsFlags</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Holds the value of the special flags passed as second parameter to
htmlspecialchars().</td>
</tr>
<tr>
<th><a href="#htmlAttrMatcher"><strong>htmlAttrMatcher</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Static Matcher which escapes characters for HTML Attribute contexts</td>
</tr>
<tr>
<th><a href="#jsMatcher"><strong>jsMatcher</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Static Matcher which escapes characters for Javascript contexts</td>
</tr>
<tr>
<th><a href="#cssMatcher"><strong>cssMatcher</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Static Matcher which escapes characters for CSS Attribute contexts</td>
</tr>
<tr>
<th><a href="#supportedEncodings"><strong>supportedEncodings</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>List of all encoding supported by this class</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor: Single parameter allows setting of global encoding for use by
the current object.</td>
</tr>
<tr>
<th><a href="#getEncoding"><strong>getEncoding</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Return the encoding that all output/input is expected to be encoded in.</td>
</tr>
<tr>
<th><a href="#escapeHtml"><strong>escapeHtml</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Escape a string for the HTML Body context where there are very few characters
of special meaning. Internally this will use htmlspecialchars().</td>
</tr>
<tr>
<th><a href="#escapeHtmlAttr"><strong>escapeHtmlAttr</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Escape a string for the HTML Attribute context. We use an extended set of characters
to escape that are not covered by htmlspecialchars() to cover cases where an attribute
might be unquoted or quoted illegally (e.g. backticks are valid quotes for IE).</td>
</tr>
<tr>
<th><a href="#escapeJs"><strong>escapeJs</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Escape a string for the Javascript context. This does not use json_encode(). An extended
set of characters are escaped beyond ECMAScript&#039;s rules for Javascript literal string
escaping in order to prevent misinterpretation of Javascript as HTML leading to the
injection of special characters and entities. The escaping used should be tolerant
of cases where HTML escaping was not applied on top of Javascript escaping correctly.</td>
</tr>
<tr>
<th><a href="#escapeUrl"><strong>escapeUrl</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Escape a string for the URI or Parameter contexts. This should not be used to escape
an entire URI - only a subcomponent being inserted. The function is a simple proxy
to rawurlencode() which now implements RFC 3986 since PHP 5.3 completely.</td>
</tr>
<tr>
<th><a href="#escapeCss"><strong>escapeCss</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Escape a string for the CSS context. CSS escaping can be applied to any string being
inserted into CSS and escapes everything except alphanumerics.</td>
</tr>
<tr>
<th><a href="#htmlAttrMatcher"><strong>htmlAttrMatcher</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Callback function for preg_replace_callback that applies HTML Attribute
escaping to all matches.</td>
</tr>
<tr>
<th><a href="#jsMatcher"><strong>jsMatcher</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Callback function for preg_replace_callback that applies Javascript
escaping to all matches.</td>
</tr>
<tr>
<th><a href="#cssMatcher"><strong>cssMatcher</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Callback function for preg_replace_callback that applies CSS
escaping to all matches.</td>
</tr>
<tr>
<th><a href="#toUtf8"><strong>toUtf8</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Converts a string to UTF-8 from the base encoding. The base encoding is set via this
class&#039; constructor.</td>
</tr>
<tr>
<th><a href="#fromUtf8"><strong>fromUtf8</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Converts a string from UTF-8 to the base encoding. The base encoding is set via this
class&#039; constructor.</td>
</tr>
<tr>
<th><a href="#isUtf8"><strong>isUtf8</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Checks if a given string appears to be valid UTF-8 or not.</td>
</tr>
<tr>
<th><a href="#convertEncoding"><strong>convertEncoding</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Encoding conversion helper which wraps iconv and mbstring where they exist or throws
and exception where neither is available.</td>
</tr>

</table>





### Properties


<hr>

#### $htmlNamedEntityMap

```php
protected static $htmlNamedEntityMap = [
    34 => 'quot',         // quotation mark
    38 => 'amp',          // ampersand
    60 => 'lt',           // less-than sign
    62 => 'gt',           // greater-than sign
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Entity Map mapping Unicode codepoints to any available named HTML entities.
</td></tr>
</table>

<table>
<tr><td>
While HTML supports far more named entities, the lowest common denominator
has become HTML5's XML Serialisation which is restricted to the those named
entities that XML supports. Using HTML entities would result in this error:
    XML Parsing Error: undefined entity
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

#### $encoding

```php
protected $encoding = 'utf-8';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Current encoding for escaping. If not UTF-8, we convert strings from this encoding
pre-escaping and back to this encoding post-escaping.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>string
</td>
</tr>
</table>


<hr>

#### $htmlSpecialCharsFlags

```php
protected $htmlSpecialCharsFlags;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Holds the value of the special flags passed as second parameter to
htmlspecialchars().
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>int
</td>
</tr>
</table>


<hr>

#### $htmlAttrMatcher

```php
protected $htmlAttrMatcher;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Static Matcher which escapes characters for HTML Attribute contexts
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>callable
</td>
</tr>
</table>


<hr>

#### $jsMatcher

```php
protected $jsMatcher;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Static Matcher which escapes characters for Javascript contexts
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>callable
</td>
</tr>
</table>


<hr>

#### $cssMatcher

```php
protected $cssMatcher;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Static Matcher which escapes characters for CSS Attribute contexts
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>callable
</td>
</tr>
</table>


<hr>

#### $supportedEncodings

```php
protected $supportedEncodings = [
    'iso-8859-1',   'iso8859-1',    'iso-8859-5',   'iso8859-5',
    'iso-8859-15',  'iso8859-15',   'utf-8',        'cp866',
    'ibm866',       '866',          'cp1251',       'windows-1251',
    'win-1251',     '1251',         'cp1252',       'windows-1252',
    '1252',         'koi8-r',       'koi8-ru',      'koi8r',
    'big5',         '950',          'gb2312',       '936',
    'big5-hkscs',   'shift_jis',    'sjis',         'sjis-win',
    'cp932',        '932',          'euc-jp',       'eucjp',
    'eucjp-win',    'macroman'
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
List of all encoding supported by this class
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







### Methods


<hr>

#### __construct()

```php
public function __construct($encoding = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor: Single parameter allows setting of global encoding for use by
the current object.
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
<td><code>$encoding</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception\InvalidArgumentException
</td>
</tr>
</table>



<details>
<summary><small>Source: 33 lines (94 - 126)</small></summary>

```php
public function __construct($encoding = null)
{
    if ($encoding !== null) {
        if (! is_string($encoding)) {
            throw new Exception\InvalidArgumentException(
                get_class($this) . ' constructor parameter must be a string, received ' . gettype($encoding)
            );
        }
        if ($encoding === '') {
            throw new Exception\InvalidArgumentException(
                get_class($this) . ' constructor parameter does not allow a blank value'
            );
        }

        $encoding = strtolower($encoding);
        if (! in_array($encoding, $this->supportedEncodings)) {
            throw new Exception\InvalidArgumentException(
                'Value of \'' . $encoding . '\' passed to ' . get_class($this)
                . ' constructor parameter is invalid. Provide an encoding supported by htmlspecialchars()'
            );
        }

        $this->encoding = $encoding;
    }

    // We take advantage of ENT_SUBSTITUTE flag to correctly deal with invalid UTF-8 sequences.
    $this->htmlSpecialCharsFlags = ENT_QUOTES | ENT_SUBSTITUTE;

    // set matcher callbacks
    $this->htmlAttrMatcher = [$this, 'htmlAttrMatcher'];
    $this->jsMatcher       = [$this, 'jsMatcher'];
    $this->cssMatcher      = [$this, 'cssMatcher'];
}
```

</details>


<hr>

#### getEncoding()

```php
public function getEncoding()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Return the encoding that all output/input is expected to be encoded in.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (133 - 136)</small></summary>

```php
public function getEncoding()
{
    return $this->encoding;
}
```

</details>


<hr>

#### escapeHtml()

```php
public function escapeHtml($string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Escape a string for the HTML Body context where there are very few characters
of special meaning. Internally this will use htmlspecialchars().
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
<td><code>$string</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (145 - 148)</small></summary>

```php
public function escapeHtml($string)
{
    return htmlspecialchars($string, $this->htmlSpecialCharsFlags, $this->encoding);
}
```

</details>


<hr>

#### escapeHtmlAttr()

```php
public function escapeHtmlAttr($string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Escape a string for the HTML Attribute context. We use an extended set of characters
to escape that are not covered by htmlspecialchars() to cover cases where an attribute
might be unquoted or quoted illegally (e.g. backticks are valid quotes for IE).
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
<td><code>$string</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (158 - 167)</small></summary>

```php
public function escapeHtmlAttr($string)
{
    $string = $this->toUtf8($string);
    if ($string === '' || ctype_digit($string)) {
        return $string;
    }

    $result = preg_replace_callback('/[^a-z0-9,\.\-_]/iSu', $this->htmlAttrMatcher, $string);
    return $this->fromUtf8($result);
}
```

</details>


<hr>

#### escapeJs()

```php
public function escapeJs($string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Escape a string for the Javascript context. This does not use json_encode(). An extended
set of characters are escaped beyond ECMAScript's rules for Javascript literal string
escaping in order to prevent misinterpretation of Javascript as HTML leading to the
injection of special characters and entities. The escaping used should be tolerant
of cases where HTML escaping was not applied on top of Javascript escaping correctly.
</td></tr>
</table>

<table>
<tr><td>
Backslash escaping is not used as it still leaves the escaped character as-is and so
is not useful in a HTML context.
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
<td><code>$string</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (181 - 190)</small></summary>

```php
public function escapeJs($string)
{
    $string = $this->toUtf8($string);
    if ($string === '' || ctype_digit($string)) {
        return $string;
    }

    $result = preg_replace_callback('/[^a-z0-9,\._]/iSu', $this->jsMatcher, $string);
    return $this->fromUtf8($result);
}
```

</details>


<hr>

#### escapeUrl()

```php
public function escapeUrl($string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Escape a string for the URI or Parameter contexts. This should not be used to escape
an entire URI - only a subcomponent being inserted. The function is a simple proxy
to rawurlencode() which now implements RFC 3986 since PHP 5.3 completely.
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
<td><code>$string</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (200 - 203)</small></summary>

```php
public function escapeUrl($string)
{
    return rawurlencode($string);
}
```

</details>


<hr>

#### escapeCss()

```php
public function escapeCss($string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Escape a string for the CSS context. CSS escaping can be applied to any string being
inserted into CSS and escapes everything except alphanumerics.
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
<td><code>$string</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 10 lines (212 - 221)</small></summary>

```php
public function escapeCss($string)
{
    $string = $this->toUtf8($string);
    if ($string === '' || ctype_digit($string)) {
        return $string;
    }

    $result = preg_replace_callback('/[^a-z0-9]/iSu', $this->cssMatcher, $string);
    return $this->fromUtf8($result);
}
```

</details>


<hr>

#### htmlAttrMatcher()

```php
protected function htmlAttrMatcher($matches)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callback function for preg_replace_callback that applies HTML Attribute
escaping to all matches.
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
<td><code>$matches</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 38 lines (230 - 267)</small></summary>

```php
protected function htmlAttrMatcher($matches)
{
    $chr = $matches[0];
    $ord = ord($chr);

    /**
     * The following replaces characters undefined in HTML with the
     * hex entity for the Unicode replacement character.
     */
    if (($ord <= 0x1f && $chr != "\t" && $chr != "\n" && $chr != "\r")
        || ($ord >= 0x7f && $ord <= 0x9f)
    ) {
        return '&#xFFFD;';
    }

    /**
     * Check if the current character to escape has a name entity we should
     * replace it with while grabbing the integer value of the character.
     */
    if (strlen($chr) > 1) {
        $chr = $this->convertEncoding($chr, 'UTF-32BE', 'UTF-8');
    }

    $hex = bin2hex($chr);
    $ord = hexdec($hex);
    if (isset(static::$htmlNamedEntityMap[$ord])) {
        return '&' . static::$htmlNamedEntityMap[$ord] . ';';
    }

    /**
     * Per OWASP recommendations, we'll use upper hex entities
     * for any other characters where a named entity does not exist.
     */
    if ($ord > 255) {
        return sprintf('&#x%04X;', $ord);
    }
    return sprintf('&#x%02X;', $ord);
}
```

</details>


<hr>

#### jsMatcher()

```php
protected function jsMatcher($matches)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callback function for preg_replace_callback that applies Javascript
escaping to all matches.
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
<td><code>$matches</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (276 - 290)</small></summary>

```php
protected function jsMatcher($matches)
{
    $chr = $matches[0];
    if (strlen($chr) == 1) {
        return sprintf('\\x%02X', ord($chr));
    }
    $chr = $this->convertEncoding($chr, 'UTF-16BE', 'UTF-8');
    $hex = strtoupper(bin2hex($chr));
    if (strlen($hex) <= 4) {
        return sprintf('\\u%04s', $hex);
    }
    $highSurrogate = substr($hex, 0, 4);
    $lowSurrogate = substr($hex, 4, 4);
    return sprintf('\\u%04s\\u%04s', $highSurrogate, $lowSurrogate);
}
```

</details>


<hr>

#### cssMatcher()

```php
protected function cssMatcher($matches)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callback function for preg_replace_callback that applies CSS
escaping to all matches.
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
<td><code>$matches</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (299 - 309)</small></summary>

```php
protected function cssMatcher($matches)
{
    $chr = $matches[0];
    if (strlen($chr) == 1) {
        $ord = ord($chr);
    } else {
        $chr = $this->convertEncoding($chr, 'UTF-32BE', 'UTF-8');
        $ord = hexdec(bin2hex($chr));
    }
    return sprintf('\\%X ', $ord);
}
```

</details>


<hr>

#### toUtf8()

```php
protected function toUtf8($string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts a string to UTF-8 from the base encoding. The base encoding is set via this
class' constructor.
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
<td><code>$string</code></td>
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
<td>string
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception\RuntimeException
</td>
</tr>
</table>



<details>
<summary><small>Source: 16 lines (319 - 334)</small></summary>

```php
protected function toUtf8($string)
{
    if ($this->getEncoding() === 'utf-8') {
        $result = $string;
    } else {
        $result = $this->convertEncoding($string, 'UTF-8', $this->getEncoding());
    }

    if (! $this->isUtf8($result)) {
        throw new Exception\RuntimeException(
            sprintf('String to be escaped was not valid UTF-8 or could not be converted: %s', $result)
        );
    }

    return $result;
}
```

</details>


<hr>

#### fromUtf8()

```php
protected function fromUtf8($string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Converts a string from UTF-8 to the base encoding. The base encoding is set via this
class' constructor.
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
<td><code>$string</code></td>
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
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (342 - 349)</small></summary>

```php
protected function fromUtf8($string)
{
    if ($this->getEncoding() === 'utf-8') {
        return $string;
    }

    return $this->convertEncoding($string, $this->getEncoding(), 'UTF-8');
}
```

</details>


<hr>

#### isUtf8()

```php
protected function isUtf8($string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks if a given string appears to be valid UTF-8 or not.
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
<td><code>$string</code></td>
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (357 - 360)</small></summary>

```php
protected function isUtf8($string)
{
    return ($string === '' || preg_match('/^./su', $string));
}
```

</details>


<hr>

#### convertEncoding()

```php
protected function convertEncoding($string, $to, $from)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Encoding conversion helper which wraps iconv and mbstring where they exist or throws
and exception where neither is available.
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
<td><code>$string</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$to</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$from</code></td>
<td><em>array<br>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\Exception\RuntimeException
</td>
</tr>
</table>



<details>
<summary><small>Source: 19 lines (372 - 390)</small></summary>

```php
protected function convertEncoding($string, $to, $from)
{
    if (function_exists('iconv')) {
        $result = iconv($from, $to, $string);
    } elseif (function_exists('mb_convert_encoding')) {
        $result = mb_convert_encoding($string, $to, $from);
    } else {
        throw new Exception\RuntimeException(
            get_class($this)
            . ' requires either the iconv or mbstring extension to be installed'
            . ' when escaping for non UTF-8 strings.'
        );
    }

    if ($result === false) {
        return ''; // return non-fatal blank string on encoding errors from users
    }
    return $result;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/Escaper/Escaper.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/Utils.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Escaper/Exception/ExceptionInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>