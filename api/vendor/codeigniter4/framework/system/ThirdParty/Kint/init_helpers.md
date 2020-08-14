


 



<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/Kint/init_helpers.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Helpers/html_helper.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/init_helpers.md">next</a></td>
</tr>
</table>




 



# Init Helpers


<hr>

## d()

```php
function d()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alias of Kint::dump().
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (34 - 39)</small></summary>

```php
function d()
{
    $args = \func_get_args();

    return \call_user_func_array(array('Kint', 'dump'), $args);
}
```

</details>


<hr>

## s()

```php
function s()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alias of Kint::dump(), however the output is in plain text.
</td></tr>
</table>

<table>
<tr><td>
Alias of Kint::dump(), however the output is in plain htmlescaped text
with some minor visibility enhancements added.

If run in CLI mode, output is not escaped.

To force rendering mode without autodetecting anything:

Kint::$enabled_mode = Kint::MODE_PLAIN;
Kint::dump( $variable );
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int<br>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 22 lines (60 - 81)</small></summary>

```php
function s()
{
    if (!Kint::$enabled_mode) {
        return 0;
    }

    $stash = Kint::$enabled_mode;

    if (Kint::MODE_TEXT !== Kint::$enabled_mode) {
        Kint::$enabled_mode = Kint::MODE_PLAIN;
        if (PHP_SAPI === 'cli' && true === Kint::$cli_detection) {
            Kint::$enabled_mode = Kint::$mode_default_cli;
        }
    }

    $args = \func_get_args();
    $out = \call_user_func_array(array('Kint', 'dump'), $args);

    Kint::$enabled_mode = $stash;

    return $out;
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/ThirdParty/Kint/init_helpers.php</em></td>
<td><a href="../../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/Helpers/html_helper.md">prev</a></td>
<td><a href="../../../../../../../api/vendor/codeigniter4/framework/system/ThirdParty/Kint/init_helpers.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:04**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>