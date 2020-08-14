


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/inflector_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/security_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/inflector_helper.md">next</a></td>
</tr>
</table>




 



# Inflector Helper


<hr>

## singular()

```php
function singular(string $string) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Singular
</td></tr>
</table>

<table>
<tr><td>
Takes a plural word and makes it singular
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
<td>Input string</td>
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
<summary><small>Source: 52 lines (58 - 109)</small></summary>

```php
function singular(string $string): string
{
	$result = strval($string);

	if (! is_pluralizable($result))
	{
		return $result;
	}

	//Arranged in order.
	$singularRules = [
		'/(matr)ices$/'                                                   => '\1ix',
		'/(vert|ind)ices$/'                                               => '\1ex',
		'/^(ox)en/'                                                       => '\1',
		'/(alias)es$/'                                                    => '\1',
		'/([octop|vir])i$/'                                               => '\1us',
		'/(cris|ax|test)es$/'                                             => '\1is',
		'/(shoe)s$/'                                                      => '\1',
		'/(o)es$/'                                                        => '\1',
		'/(bus|campus)es$/'                                               => '\1',
		'/([m|l])ice$/'                                                   => '\1ouse',
		'/(x|ch|ss|sh)es$/'                                               => '\1',
		'/(m)ovies$/'                                                     => '\1\2ovie',
		'/(s)eries$/'                                                     => '\1\2eries',
		'/([^aeiouy]|qu)ies$/'                                            => '\1y',
		'/([lr])ves$/'                                                    => '\1f',
		'/(tive)s$/'                                                      => '\1',
		'/(hive)s$/'                                                      => '\1',
		'/([^f])ves$/'                                                    => '\1fe',
		'/(^analy)ses$/'                                                  => '\1sis',
		'/((a)naly|(b)a|(d)iagno|(p)arenthe|(p)rogno|(s)ynop|(t)he)ses$/' => '\1\2sis',
		'/([ti])a$/'                                                      => '\1um',
		'/(p)eople$/'                                                     => '\1\2erson',
		'/(m)en$/'                                                        => '\1an',
		'/(s)tatuses$/'                                                   => '\1\2tatus',
		'/(c)hildren$/'                                                   => '\1\2hild',
		'/(n)ews$/'                                                       => '\1\2ews',
		'/(quiz)zes$/'                                                    => '\1',
		'/([^us])s$/'                                                     => '\1',
	];

	foreach ($singularRules as $rule => $replacement)
	{
		if (preg_match($rule, $result))
		{
			$result = preg_replace($rule, $replacement, $result);
			break;
		}
	}

	return $result;
}
```

</details>


<hr>

## plural()

```php
function plural(string $string) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Plural
</td></tr>
</table>

<table>
<tr><td>
Takes a singular word and makes it plural
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
<td>Input string</td>
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
<summary><small>Source: 43 lines (125 - 167)</small></summary>

```php
function plural(string $string): string
{
	$result = strval($string);

	if (! is_pluralizable($result))
	{
		return $result;
	}

	$pluralRules = [
		'/(quiz)$/'               => '\1zes',    // quizzes
		'/^(ox)$/'                => '\1\2en', // ox
		'/([m|l])ouse$/'          => '\1ice', // mouse, louse
		'/(matr|vert|ind)ix|ex$/' => '\1ices', // matrix, vertex, index
		'/(x|ch|ss|sh)$/'         => '\1es', // search, switch, fix, box, process, address
		'/([^aeiouy]|qu)y$/'      => '\1ies', // query, ability, agency
		'/(hive)$/'               => '\1s', // archive, hive
		'/(?:([^f])fe|([lr])f)$/' => '\1\2ves', // half, safe, wife
		'/sis$/'                  => 'ses', // basis, diagnosis
		'/([ti])um$/'             => '\1a', // datum, medium
		'/(p)erson$/'             => '\1eople', // person, salesperson
		'/(m)an$/'                => '\1en', // man, woman, spokesman
		'/(c)hild$/'              => '\1hildren', // child
		'/(buffal|tomat)o$/'      => '\1\2oes', // buffalo, tomato
		'/(bu|campu)s$/'          => '\1\2ses', // bus, campus
		'/(alias|status|virus)$/' => '\1es', // alias
		'/(octop)us$/'            => '\1i', // octopus
		'/(ax|cris|test)is$/'     => '\1es', // axis, crisis
		'/s$/'                    => 's', // no change (compatibility)
		'/$/'                     => 's',
	];

	foreach ($pluralRules as $rule => $replacement)
	{
		if (preg_match($rule, $result))
		{
			$result = preg_replace($rule, $replacement, $result);
			break;
		}
	}

	return $result;
}
```

</details>


<hr>

## counted()

