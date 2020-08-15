


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/CreditCardRules.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Typography/Typography.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md">next</a></td>
</tr>
</table>







# CodeIgniter\Validation 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Validation</td></tr>
</table>

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CodeIgniter
</td></tr>
</table>

<table>
<tr><td>
An open source application development framework for PHP

This content is released under the MIT License (MIT)

Copyright (c) 2014-2019 British Columbia Institute of Technology
Copyright (c) 2019-2020 CodeIgniter Foundation

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter
</td>
</tr>
<tr style="vertical-align:top;">
<th>author</th>
<td>CodeIgniter Dev Team
</td>
</tr>
<tr style="vertical-align:top;">
<th>copyright</th>
<td>2019-2020 CodeIgniter Foundation
</td>
</tr>
<tr style="vertical-align:top;">
<th>license</th>
<td><a href="https://opensource.org/licenses/MIT">https://opensource.org/licenses/MIT</a>	MIT License
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com">https://codeigniter.com</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>filesource</th>
<td>framework/system/Validation/CreditCardRules.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/CreditCardRules.md">CodeIgniter\Validation\CreditCardRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md">CodeIgniter\Validation\Exceptions\ValidationException</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FileRules.md">CodeIgniter\Validation\FileRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/FormatRules.md">CodeIgniter\Validation\FormatRules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Rules.md">CodeIgniter\Validation\Rules</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Validation.md">CodeIgniter\Validation\Validation</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md">CodeIgniter\Validation\ValidationInterface</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Validation\CreditCardRules

<table style="text-align:left">
<tr><th>Class</th><td>CreditCardRules</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Validation\CreditCardRules</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class CreditCardRules
</td></tr>
</table>

<table>
<tr><td>
Provides validation methods for common credit-card inputs.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\Validation
</td>
</tr>
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
<th><a href="#cards"><strong>cards</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The cards that we support, with the defining details:</td>
</tr>

<tr>
<th><a href="#valid_cc_number"><strong>valid_cc_number</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Verifies that a credit card number is valid and matches the known
formats for a wide number of credit card types. This does not verify
that the card is a valid card, only that the number is formatted correctly.</td>
</tr>
<tr>
<th><a href="#isValidLuhn"><strong>isValidLuhn</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Checks the given number to see if the number passing a Luhn check.</td>
</tr>

</table>





### Properties


<hr>

#### $cards

```php
protected $cards = [
	'American Express'                 => [
		'name'       => 'amex',
		'length'     => '15',
		'prefixes'   => '34,37',
		'checkdigit' => true,
	],
	'China UnionPay'                   => [
		'name'       => 'unionpay',
		'length'     => '16,17,18,19',
		'prefixes'   => '62',
		'checkdigit' => true,
	],
	'Dankort'                          => [
		'name'       => 'dankort',
		'length'     => '16',
		'prefixes'   => '5019,4175,4571,4',
		'checkdigit' => true,
	],
	'DinersClub'                       => [
		'name'       => 'dinersclub',
		'length'     => '14,16',
		'prefixes'   => '300,301,302,303,304,305,309,36,38,39,54,55',
		'checkdigit' => true,
	],
	'DinersClub CarteBlanche'          => [
		'name'       => 'carteblanche',
		'length'     => '14',
		'prefixes'   => '300,301,302,303,304,305',
		'checkdigit' => true,
	],
	'Discover Card'                    => [
		'name'       => 'discover',
		'length'     => '16,19',
		'prefixes'   => '6011,622,644,645,656,647,648,649,65',
		'checkdigit' => true,
	],
	'InterPayment'                     => [
		'name'       => 'interpayment',
		'length'     => '16,17,18,19',
		'prefixes'   => '4',
		'checkdigit' => true,
	],
	'JCB'                              => [
		'name'       => 'jcb',
		'length'     => '16,17,18,19',
		'prefixes'   => '352,353,354,355,356,357,358',
		'checkdigit' => true,
	],
	'Maestro'                          => [
		'name'       => 'maestro',
		'length'     => '12,13,14,15,16,18,19',
		'prefixes'   => '50,56,57,58,59,60,61,62,63,64,65,66,67,68,69',
		'checkdigit' => true,
	],
	'MasterCard'                       => [
		'name'       => 'mastercard',
		'length'     => '16',
		'prefixes'   => '51,52,53,54,55,22,23,24,25,26,27',
		'checkdigit' => true,
	],
	'NSPK MIR'                         => [
		'name'       => 'mir',
		'length'     => '16',
		'prefixes'   => '2200,2201,2202,2203,2204',
		'checkdigit' => true,
	],
	'Troy'                             => [
		'name'       => 'troy',
		'length'     => '16',
		'prefixes'   => '979200,979289',
		'checkdigit' => true,
	],
	'UATP'                             => [
		'name'       => 'uatp',
		'length'     => '15',
		'prefixes'   => '1',
		'checkdigit' => true,
	],
	'Verve'                            => [
		'name'       => 'verve',
		'length'     => '16,19',
		'prefixes'   => '506,650',
		'checkdigit' => true,
	],
	'Visa'                             => [
		'name'       => 'visa',
		'length'     => '13,16,19',
		'prefixes'   => '4',
		'checkdigit' => true,
	],
	// Canadian Cards
	'BMO ABM Card'                     => [
		'name'       => 'bmoabm',
		'length'     => '16',
		'prefixes'   => '500',
		'checkdigit' => false,
	],
	'CIBC Convenience Card'            => [
		'name'       => 'cibc',
		'length'     => '16',
		'prefixes'   => '4506',
		'checkdigit' => false,
	],
	'HSBC Canada Card'                 => [
		'name'       => 'hsbc',
		'length'     => '16',
		'prefixes'   => '56',
		'checkdigit' => false,
	],
	'Royal Bank of Canada Client Card' => [
		'name'       => 'rbc',
		'length'     => '16',
		'prefixes'   => '45',
		'checkdigit' => false,
	],
	'Scotiabank Scotia Card'           => [
		'name'       => 'scotia',
		'length'     => '16',
		'prefixes'   => '4536',
		'checkdigit' => false,
	],
	'TD Canada Trust Access Card'      => [
		'name'       => 'tdtrust',
		'length'     => '16',
		'prefixes'   => '589297',
		'checkdigit' => false,
	],
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The cards that we support, with the defining details:
</td></tr>
</table>

<table>
<tr><td>
name        - The type of card as found in the form. Must match the user's value
length      - List of possible lengths for the card number
prefixes    - List of possible prefixes for the card
checkdigit  - Boolean on whether we should do a modulus10 check on the numbers.
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

#### valid_cc_number()

```php
public function valid_cc_number(string $ccNumber = null, string $type) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Verifies that a credit card number is valid and matches the known
formats for a wide number of credit card types. This does not verify
that the card is a valid card, only that the number is formatted correctly.
</td></tr>
</table>

