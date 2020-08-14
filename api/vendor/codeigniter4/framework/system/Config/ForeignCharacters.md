


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Config/ForeignCharacters.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Services.md">next</a></td>
</tr>
</table>







# CodeIgniter\Config 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Config</td></tr>
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
<td>framework/system/Config/ForeignCharacters.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/AutoloadConfig.md">CodeIgniter\Config\AutoloadConfig</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseConfig.md">CodeIgniter\Config\BaseConfig</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/BaseService.md">CodeIgniter\Config\BaseService</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Config.md">CodeIgniter\Config\Config</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md">CodeIgniter\Config\DotEnv</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/ForeignCharacters.md">CodeIgniter\Config\ForeignCharacters</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Services.md">CodeIgniter\Config\Services</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/View.md">CodeIgniter\Config\View</a></td></tr>
</table>
</details>



 

 
## CodeIgniter\Config\ForeignCharacters

<table style="text-align:left">
<tr><th>Class</th><td>ForeignCharacters</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Config\ForeignCharacters</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Describes foreign characters for transliteration with the text helper.
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
<th><a href="#characterList"><strong>characterList</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Without further ado, the list of foreign characters.</td>
</tr>


</table>





### Properties


<hr>

#### $characterList

```php
public $characterList = [
	'/ä|æ|ǽ/'                                                     => 'ae',
	'/ö|œ/'                                                       => 'oe',
	'/ü/'                                                         => 'ue',
	'/Ä/'                                                         => 'Ae',
	'/Ü/'                                                         => 'Ue',
	'/Ö/'                                                         => 'Oe',
	'/À|Á|Â|Ã|Ä|Å|Ǻ|Ā|Ă|Ą|Ǎ|Α|Ά|Ả|Ạ|Ầ|Ẫ|Ẩ|Ậ|Ằ|Ắ|Ẵ|Ẳ|Ặ|А/'         => 'A',
	'/à|á|â|ã|å|ǻ|ā|ă|ą|ǎ|ª|α|ά|ả|ạ|ầ|ấ|ẫ|ẩ|ậ|ằ|ắ|ẵ|ẳ|ặ|а/'       => 'a',
	'/Б/'                                                         => 'B',
	'/б/'                                                         => 'b',
	'/Ç|Ć|Ĉ|Ċ|Č/'                                                 => 'C',
	'/ç|ć|ĉ|ċ|č/'                                                 => 'c',
	'/Д/'                                                         => 'D',
	'/д/'                                                         => 'd',
	'/Ð|Ď|Đ|Δ/'                                                   => 'Dj',
	'/ð|ď|đ|δ/'                                                   => 'dj',
	'/È|É|Ê|Ë|Ē|Ĕ|Ė|Ę|Ě|Ε|Έ|Ẽ|Ẻ|Ẹ|Ề|Ế|Ễ|Ể|Ệ|Е|Э/'                 => 'E',
	'/è|é|ê|ë|ē|ĕ|ė|ę|ě|έ|ε|ẽ|ẻ|ẹ|ề|ế|ễ|ể|ệ|е|э/'                 => 'e',
	'/Ф/'                                                         => 'F',
	'/ф/'                                                         => 'f',
	'/Ĝ|Ğ|Ġ|Ģ|Γ|Г|Ґ/'                                             => 'G',
	'/ĝ|ğ|ġ|ģ|γ|г|ґ/'                                             => 'g',
	'/Ĥ|Ħ/'                                                       => 'H',
	'/ĥ|ħ/'                                                       => 'h',
	'/Ì|Í|Î|Ï|Ĩ|Ī|Ĭ|Ǐ|Į|İ|Η|Ή|Ί|Ι|Ϊ|Ỉ|Ị|И|Ы/'                     => 'I',
	'/ì|í|î|ï|ĩ|ī|ĭ|ǐ|į|ı|η|ή|ί|ι|ϊ|ỉ|ị|и|ы|ї/'                   => 'i',
	'/Ĵ/'                                                         => 'J',
	'/ĵ/'                                                         => 'j',
	'/Ķ|Κ|К/'                                                     => 'K',
	'/ķ|κ|к/'                                                     => 'k',
	'/Ĺ|Ļ|Ľ|Ŀ|Ł|Λ|Л/'                                             => 'L',
	'/ĺ|ļ|ľ|ŀ|ł|λ|л/'                                             => 'l',
	'/М/'                                                         => 'M',
	'/м/'                                                         => 'm',
	'/Ñ|Ń|Ņ|Ň|Ν|Н/'                                               => 'N',
	'/ñ|ń|ņ|ň|ŉ|ν|н/'                                             => 'n',
	'/Ò|Ó|Ô|Õ|Ō|Ŏ|Ǒ|Ő|Ơ|Ø|Ǿ|Ο|Ό|Ω|Ώ|Ỏ|Ọ|Ồ|Ố|Ỗ|Ổ|Ộ|Ờ|Ớ|Ỡ|Ở|Ợ|О/'   => 'O',
	'/ò|ó|ô|õ|ō|ŏ|ǒ|ő|ơ|ø|ǿ|º|ο|ό|ω|ώ|ỏ|ọ|ồ|ố|ỗ|ổ|ộ|ờ|ớ|ỡ|ở|ợ|о/' => 'o',
	'/П/'                                                         => 'P',
	'/п/'                                                         => 'p',
	'/Ŕ|Ŗ|Ř|Ρ|Р/'                                                 => 'R',
	'/ŕ|ŗ|ř|ρ|р/'                                                 => 'r',
	'/Ś|Ŝ|Ş|Ș|Š|Σ|С/'                                             => 'S',
	'/ś|ŝ|ş|ș|š|ſ|σ|ς|с/'                                         => 's',
	'/Ț|Ţ|Ť|Ŧ|τ|Т/'                                               => 'T',
	'/ț|ţ|ť|ŧ|т/'                                                 => 't',
	'/Ù|Ú|Û|Ũ|Ū|Ŭ|Ů|Ű|Ų|Ư|Ǔ|Ǖ|Ǘ|Ǚ|Ǜ|Ũ|Ủ|Ụ|Ừ|Ứ|Ữ|Ử|Ự|У/'           => 'U',
	'/ù|ú|û|ũ|ū|ŭ|ů|ű|ų|ư|ǔ|ǖ|ǘ|ǚ|ǜ|υ|ύ|ϋ|ủ|ụ|ừ|ứ|ữ|ử|ự|у/'       => 'u',
	'/Ƴ|Ɏ|Ỵ|Ẏ|Ӳ|Ӯ|Ў|Ý|Ÿ|Ŷ|Υ|Ύ|Ϋ|Ỳ|Ỹ|Ỷ|Ỵ|Й/'                       => 'Y',
	'/ẙ|ʏ|ƴ|ɏ|ỵ|ẏ|ӳ|ӯ|ў|ý|ÿ|ŷ|ỳ|ỹ|ỷ|ỵ|й/'                         => 'y',
	'/В/'                                                         => 'V',
	'/в/'                                                         => 'v',
	'/Ŵ/'                                                         => 'W',
	'/ŵ/'                                                         => 'w',
	'/Ź|Ż|Ž|Ζ|З/'                                                 => 'Z',
	'/ź|ż|ž|ζ|з/'                                                 => 'z',
	'/Æ|Ǽ/'                                                       => 'AE',
	'/ß/'                                                         => 'ss',
	'/Ĳ/'                                                         => 'IJ',
	'/ĳ/'                                                         => 'ij',
	'/Œ/'                                                         => 'OE',
	'/ƒ/'                                                         => 'f',
	'/ξ/'                                                         => 'ks',
	'/π/'                                                         => 'p',
	'/β/'                                                         => 'v',
	'/μ/'                                                         => 'm',
	'/ψ/'                                                         => 'ps',
	'/Ё/'                                                         => 'Yo',
	'/ё/'                                                         => 'yo',
	'/Є/'                                                         => 'Ye',
	'/є/'                                                         => 'ye',
	'/Ї/'                                                         => 'Yi',
	'/Ж/'                                                         => 'Zh',
	'/ж/'                                                         => 'zh',
	'/Х/'                                                         => 'Kh',
	'/х/'                                                         => 'kh',
	'/Ц/'                                                         => 'Ts',
	'/ц/'                                                         => 'ts',
	'/Ч/'                                                         => 'Ch',
	'/ч/'                                                         => 'ch',
	'/Ш/'                                                         => 'Sh',
	'/ш/'                                                         => 'sh',
	'/Щ/'                                                         => 'Shch',
	'/щ/'                                                         => 'shch',
	'/Ъ|ъ|Ь|ь/'                                                   => '',
	'/Ю/'                                                         => 'Yu',
	'/ю/'                                                         => 'yu',
	'/Я/'                                                         => 'Ya',
	'/я/'                                                         => 'ya',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Without further ado, the list of foreign characters.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Config/ForeignCharacters.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/DotEnv.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Config/Services.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:08**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>