```php
function counted(int $count, string $string) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Counted
</td></tr>
</table>

<table>
<tr><td>
Takes a number and a word to return the plural or not
E.g. 0 cats, 1 cat, 2 cats, ...
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
<td><code>$count</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Number of items</td>
</tr>

<tr>
<td>2.</td>
<td><code>$string</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Input string</td>
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
<summary><small>Source: 6 lines (185 - 190)</small></summary>

```php
function counted(int $count, string $string): string
{
	$result = "{$count} ";

	return $result . ($count === 1 ? singular($string) : plural($string));
}
```

</details>


<hr>

## camelize()

```php
function camelize(string $string) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Camelize
</td></tr>
</table>

<table>
<tr><td>
Takes multiple words separated by spaces or
underscores and converts them to camel case.
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
<td>Input string</td>
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
<summary><small>Source: 4 lines (206 - 209)</small></summary>

```php
function camelize(string $string): string
{
	return lcfirst(str_replace(' ', '', ucwords(preg_replace('/[\s_]+/', ' ', $string))));
}
```

</details>


<hr>

## pascalize()

```php
function pascalize(string $string) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Pascalize
</td></tr>
</table>

<table>
<tr><td>
Takes multiple words separated by spaces or
underscores and converts them to Pascal case,
which is camel case with an uppercase first letter.
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
<td>Input string</td>
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
<summary><small>Source: 4 lines (227 - 230)</small></summary>

```php
function pascalize(string $string): string
{
	return ucfirst(camelize($string));
}
```

</details>


<hr>

## underscore()

```php
function underscore(string $string) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Underscore
</td></tr>
</table>

<table>
<tr><td>
Takes multiple words separated by spaces and underscores them
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
<td>Input string</td>
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
<summary><small>Source: 6 lines (246 - 251)</small></summary>

```php
function underscore(string $string): string
{
	$replacement = trim($string);

	return preg_replace('/[\s]+/', '_', $replacement);
}
```

</details>


<hr>

## humanize()

```php
function humanize(string $string, string $separator = '_') : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Humanize
</td></tr>
</table>

<table>
<tr><td>
Takes multiple words separated by the separator,
camelizes and changes them to spaces
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
<td>Input string</td>
</tr>

<tr>
<td>2.</td>
<td><code>$separator</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Input separator</td>
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
<summary><small>Source: 9 lines (269 - 277)</small></summary>

```php
function humanize(string $string, string $separator = '_'): string
{
	$replacement = trim($string);

	return ucwords
			(
			preg_replace('/[' . $separator . ']+/', ' ', $replacement)
	);
}
```

</details>


<hr>

## is_pluralizable()

```php
function is_pluralizable(string $word) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks if the given word has a plural version.
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
<td><code>$word</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Word to check</td>
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
<summary><small>Source: 55 lines (291 - 345)</small></summary>

```php
function is_pluralizable(string $word): bool
{
	$uncountables = in_array
			(
		strtolower($word), [
					   'advice',
					   'bravery',
					   'butter',
					   'chaos',
					   'clarity',
					   'coal',
					   'courage',
					   'cowardice',
					   'curiosity',
					   'education',
					   'equipment',
					   'evidence',
					   'fish',
					   'fun',
					   'furniture',
					   'greed',
					   'help',
					   'homework',
					   'honesty',
					   'information',
					   'insurance',
					   'jewelry',
					   'knowledge',
					   'livestock',
					   'love',
					   'luck',
					   'marketing',
					   'meta',
					   'money',
					   'mud',
					   'news',
					   'patriotism',
					   'racism',
					   'rice',
					   'satisfaction',
					   'scenery',
					   'series',
					   'sexism',
					   'silence',
					   'species',
					   'spelling',
					   'sugar',
					   'water',
					   'weather',
					   'wisdom',
					   'work',
				   ]);

	return ! $uncountables;
}
```

</details>


<hr>

## dasherize()

```php
function dasherize(string $string) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replaces underscores with dashes in the string.
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
<td>Input string</td>
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
<summary><small>Source: 4 lines (359 - 362)</small></summary>

```php
function dasherize(string $string): string
{
	return str_replace('_', '-', $string);
}
```

</details>


<hr>

## ordinal()

```php
function ordinal(int $integer) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the suffix that should be added to a
number to denote the position in an ordered
sequence such as 1st, 2nd, 3rd, 4th.
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
<td><code>$integer</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The integer to determine the suffix</td>
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
<summary><small>Source: 17 lines (378 - 394)</small></summary>

```php
function ordinal(int $integer): string
{
	$suffixes = [
		'th',
		'st',
		'nd',
		'rd',
		'th',
		'th',
		'th',
		'th',
		'th',
		'th',
	];

	return $integer % 100 >= 11 && $integer % 100 <= 13 ? 'th' : $suffixes[$integer % 10];
}
```

</details>


<hr>

## ordinalize()

```php
function ordinalize(int $integer) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Turns a number into an ordinal string used
to denote the position in an ordered sequence
such as 1st, 2nd, 3rd, 4th.
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
<td><code>$integer</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The integer to ordinalize</td>
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
<summary><small>Source: 4 lines (410 - 413)</small></summary>

```php
function ordinalize(int $integer): string
{
	return $integer . ordinal($integer);
}
```

</details>







<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Helpers/inflector_helper.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/security_helper.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Helpers/inflector_helper.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:24**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>