<table>
<tr><td>
Example:
$rules = [
    'cc_num' => 'valid_cc_number[visa]'
];
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
<td><code>$ccNumber</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$type</code></td>
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
<summary><small>Source: 73 lines (211 - 283)</small></summary>

```php
public function valid_cc_number(string $ccNumber = null, string $type): bool
{
	$type = strtolower($type);
	$info = null;

	// Get our card info based on provided name.
	foreach ($this->cards as $card)
	{
		if ($card['name'] === $type)
		{
			$info = $card;
			break;
		}
	}

	// If empty, it's not a card type we recognize, or invalid type.
	if (empty($info))
	{
		return false;
	}

	// Make sure we have a valid length
	if (strlen($ccNumber) === 0)
	{
		return false;
	}

	// Remove any spaces and dashes
	$ccNumber = str_replace([' ', '-'], '', $ccNumber);

	// Non-numeric values cannot be a number...duh
	if (! is_numeric($ccNumber))
	{
		return false;
	}

	// Make sure it's a valid length for this card
	$lengths = explode(',', $info['length']);

	if (! in_array(strlen($ccNumber), $lengths))
	{
		return false;
	}

	// Make sure it has a valid prefix
	$prefixes = explode(',', $info['prefixes']);

	$validPrefix = false;

	foreach ($prefixes as $prefix)
	{
		if (strpos($ccNumber, $prefix) === 0)
		{
						  $validPrefix = true;
						  break;
		}
	}

	if ($validPrefix === false)
	{
		return false;
	}

	// Still here? Then check the number against the Luhn algorithm, if required
	// @see https://en.wikipedia.org/wiki/Luhn_algorithm
	// @see https://gist.github.com/troelskn/1287893
	if ($info['checkdigit'] === true)
	{
		return $this->isValidLuhn($ccNumber);
	}

	return true;
}
```

</details>


<hr>

#### isValidLuhn()

```php
protected function isValidLuhn(string $number = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks the given number to see if the number passing a Luhn check.
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
<td><code>$number</code></td>
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
<summary><small>Source: 41 lines (294 - 334)</small></summary>

```php
protected function isValidLuhn(string $number = null): bool
{
	settype($number, 'string');

	$sumTable = [
		[
			0,
			1,
			2,
			3,
			4,
			5,
			6,
			7,
			8,
			9,
		],
		[
			0,
			2,
			4,
			6,
			8,
			1,
			3,
			5,
			7,
			9,
		],
	];

	$sum  = 0;
	$flip = 0;

	for ($i = strlen($number) - 1; $i >= 0; $i --)
	{
		$sum += $sumTable[$flip ++ & 0x1][$number[$i]];
	}

	return $sum % 10 === 0;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Validation/CreditCardRules.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Typography/Typography.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Validation/Exceptions/ValidationException.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-15 12:03:19**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>