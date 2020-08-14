


 



<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/CLI.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CommandRunner.md">next</a></td>
</tr>
</table>







# CodeIgniter\CLI 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\CLI</td></tr>
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
<td>framework/system/CLI/CLI.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">CodeIgniter\CLI\BaseCommand</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CLI.md">CodeIgniter\CLI\CLI</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CommandRunner.md">CodeIgniter\CLI\CommandRunner</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Commands.md">CodeIgniter\CLI\Commands</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Console.md">CodeIgniter\CLI\Console</a></td></tr>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Exceptions/CLIException.md">CodeIgniter\CLI\Exceptions\CLIException</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/Exceptions/CLIException.md"><strong>CodeIgniter\CLI\Exceptions\CLIException</strong></a>
</td>
<td>CLIException</td>
</tr>
</table>



 
## CodeIgniter\CLI\CLI

<table style="text-align:left">
<tr><th>Class</th><td>CLI</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\CLI\CLI</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set of static methods useful for CLI request handling.
</td></tr>
</table>

<table>
<tr><td>
Portions of this code were initially from the FuelPHP Framework,
version 1.7.x, and used here under the MIT license they were
originally made available under. Reference: <a href="http://fuelphp.com">http://fuelphp.com</a>

Some of the code in this class is Windows-specific, and not
possible to test using travis-ci. It has been phpunit-annotated
to prevent messing up code coverage.

Some of the methods require keyboard input, and are not unit-testable
as a result: input() and prompt().
validate() is internal, and not testable if prompt() isn't.
The wait() method is mostly testable, as long as you don't give it
an argument of "0".
These have been flagged to ignore for code coverage purposes.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>package</th>
<td>CodeIgniter\CLI
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
<th><a href="#readline_support"><strong>readline_support</strong></a></th>
<td>prop</td>
<td>
public<br>static

</td>
<td>Is the readline library on the system?</td>
</tr>
<tr>
<th><a href="#wait_msg"><strong>wait_msg</strong></a></th>
<td>prop</td>
<td>
public<br>static

</td>
<td>The message displayed at prompts.</td>
</tr>
<tr>
<th><a href="#initialized"><strong>initialized</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Has the class already been initialized?</td>
</tr>
<tr>
<th><a href="#foreground_colors"><strong>foreground_colors</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Foreground color list</td>
</tr>
<tr>
<th><a href="#background_colors"><strong>background_colors</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Background color list</td>
</tr>
<tr>
<th><a href="#segments"><strong>segments</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>List of array segments.</td>
</tr>
<tr>
<th><a href="#options"><strong>options</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td></td>
</tr>
<tr>
<th><a href="#lastWrite"><strong>lastWrite</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Helps track internally whether the last
output was a &quot;write&quot; or a &quot;print&quot; to
keep the output clean and as expected.</td>
</tr>
<tr>
<th><a href="#height"><strong>height</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Height of the CLI window</td>
</tr>
<tr>
<th><a href="#width"><strong>width</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Width of the CLI window</td>
</tr>
<tr>
<th><a href="#isColored"><strong>isColored</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>Whether the current stream supports colored output.</td>
</tr>

<tr>
<th><a href="#init"><strong>init</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Static &quot;constructor&quot;.</td>
</tr>
<tr>
<th><a href="#input"><strong>input</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Get input from the shell, using readline or the standard STDIN</td>
</tr>
<tr>
<th><a href="#prompt"><strong>prompt</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Asks the user for input.</td>
</tr>
<tr>
<th><a href="#validate"><strong>validate</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Validate one prompt &quot;field&quot; at a time</td>
</tr>
<tr>
<th><a href="#print"><strong>print</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Outputs a string to the CLI without any surrounding newlines.</td>
</tr>
<tr>
<th><a href="#write"><strong>write</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Outputs a string to the cli on it&#039;s own line.</td>
</tr>
<tr>
<th><a href="#error"><strong>error</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Outputs an error to the CLI using STDERR instead of STDOUT</td>
</tr>
<tr>
<th><a href="#beep"><strong>beep</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Beeps a certain number of times.</td>
</tr>
<tr>
<th><a href="#wait"><strong>wait</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Waits a certain number of seconds, optionally showing a wait message and
waiting for a key press.</td>
</tr>
<tr>
<th><a href="#isWindows"><strong>isWindows</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>if operating system === windows</td>
</tr>
<tr>
<th><a href="#newLine"><strong>newLine</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Enter a number of empty lines</td>
</tr>
<tr>
<th><a href="#clearScreen"><strong>clearScreen</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Clears the screen of output</td>
</tr>
<tr>
<th><a href="#color"><strong>color</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns the given text with the correct color codes for a foreground and
optionally a background color.</td>
</tr>
<tr>
<th><a href="#strlen"><strong>strlen</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Get the number of characters in string having encoded characters
and ignores styles set by the color() function</td>
</tr>
<tr>
<th><a href="#streamSupports"><strong>streamSupports</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Checks whether the current stream resource supports or
refers to a valid terminal type device.</td>
</tr>
<tr>
<th><a href="#hasColorSupport"><strong>hasColorSupport</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns true if the stream resource supports colors.</td>
</tr>
<tr>
<th><a href="#getWidth"><strong>getWidth</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Attempts to determine the width of the viewable CLI window.</td>
</tr>
<tr>
<th><a href="#getHeight"><strong>getHeight</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Attempts to determine the height of the viewable CLI window.</td>
</tr>
<tr>
<th><a href="#generateDimensions"><strong>generateDimensions</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Populates the CLI&#039;s dimensions.</td>
</tr>
<tr>
<th><a href="#showProgress"><strong>showProgress</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Displays a progress bar on the CLI. You must call it repeatedly
to update it. Set $thisStep = false to erase the progress bar.</td>
</tr>
<tr>
<th><a href="#wrap"><strong>wrap</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Takes a string and writes it to the command line, wrapping to a maximum
width. If no maximum width is specified, will wrap to the window&#039;s max
width.</td>
</tr>
<tr>
<th><a href="#parseCommandLine"><strong>parseCommandLine</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Parses the command line it was called from and collects all
options and valid segments.</td>
</tr>
<tr>
<th><a href="#getURI"><strong>getURI</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns the command line string portions of the arguments, minus
any options, as a string. This is used to pass along to the main
CodeIgniter application.</td>
</tr>
<tr>
<th><a href="#getSegment"><strong>getSegment</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns an individual segment.</td>
</tr>
<tr>
<th><a href="#getSegments"><strong>getSegments</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns the raw array of segments found.</td>
</tr>
<tr>
<th><a href="#getOption"><strong>getOption</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Gets a single command-line option. Returns TRUE if the option
exists, but doesn&#039;t have a value, and is simply acting as a flag.</td>
</tr>
<tr>
<th><a href="#getOptions"><strong>getOptions</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns the raw array of options found.</td>
</tr>
<tr>
<th><a href="#getOptionString"><strong>getOptionString</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns the options as a string, suitable for passing along on
the CLI to other commands.</td>
</tr>
<tr>
<th><a href="#table"><strong>table</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Returns a well formatted table</td>
</tr>
<tr>
<th><a href="#fwrite"><strong>fwrite</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>While the library is intended for use on CLI commands,
commands can be called from controllers and elsewhere
so we need a way to allow them to still work.</td>
</tr>

</table>





### Properties


<hr>

#### $readline_support

```php
public static $readline_support = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Is the readline library on the system?
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>bool
</td>
</tr>
</table>


<hr>

#### $wait_msg

```php
public static $wait_msg = 'Press any key to continue...';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The message displayed at prompts.
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

#### $initialized

```php
protected static $initialized = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Has the class already been initialized?
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>bool
</td>
</tr>
</table>


<hr>

#### $foreground_colors

```php
protected static $foreground_colors = [
	'black'        => '0;30',
	'dark_gray'    => '1;30',
	'blue'         => '0;34',
	'dark_blue'    => '0;34',
	'light_blue'   => '1;34',
	'green'        => '0;32',
	'light_green'  => '1;32',
	'cyan'         => '0;36',
	'light_cyan'   => '1;36',
	'red'          => '0;31',
	'light_red'    => '1;31',
	'purple'       => '0;35',
	'light_purple' => '1;35',
	'yellow'       => '0;33',
	'light_yellow' => '1;33',
	'light_gray'   => '0;37',
	'white'        => '1;37',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Foreground color list
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

#### $background_colors

```php
protected static $background_colors = [
	'black'      => '40',
	'red'        => '41',
	'green'      => '42',
	'yellow'     => '43',
	'blue'       => '44',
	'magenta'    => '45',
	'cyan'       => '46',
	'light_gray' => '47',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Background color list
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

#### $segments

```php
protected static $segments = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
List of array segments.
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

#### $options

```php
protected static $options = [];
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
<td>array
</td>
</tr>
</table>


<hr>

#### $lastWrite

```php
protected static $lastWrite;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Helps track internally whether the last
output was a "write" or a "print" to
keep the output clean and as expected.
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

#### $height

```php
protected static $height;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Height of the CLI window
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

#### $width

```php
protected static $width;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Width of the CLI window
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

#### $isColored

```php
protected static $isColored = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether the current stream supports colored output.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>bool
</td>
</tr>
</table>







### Methods


<hr>

#### init()

```php
public static function init()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Static "constructor".
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 29 lines (176 - 204)</small></summary>

```php
public static function init()
{
	if (is_cli())
	{
		// Readline is an extension for PHP that makes interactivity with PHP
		// much more bash-like.
		// http://www.php.net/manual/en/readline.installation.php
		static::$readline_support = extension_loaded('readline');

		// clear segments & options to keep testing clean
		static::$segments = [];
		static::$options  = [];

		// Check our stream resource for color support
		static::$isColored = static::hasColorSupport(STDOUT);

		static::parseCommandLine();

		static::$initialized = true;
	}
	else
	{
		// If the command is being called from a controller
		// we need to define STDOUT ourselves
		// @codeCoverageIgnoreStart
		define('STDOUT', 'php://output');
		// @codeCoverageIgnoreEnd
	}
}
```

</details>


<hr>

#### input()

```php
public static function input(string $prefix = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get input from the shell, using readline or the standard STDIN
</td></tr>
</table>

<table>
<tr><td>
Named options must be in the following formats:
php index.php user -v --v -name=John --name=John
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
</td>
</tr>
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
<td><code>$prefix</code></td>
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
<summary><small>Source: 11 lines (219 - 229)</small></summary>

```php
public static function input(string $prefix = null): string
{
	if (static::$readline_support)
	{
		return readline($prefix);
	}

	echo $prefix;

	return fgets(STDIN);
}
```

</details>


<hr>

#### prompt()

```php
public static function prompt(string $field, $options = null, string $validation = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Asks the user for input.
</td></tr>
</table>

<table>
<tr><td>
Usage:

// Takes any input
$color = CLI::prompt('What is your favorite color?');

// Takes any input, but offers default
$color = CLI::prompt('What is your favourite color?', 'white');

// Will validate options with the in_list rule and accept only if one of the list
$color = CLI::prompt('What is your favourite color?', array('red','blue'));

// Do not provide options but requires a valid email
$email = CLI::prompt('What is your email?', null, 'required|valid_email');
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
</td>
</tr>
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
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Output "field" question</td>
</tr>

<tr>
<td>2.</td>
<td><code>$options</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>String to a default value, array to a list of options (the first option will be the default value)</td>
</tr>

<tr>
<td>3.</td>
<td><code>$validation</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Validation rules</td>
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
<summary><small>Source: 47 lines (258 - 304)</small></summary>

```php
public static function prompt(string $field, $options = null, string $validation = null): string
{
	$extra_output = '';
	$default      = '';

	if (is_string($options))
	{
		$extra_output = ' [' . static::color($options, 'white') . ']';
		$default      = $options;
	}

	if (is_array($options) && $options)
	{
		$opts                 = $options;
		$extra_output_default = static::color($opts[0], 'white');

		unset($opts[0]);

		if (empty($opts))
		{
			$extra_output = $extra_output_default;
		}
		else
		{
			$extra_output = ' [' . $extra_output_default . ', ' . implode(', ', $opts) . ']';
			$validation  .= '|in_list[' . implode(',', $options) . ']';
			$validation   = trim($validation, '|');
		}

		$default = $options[0];
	}

	static::fwrite(STDOUT, $field . $extra_output . ': ');

	// Read the input from keyboard.
	$input = trim(static::input()) ?: $default;

	if (isset($validation))
	{
		while (! static::validate($field, $input, $validation))
		{
			$input = static::prompt($field, $options, $validation);
		}
	}

	return empty($input) ? '' : $input;
}
```

</details>


<hr>

#### validate()

```php
protected static function validate(string $field, string $value, string $rules) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validate one prompt "field" at a time
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
</td>
</tr>
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
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Prompt "field" output</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Input value</td>
</tr>

<tr>
<td>3.</td>
<td><code>$rules</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Validation rules</td>
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
<summary><small>Source: 17 lines (319 - 335)</small></summary>

```php
protected static function validate(string $field, string $value, string $rules): bool
{
	$label      = $field;
	$field      = 'temp';
	$validation = \Config\Services::validation(null, false);
	$validation->setRule($field, $label, $rules);
	$validation->run([$field => $value]);

	if ($validation->hasError($field))
	{
		static::error($validation->getError($field));

		return false;
	}

	return true;
}
```

</details>


<hr>

#### print()

```php
public static function print(string $text = '', string $foreground = null, string $background = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Outputs a string to the CLI without any surrounding newlines.
</td></tr>
</table>

<table>
<tr><td>
Useful for showing repeating elements on a single line.
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
<td><code>$text</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$foreground</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$background</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 11 lines (347 - 357)</small></summary>

```php
public static function print(string $text = '', string $foreground = null, string $background = null)
{
	if ($foreground || $background)
	{
		$text = static::color($text, $foreground, $background);
	}

	static::$lastWrite = null;

	static::fwrite(STDOUT, $text);
}
```

</details>


<hr>

#### write()

```php
public static function write(string $text = '', string $foreground = null, string $background = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Outputs a string to the cli on it's own line.
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
<td><code>$text</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The text to output</td>
</tr>

<tr>
<td>2.</td>
<td><code>$foreground</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$background</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 15 lines (366 - 380)</small></summary>

```php
public static function write(string $text = '', string $foreground = null, string $background = null)
{
	if ($foreground || $background)
	{
		$text = static::color($text, $foreground, $background);
	}

	if (static::$lastWrite !== 'write')
	{
		$text              = PHP_EOL . $text;
		static::$lastWrite = 'write';
	}

	static::fwrite(STDOUT, $text . PHP_EOL);
}
```

</details>


<hr>

#### error()

```php
public static function error(string $text, string $foreground = 'light_red', string $background = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Outputs an error to the CLI using STDERR instead of STDOUT
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
<td><code>$text</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td>The text to output, or array of errors</td>
</tr>

<tr>
<td>2.</td>
<td><code>$foreground</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$background</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 16 lines (391 - 406)</small></summary>

```php
public static function error(string $text, string $foreground = 'light_red', string $background = null)
{
	// Check color support for STDERR
	$stdout            = static::$isColored;
	static::$isColored = static::hasColorSupport(STDERR);

	if ($foreground || $background)
	{
		$text = static::color($text, $foreground, $background);
	}

	static::fwrite(STDERR, $text . PHP_EOL);

	// return STDOUT color support
	static::$isColored = $stdout;
}
```

</details>


<hr>

#### beep()

```php
public static function beep(int $num = 1)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Beeps a certain number of times.
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
<td><code>$num</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The number of times to beep</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (415 - 418)</small></summary>

```php
public static function beep(int $num = 1)
{
	echo str_repeat("\x07", $num);
}
```

</details>


<hr>

#### wait()

```php
public static function wait(int $seconds, bool $countdown = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Waits a certain number of seconds, optionally showing a wait message and
waiting for a key press.
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
<td><code>$seconds</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Number of seconds</td>
</tr>

<tr>
<td>2.</td>
<td><code>$countdown</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Show a countdown or not</td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 30 lines (429 - 458)</small></summary>

```php
public static function wait(int $seconds, bool $countdown = false)
{
	if ($countdown === true)
	{
		$time = $seconds;

		while ($time > 0)
		{
			static::fwrite(STDOUT, $time . '... ');
			sleep(1);
			$time --;
		}
		static::write();
	}
	else
	{
		if ($seconds > 0)
		{
			sleep($seconds);
		}
		else
		{
			// this chunk cannot be tested because of keyboard input
			// @codeCoverageIgnoreStart
			static::write(static::$wait_msg);
			static::input();
			// @codeCoverageIgnoreEnd
		}
	}
}
```

</details>


<hr>

#### isWindows()

```php
public static function isWindows() : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
if operating system === windows
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (467 - 470)</small></summary>

```php
public static function isWindows(): bool
{
	return stripos(PHP_OS, 'WIN') === 0;
}
```

</details>


<hr>

#### newLine()

```php
public static function newLine(int $num = 1)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Enter a number of empty lines
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
<td><code>$num</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Number of lines to output</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (481 - 488)</small></summary>

```php
public static function newLine(int $num = 1)
{
	// Do it once or more, write with empty string gives us a new line
	for ($i = 0; $i < $num; $i ++)
	{
		static::write();
	}
}
```

</details>


<hr>

#### clearScreen()

```php
public static function clearScreen()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Clears the screen of output
</td></tr>
</table>


</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>codeCoverageIgnore</th>
<td>
</td>
</tr>
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (499 - 506)</small></summary>

```php
public static function clearScreen()
{
	// Unix systems, and Windows with VT100 Terminal support (i.e. Win10)
	// can handle CSI sequences. For lower than Win10 we just shove in 40 new lines.
	static::isWindows() && ! static::streamSupports('sapi_windows_vt100_support', STDOUT)
		? static::newLine(40)
		: static::fwrite(STDOUT, "\033[H\033[2J");
}
```

</details>


<hr>

#### color()

```php
public static function color(string $text, string $foreground, string $background = null, string $format = null) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the given text with the correct color codes for a foreground and
optionally a background color.
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
<td><code>$text</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The text to color</td>
</tr>

<tr>
<td>2.</td>
<td><code>$foreground</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The foreground color</td>
</tr>

<tr>
<td>3.</td>
<td><code>$background</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The background color</td>
</tr>

<tr>
<td>4.</td>
<td><code>$format</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Other formatting to apply. Currently only 'underline' is understood</td>
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
<summary><small>Source: 61 lines (521 - 581)</small></summary>

```php
public static function color(string $text, string $foreground, string $background = null, string $format = null): string
{
	if (! static::$isColored)
	{
		return $text;
	}

	if (! array_key_exists($foreground, static::$foreground_colors))
	{
		throw CLIException::forInvalidColor('foreground', $foreground);
	}

	if ($background !== null && ! array_key_exists($background, static::$background_colors))
	{
		throw CLIException::forInvalidColor('background', $background);
	}

	$string = "\033[" . static::$foreground_colors[$foreground] . 'm';

	if ($background !== null)
	{
		$string .= "\033[" . static::$background_colors[$background] . 'm';
	}

	if ($format === 'underline')
	{
		$string .= "\033[4m";
	}

	// Detect if color method was already in use with this text
	if (strpos($text, "\033[0m") !== false)
	{
		// Split the text into parts so that we can see
		// if any part missing the color definition
		$chunks = mb_split("\\033\[0m", $text);
		// Reset text
		$text = '';

		foreach ($chunks as $chunk)
		{
			if ($chunk === '')
			{
				continue;
			}

			// If chunk doesn't have colors defined we need to add them
			if (strpos($chunk, "\033[") === false)
			{
				$chunk = static::color($chunk, $foreground, $background, $format);
				// Add color reset before chunk and clear end of the string
				$text .= rtrim("\033[0m" . $chunk, "\033[0m");
			}
			else
			{
				$text .= $chunk;
			}
		}
	}

	return $string . $text . "\033[0m";
}
```

</details>


<hr>

#### strlen()

```php
public static function strlen(?string $string) : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get the number of characters in string having encoded characters
and ignores styles set by the color() function
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
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 21 lines (593 - 613)</small></summary>

```php
public static function strlen(?string $string): int
{
	if (is_null($string))
	{
		return 0;
	}

	foreach (static::$foreground_colors as $color)
	{
		$string = strtr($string, ["\033[" . $color . 'm' => '']);
	}

	foreach (static::$background_colors as $color)
	{
		$string = strtr($string, ["\033[" . $color . 'm' => '']);
	}

	$string = strtr($string, ["\033[4m" => '', "\033[0m" => '']);

	return mb_strlen($string);
}
```

</details>


<hr>

#### streamSupports()

```php
public static function streamSupports(string $function, $resource) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks whether the current stream resource supports or
refers to a valid terminal type device.
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
<td><code>$function</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$resource</code></td>
<td><em>resource
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
<summary><small>Source: 14 lines (626 - 639)</small></summary>

```php
public static function streamSupports(string $function, $resource): bool
{
	if (ENVIRONMENT === 'testing')
	{
		// In the current setup of the tests we cannot fully check
		// if the stream supports the function since we are using
		// filtered streams.
		return function_exists($function);
	}

	// @codeCoverageIgnoreStart
	return function_exists($function) && @$function($resource);
	// @codeCoverageIgnoreEnd
}
```

</details>


<hr>

#### hasColorSupport()

```php
public static function hasColorSupport($resource) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns true if the stream resource supports colors.
</td></tr>
</table>

<table>
<tr><td>
This is tricky on Windows, because Cygwin, Msys2 etc. emulate pseudo
terminals via named pipes, so we can only check the environment.

Reference: <a href="https://github.com/composer/xdebug-handler/blob/master/src/Process.php">https://github.com/composer/xdebug-handler/blob/master/src/Process.php</a>
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
<td><code>$resource</code></td>
<td><em>resource
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
<summary><small>Source: 26 lines (655 - 680)</small></summary>

```php
public static function hasColorSupport($resource): bool
{
	// Follow https://no-color.org/
	if (isset($_SERVER['NO_COLOR']) || getenv('NO_COLOR') !== false)
	{
		return false;
	}

	if (getenv('TERM_PROGRAM') === 'Hyper')
	{
		return true;
	}

	if (static::isWindows())
	{
		// @codeCoverageIgnoreStart
		return static::streamSupports('sapi_windows_vt100_support', $resource)
			|| isset($_SERVER['ANSICON'])
			|| getenv('ANSICON') !== false
			|| getenv('ConEmuANSI') === 'ON'
			|| getenv('TERM') === 'xterm';
		// @codeCoverageIgnoreEnd
	}

	return static::streamSupports('stream_isatty', $resource);
}
```

</details>


<hr>

#### getWidth()

```php
public static function getWidth(int $default = 80) : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to determine the width of the viewable CLI window.
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
<td><code>$default</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (691 - 699)</small></summary>

```php
public static function getWidth(int $default = 80): int
{
	if (\is_null(static::$width))
	{
		static::generateDimensions();
	}

	return static::$width ?: $default;
}
```

</details>


<hr>

#### getHeight()

```php
public static function getHeight(int $default = 32) : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attempts to determine the height of the viewable CLI window.
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
<td><code>$default</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (710 - 718)</small></summary>

```php
public static function getHeight(int $default = 32): int
{
	if (\is_null(static::$height))
	{
		static::generateDimensions();
	}

	return static::$height ?: $default;
}
```

</details>


<hr>

#### generateDimensions()

```php
public static function generateDimensions()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Populates the CLI's dimensions.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 47 lines (727 - 773)</small></summary>

```php
public static function generateDimensions()
{
	if (static::isWindows())
	{
		// Shells such as `Cygwin` and `Git bash` returns incorrect values
		// when executing `mode CON`, so we use `tput` instead
		// @codeCoverageIgnoreStart
		if (($shell = getenv('SHELL')) && preg_match('/(?:bash|zsh)(?:\.exe)?$/', $shell) || getenv('TERM'))
		{
			static::$height = (int) exec('tput lines');
			static::$width  = (int) exec('tput cols');
		}
		else
		{
			$return = -1;
			$output = [];
			exec('mode CON', $output, $return);

			if ($return === 0 && $output)
			{
				// Look for the next lines ending in ": <number>"
				// Searching for "Columns:" or "Lines:" will fail on non-English locales
				if (preg_match('/:\s*(\d+)\n[^:]+:\s*(\d+)\n/', implode("\n", $output), $matches))
				{
					static::$height = (int) $matches[1];
					static::$width  = (int) $matches[2];
				}
			}
		}
		// @codeCoverageIgnoreEnd
	}
	else
	{
		if (($size = exec('stty size')) && preg_match('/(\d+)\s+(\d+)/', $size, $matches))
		{
			static::$height = (int) $matches[1];
			static::$width  = (int) $matches[2];
		}
		else
		{
			// @codeCoverageIgnoreStart
			static::$height = (int) exec('tput lines');
			static::$width  = (int) exec('tput cols');
			// @codeCoverageIgnoreEnd
		}
	}
}
```

</details>


<hr>

#### showProgress()

```php
public static function showProgress($thisStep = 1, int $totalSteps = 10)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Displays a progress bar on the CLI. You must call it repeatedly
to update it. Set $thisStep = false to erase the progress bar.
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
<td><code>$thisStep</code></td>
<td><em>int<br>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$totalSteps</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 30 lines (784 - 813)</small></summary>

```php
public static function showProgress($thisStep = 1, int $totalSteps = 10)
{
	static $inProgress = false;

	// restore cursor position when progress is continuing.
	if ($inProgress !== false && $inProgress <= $thisStep)
	{
		static::fwrite(STDOUT, "\033[1A");
	}
	$inProgress = $thisStep;

	if ($thisStep !== false)
	{
		// Don't allow div by zero or negative numbers....
		$thisStep   = abs($thisStep);
		$totalSteps = $totalSteps < 1 ? 1 : $totalSteps;

		$percent = intval(($thisStep / $totalSteps) * 100);
		$step    = (int) round($percent / 10);

		// Write the progress bar
		static::fwrite(STDOUT, "[\033[32m" . str_repeat('#', $step) . str_repeat('.', 10 - $step) . "\033[0m]");
		// Textual representation...
		static::fwrite(STDOUT, sprintf(' %3d%% Complete', $percent) . PHP_EOL);
	}
	else
	{
		static::fwrite(STDOUT, "\007");
	}
}
```

</details>


<hr>

#### wrap()

```php
public static function wrap(string $string = null, int $max = 0, int $pad_left = 0) : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes a string and writes it to the command line, wrapping to a maximum
width. If no maximum width is specified, will wrap to the window's max
width.
</td></tr>
</table>

<table>
<tr><td>
If an int is passed into $pad_left, then all strings after the first
will padded with that many spaces to the left. Useful when printing
short descriptions that need to start on an existing line.
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
<td><code>$max</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$pad_left</code></td>
<td><em>int
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
<summary><small>Source: 43 lines (832 - 874)</small></summary>

```php
public static function wrap(string $string = null, int $max = 0, int $pad_left = 0): string
{
	if (empty($string))
	{
		return '';
	}

	if ($max === 0)
	{
		$max = CLI::getWidth();
	}

	if (CLI::getWidth() < $max)
	{
		$max = CLI::getWidth();
	}

	$max = $max - $pad_left;

	$lines = wordwrap($string, $max, PHP_EOL);

	if ($pad_left > 0)
	{
		$lines = explode(PHP_EOL, $lines);

		$first = true;

		array_walk($lines, function (&$line, $index) use ($pad_left, &$first) {
			if (! $first)
			{
				$line = str_repeat(' ', $pad_left) . $line;
			}
			else
			{
				$first = false;
			}
		});

		$lines = implode(PHP_EOL, $lines);
	}

	return $lines;
}
```

</details>


<hr>

#### parseCommandLine()

```php
protected static function parseCommandLine()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Parses the command line it was called from and collects all
options and valid segments.
</td></tr>
</table>

<table>
<tr><td>
I tried to use getopt but had it fail occasionally to find any
options but argc has always had our back. We don't have all of the power
of getopt but this does us just fine.
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 26 lines (889 - 914)</small></summary>

```php
protected static function parseCommandLine()
{
	// start picking segments off from #1, ignoring the invoking program
	for ($i = 1; $i < $_SERVER['argc']; $i ++)
	{
		// If there's no '-' at the beginning of the argument
		// then add it to our segments.
		if (mb_strpos($_SERVER['argv'][$i], '-') !== 0)
		{
			static::$segments[] = $_SERVER['argv'][$i];
			continue;
		}

		$arg   = ltrim($_SERVER['argv'][$i], '-');
		$value = null;

		// if there is a following segment, and it doesn't start with a dash, it's a value.
		if (isset($_SERVER['argv'][$i + 1]) && mb_strpos($_SERVER['argv'][$i + 1], '-') !== 0)
		{
			$value = $_SERVER['argv'][$i + 1];
			$i ++;
		}

		static::$options[$arg] = $value;
	}
}
```

</details>


<hr>

#### getURI()

```php
public static function getURI() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the command line string portions of the arguments, minus
any options, as a string. This is used to pass along to the main
CodeIgniter application.
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
<summary><small>Source: 4 lines (925 - 928)</small></summary>

```php
public static function getURI(): string
{
	return implode('/', static::$segments);
}
```

</details>


<hr>

#### getSegment()

```php
public static function getSegment(int $index)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns an individual segment.
</td></tr>
</table>

<table>
<tr><td>
This ignores any options that might have been dispersed between
valid segments in the command:

 // segment(3) is 'three', not '-f' or 'anOption'
 > php spark one two -f anOption three
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
<td><code>$index</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (945 - 953)</small></summary>

```php
public static function getSegment(int $index)
{
	if (! isset(static::$segments[$index - 1]))
	{
		return null;
	}

	return static::$segments[$index - 1];
}
```

</details>


<hr>

#### getSegments()

```php
public static function getSegments() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the raw array of segments found.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (962 - 965)</small></summary>

```php
public static function getSegments(): array
{
	return static::$segments;
}
```

</details>


<hr>

#### getOption()

```php
public static function getOption(string $name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Gets a single command-line option. Returns TRUE if the option
exists, but doesn't have a value, and is simply acting as a flag.
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
<td><code>$name</code></td>
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
<td>bool<br>mixed<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 13 lines (977 - 989)</small></summary>

```php
public static function getOption(string $name)
{
	if (! array_key_exists($name, static::$options))
	{
		return null;
	}

	// If the option didn't have a value, simply return TRUE
	// so they know it was set, otherwise return the actual value.
	$val = static::$options[$name] === null ? true : static::$options[$name];

	return $val;
}
```

</details>


<hr>

#### getOptions()

```php
public static function getOptions() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the raw array of options found.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (998 - 1001)</small></summary>

```php
public static function getOptions(): array
{
	return static::$options;
}
```

</details>


<hr>

#### getOptionString()

```php
public static function getOptionString() : string
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the options as a string, suitable for passing along on
the CLI to other commands.
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
<summary><small>Source: 23 lines (1011 - 1033)</small></summary>

```php
public static function getOptionString(): string
{
	if (empty(static::$options))
	{
		return '';
	}

	$out = '';

	foreach (static::$options as $name => $value)
	{
		// If there's a space, we need to group
		// so it will pass correctly.
		if (mb_strpos($value, ' ') !== false)
		{
			$value = '"' . $value . '"';
		}

		$out .= "-{$name} $value ";
	}

	return $out;
}
```

</details>


<hr>

#### table()

```php
public static function table(array $tbody, array $thead = array())
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns a well formatted table
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
<td><code>$tbody</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>List of rows</td>
</tr>

<tr>
<td>2.</td>
<td><code>$thead</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>List of columns</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 93 lines (1045 - 1137)</small></summary>

```php
public static function table(array $tbody, array $thead = [])
{
	// All the rows in the table will be here until the end
	$table_rows = [];

	// We need only indexes and not keys
	if (! empty($thead))
	{
		$table_rows[] = array_values($thead);
	}

	foreach ($tbody as $tr)
	{
		$table_rows[] = array_values($tr);
	}

	// Yes, it really is necessary to know this count
	$total_rows = count($table_rows);

	// Store all columns lengths
	// $all_cols_lengths[row][column] = length
	$all_cols_lengths = [];

	// Store maximum lengths by column
	// $max_cols_lengths[column] = length
	$max_cols_lengths = [];

	// Read row by row and define the longest columns
	for ($row = 0; $row < $total_rows; $row ++)
	{
		$column = 0; // Current column index
		foreach ($table_rows[$row] as $col)
		{
			// Sets the size of this column in the current row
			$all_cols_lengths[$row][$column] = static::strlen($col);

			// If the current column does not have a value among the larger ones
			// or the value of this is greater than the existing one
			// then, now, this assumes the maximum length
			if (! isset($max_cols_lengths[$column]) || $all_cols_lengths[$row][$column] > $max_cols_lengths[$column])
			{
				$max_cols_lengths[$column] = $all_cols_lengths[$row][$column];
			}

			// We can go check the size of the next column...
			$column ++;
		}
	}

	// Read row by row and add spaces at the end of the columns
	// to match the exact column length
	for ($row = 0; $row < $total_rows; $row ++)
	{
		$column = 0;
		foreach ($table_rows[$row] as $col)
		{
			$diff = $max_cols_lengths[$column] - static::strlen($col);
			if ($diff)
			{
				$table_rows[$row][$column] = $table_rows[$row][$column] . str_repeat(' ', $diff);
			}
			$column ++;
		}
	}

	$table = '';

	// Joins columns and append the well formatted rows to the table
	for ($row = 0; $row < $total_rows; $row ++)
	{
		// Set the table border-top
		if ($row === 0)
		{
			$cols = '+';
			foreach ($table_rows[$row] as $col)
			{
				$cols .= str_repeat('-', static::strlen($col) + 2) . '+';
			}
			$table .= $cols . PHP_EOL;
		}

		// Set the columns borders
		$table .= '| ' . implode(' | ', $table_rows[$row]) . ' |' . PHP_EOL;

		// Set the thead and table borders-bottom
		if ($row === 0 && ! empty($thead) || $row + 1 === $total_rows)
		{
			$table .= $cols . PHP_EOL;
		}
	}

	static::write($table);
}
```

</details>


<hr>

#### fwrite()

```php
protected static function fwrite($handle, string $string)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
While the library is intended for use on CLI commands,
commands can be called from controllers and elsewhere
so we need a way to allow them to still work.
</td></tr>
</table>

<table>
<tr><td>
For now, just echo the content, but look into a better
solution down the road.
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
<td><code>$handle</code></td>
<td><em>resource
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 12 lines (1154 - 1165)</small></summary>

```php
protected static function fwrite($handle, string $string)
{
	if (! is_cli())
	{
		// @codeCoverageIgnoreStart
		echo $string;
		return;
		// @codeCoverageIgnoreEnd
	}

	fwrite($handle, $string);
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/CLI/CLI.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/BaseCommand.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/CLI/CommandRunner.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:07**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>