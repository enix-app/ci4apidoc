


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Email/Email.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Views.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/EncrypterInterface.md">next</a></td>
</tr>
</table>







# CodeIgniter\Email 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter\Email</td></tr>
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

Copyright (c) 2014 - 2019, British Columbia Institute of Technology
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
<td>EllisLab Dev Team
</td>
</tr>
<tr style="vertical-align:top;">
<th>copyright</th>
<td>Copyright (c) 2008 - 2014, EllisLab, Inc. (<a href="https://ellislab.com">https://ellislab.com</a>/)
</td>
</tr>
<tr style="vertical-align:top;">
<th>copyright</th>
<td>Copyright (c) 2014 - 2019, British Columbia Institute of Technology (<a href="http://bcit.ca">http://bcit.ca</a>/)
</td>
</tr>
<tr style="vertical-align:top;">
<th>license</th>
<td><a href="http://opensource.org/licenses/MIT">http://opensource.org/licenses/MIT</a>    MIT License
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com">https://codeigniter.com</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>filesource</th>
<td>framework/system/Email/Email.php
</td>
</tr>
</table>

 

<details>
<summary style="margin-bottom:12px;"><strong>Members</strong></summary>
<table>
<tr><td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Email/Email.md">CodeIgniter\Email\Email</a></td></tr>
</table>
</details>



 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<a href="../../../../../../api/vendor/codeigniter4/framework/system/Events/Events.md"><strong>CodeIgniter\Events\Events</strong></a>
</td>
<td>Events</td>
</tr>
<tr>
<td>
<strong>Config\Mimes</strong>
</td>
<td>Mimes</td>
</tr>
</table>



 
## CodeIgniter\Email\Email

<table style="text-align:left">
<tr><th>Class</th><td>Email</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Email\Email</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CodeIgniter Email Class
</td></tr>
</table>

<table>
<tr><td>
Permits email to be sent using Mail, Sendmail, or SMTP.
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
<th>subpackage</th>
<td>Libraries
</td>
</tr>
<tr style="vertical-align:top;">
<th>category</th>
<td>Libraries
</td>
</tr>
<tr style="vertical-align:top;">
<th>author</th>
<td>EllisLab Dev Team
</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://codeigniter.com/user_guide/libraries/email.html">https://codeigniter.com/user_guide/libraries/email.html</a>

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
<th><a href="#archive"><strong>archive</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Properties from the last successful send.</td>
</tr>
<tr>
<th><a href="#tmpArchive"><strong>tmpArchive</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Properties to be added to the next archive.</td>
</tr>
<tr>
<th><a href="#fromEmail"><strong>fromEmail</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#fromName"><strong>fromName</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td></td>
</tr>
<tr>
<th><a href="#userAgent"><strong>userAgent</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Used as the User-Agent and X-Mailer headers&#039; value.</td>
</tr>
<tr>
<th><a href="#mailPath"><strong>mailPath</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Path to the Sendmail binary.</td>
</tr>
<tr>
<th><a href="#protocol"><strong>protocol</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Which method to use for sending e-mails.</td>
</tr>
<tr>
<th><a href="#SMTPHost"><strong>SMTPHost</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>STMP Server host</td>
</tr>
<tr>
<th><a href="#SMTPUser"><strong>SMTPUser</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>SMTP Username</td>
</tr>
<tr>
<th><a href="#SMTPPass"><strong>SMTPPass</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>SMTP Password</td>
</tr>
<tr>
<th><a href="#SMTPPort"><strong>SMTPPort</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>SMTP Server port</td>
</tr>
<tr>
<th><a href="#SMTPTimeout"><strong>SMTPTimeout</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>SMTP connection timeout in seconds</td>
</tr>
<tr>
<th><a href="#SMTPKeepAlive"><strong>SMTPKeepAlive</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>SMTP persistent connection</td>
</tr>
<tr>
<th><a href="#SMTPCrypto"><strong>SMTPCrypto</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>SMTP Encryption</td>
</tr>
<tr>
<th><a href="#wordWrap"><strong>wordWrap</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Whether to apply word-wrapping to the message body.</td>
</tr>
<tr>
<th><a href="#wrapChars"><strong>wrapChars</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Number of characters to wrap at.</td>
</tr>
<tr>
<th><a href="#mailType"><strong>mailType</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Message format.</td>
</tr>
<tr>
<th><a href="#charset"><strong>charset</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Character set (default: utf-8)</td>
</tr>
<tr>
<th><a href="#altMessage"><strong>altMessage</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Alternative message (for HTML messages only)</td>
</tr>
<tr>
<th><a href="#validate"><strong>validate</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Whether to validate e-mail addresses.</td>
</tr>
<tr>
<th><a href="#priority"><strong>priority</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>X-Priority header value.</td>
</tr>
<tr>
<th><a href="#newline"><strong>newline</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Newline character sequence.</td>
</tr>
<tr>
<th><a href="#CRLF"><strong>CRLF</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>CRLF character sequence</td>
</tr>
<tr>
<th><a href="#DSN"><strong>DSN</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Whether to use Delivery Status Notification.</td>
</tr>
<tr>
<th><a href="#sendMultipart"><strong>sendMultipart</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Whether to send multipart alternatives.</td>
</tr>
<tr>
<th><a href="#BCCBatchMode"><strong>BCCBatchMode</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Whether to send messages to BCC recipients in batches.</td>
</tr>
<tr>
<th><a href="#BCCBatchSize"><strong>BCCBatchSize</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>BCC Batch max number size.</td>
</tr>
<tr>
<th><a href="#subject"><strong>subject</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Subject header</td>
</tr>
<tr>
<th><a href="#body"><strong>body</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Message body</td>
</tr>
<tr>
<th><a href="#finalBody"><strong>finalBody</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Final message body to be sent.</td>
</tr>
<tr>
<th><a href="#headerStr"><strong>headerStr</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Final headers to send</td>
</tr>
<tr>
<th><a href="#SMTPConnect"><strong>SMTPConnect</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>SMTP Connection socket placeholder</td>
</tr>
<tr>
<th><a href="#encoding"><strong>encoding</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Mail encoding</td>
</tr>
<tr>
<th><a href="#SMTPAuth"><strong>SMTPAuth</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether to perform SMTP authentication</td>
</tr>
<tr>
<th><a href="#replyToFlag"><strong>replyToFlag</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether to send a Reply-To header</td>
</tr>
<tr>
<th><a href="#debugMessage"><strong>debugMessage</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Debug messages</td>
</tr>
<tr>
<th><a href="#recipients"><strong>recipients</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Recipients</td>
</tr>
<tr>
<th><a href="#CCArray"><strong>CCArray</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>CC Recipients</td>
</tr>
<tr>
<th><a href="#BCCArray"><strong>BCCArray</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>BCC Recipients</td>
</tr>
<tr>
<th><a href="#headers"><strong>headers</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Message headers</td>
</tr>
<tr>
<th><a href="#attachments"><strong>attachments</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Attachment data</td>
</tr>
<tr>
<th><a href="#protocols"><strong>protocols</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Valid $protocol values</td>
</tr>
<tr>
<th><a href="#baseCharsets"><strong>baseCharsets</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Base charsets</td>
</tr>
<tr>
<th><a href="#bitDepths"><strong>bitDepths</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Bit depths</td>
</tr>
<tr>
<th><a href="#priorities"><strong>priorities</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>$priority translations</td>
</tr>
<tr>
<th><a href="#func_overload"><strong>func_overload</strong></a></th>
<td>prop</td>
<td>
protected<br>static

</td>
<td>mbstring.func_overload flag</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Constructor - Sets Email Preferences</td>
</tr>
<tr>
<th><a href="#initialize"><strong>initialize</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Initialize preferences</td>
</tr>
<tr>
<th><a href="#clear"><strong>clear</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Initialize the Email Data</td>
</tr>
<tr>
<th><a href="#setFrom"><strong>setFrom</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set FROM</td>
</tr>
<tr>
<th><a href="#setReplyTo"><strong>setReplyTo</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Reply-to</td>
</tr>
<tr>
<th><a href="#setTo"><strong>setTo</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Recipients</td>
</tr>
<tr>
<th><a href="#setCC"><strong>setCC</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set CC</td>
</tr>
<tr>
<th><a href="#setBCC"><strong>setBCC</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set BCC</td>
</tr>
<tr>
<th><a href="#setSubject"><strong>setSubject</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Email Subject</td>
</tr>
<tr>
<th><a href="#setMessage"><strong>setMessage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Body</td>
</tr>
<tr>
<th><a href="#attach"><strong>attach</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Assign file attachments</td>
</tr>
<tr>
<th><a href="#setAttachmentCID"><strong>setAttachmentCID</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set and return attachment Content-ID</td>
</tr>
<tr>
<th><a href="#setHeader"><strong>setHeader</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Add a Header Item</td>
</tr>
<tr>
<th><a href="#stringToArray"><strong>stringToArray</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Convert a String to an Array</td>
</tr>
<tr>
<th><a href="#setAltMessage"><strong>setAltMessage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Multipart Value</td>
</tr>
<tr>
<th><a href="#setMailType"><strong>setMailType</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Mailtype</td>
</tr>
<tr>
<th><a href="#setWordWrap"><strong>setWordWrap</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Wordwrap</td>
</tr>
<tr>
<th><a href="#setProtocol"><strong>setProtocol</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Protocol</td>
</tr>
<tr>
<th><a href="#setPriority"><strong>setPriority</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Priority</td>
</tr>
<tr>
<th><a href="#setNewline"><strong>setNewline</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set Newline Character</td>
</tr>
<tr>
<th><a href="#setCRLF"><strong>setCRLF</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set CRLF</td>
</tr>
<tr>
<th><a href="#getMessageID"><strong>getMessageID</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get the Message ID</td>
</tr>
<tr>
<th><a href="#getProtocol"><strong>getProtocol</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get Mail Protocol</td>
</tr>
<tr>
<th><a href="#getEncoding"><strong>getEncoding</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get Mail Encoding</td>
</tr>
<tr>
<th><a href="#getContentType"><strong>getContentType</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get content type (text/html/attachment)</td>
</tr>
<tr>
<th><a href="#setDate"><strong>setDate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Set RFC 822 Date</td>
</tr>
<tr>
<th><a href="#getMimeMessage"><strong>getMimeMessage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Mime message</td>
</tr>
<tr>
<th><a href="#validateEmail"><strong>validateEmail</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Validate Email Address</td>
</tr>
<tr>
<th><a href="#isValidEmail"><strong>isValidEmail</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Email Validation</td>
</tr>
<tr>
<th><a href="#cleanEmail"><strong>cleanEmail</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Clean Extended Email Address: Joe Smith &lt;joe@smith.com&gt;</td>
</tr>
<tr>
<th><a href="#getAltMessage"><strong>getAltMessage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Build alternative plain text message</td>
</tr>
<tr>
<th><a href="#wordWrap"><strong>wordWrap</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Word Wrap</td>
</tr>
<tr>
<th><a href="#buildHeaders"><strong>buildHeaders</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Build final headers</td>
</tr>
<tr>
<th><a href="#writeHeaders"><strong>writeHeaders</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Write Headers as a string</td>
</tr>
<tr>
<th><a href="#buildMessage"><strong>buildMessage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Build Final Body and attachments</td>
</tr>
<tr>
<th><a href="#attachmentsHaveMultipart"><strong>attachmentsHaveMultipart</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td></td>
</tr>
<tr>
<th><a href="#appendAttachments"><strong>appendAttachments</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Prepares attachment string</td>
</tr>
<tr>
<th><a href="#prepQuotedPrintable"><strong>prepQuotedPrintable</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Prep Quoted Printable</td>
</tr>
<tr>
<th><a href="#prepQEncoding"><strong>prepQEncoding</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Prep Q Encoding</td>
</tr>
<tr>
<th><a href="#send"><strong>send</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Send Email</td>
</tr>
<tr>
<th><a href="#batchBCCSend"><strong>batchBCCSend</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Batch Bcc Send. Sends groups of BCCs in batches</td>
</tr>
<tr>
<th><a href="#unwrapSpecials"><strong>unwrapSpecials</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Unwrap special elements</td>
</tr>
<tr>
<th><a href="#removeNLCallback"><strong>removeNLCallback</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Strip line-breaks via callback</td>
</tr>
<tr>
<th><a href="#spoolEmail"><strong>spoolEmail</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Spool mail to the mail server</td>
</tr>
<tr>
<th><a href="#validateEmailForShell"><strong>validateEmailForShell</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Validate email for shell</td>
</tr>
<tr>
<th><a href="#sendWithMail"><strong>sendWithMail</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Send using mail()</td>
</tr>
<tr>
<th><a href="#sendWithSendmail"><strong>sendWithSendmail</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Send using Sendmail</td>
</tr>
<tr>
<th><a href="#sendWithSmtp"><strong>sendWithSmtp</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Send using SMTP</td>
</tr>
<tr>
<th><a href="#SMTPEnd"><strong>SMTPEnd</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>SMTP End</td>
</tr>
<tr>
<th><a href="#SMTPConnect"><strong>SMTPConnect</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>SMTP Connect</td>
</tr>
<tr>
<th><a href="#sendCommand"><strong>sendCommand</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Send SMTP command</td>
</tr>
<tr>
<th><a href="#SMTPAuthenticate"><strong>SMTPAuthenticate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>SMTP Authenticate</td>
</tr>
<tr>
<th><a href="#sendData"><strong>sendData</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Send SMTP data</td>
</tr>
<tr>
<th><a href="#getSMTPData"><strong>getSMTPData</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get SMTP data</td>
</tr>
<tr>
<th><a href="#getHostname"><strong>getHostname</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Get Hostname</td>
</tr>
<tr>
<th><a href="#printDebugger"><strong>printDebugger</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Get Debug Message</td>
</tr>
<tr>
<th><a href="#setErrorMessage"><strong>setErrorMessage</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Set Message</td>
</tr>
<tr>
<th><a href="#mimeTypes"><strong>mimeTypes</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Mime Types</td>
</tr>
<tr>
<th><a href="#__destruct"><strong>__destruct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Destructor</td>
</tr>
<tr>
<th><a href="#strlen"><strong>strlen</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Byte-safe strlen()</td>
</tr>
<tr>
<th><a href="#substr"><strong>substr</strong>()</a></th>
<td>method</td>
<td>
protected<br>static

</td>
<td>Byte-safe substr()</td>
</tr>
<tr>
<th><a href="#setArchiveValues"><strong>setArchiveValues</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Determines the values that should be stored in $archive.</td>
</tr>

</table>





### Properties


<hr>

#### $archive

```php
public $archive;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Properties from the last successful send.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>array<br>null
</td>
</tr>
</table>


<hr>

#### $tmpArchive

```php
protected $tmpArchive = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Properties to be added to the next archive.
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

#### $fromEmail

```php
public $fromEmail;
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
<td>string
</td>
</tr>
</table>


<hr>

#### $fromName

```php
public $fromName;
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
<td>string
</td>
</tr>
</table>


<hr>

#### $userAgent

```php
public $userAgent = 'CodeIgniter';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used as the User-Agent and X-Mailer headers' value.
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

#### $mailPath

```php
public $mailPath = '/usr/sbin/sendmail';    // Sendmail path
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Path to the Sendmail binary.
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

#### $protocol

```php
public $protocol = 'mail';        // mail/sendmail/smtp
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Which method to use for sending e-mails.
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

#### $SMTPHost

```php
public $SMTPHost = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
STMP Server host
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

#### $SMTPUser

```php
public $SMTPUser = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP Username
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

#### $SMTPPass

```php
public $SMTPPass = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP Password
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

#### $SMTPPort

```php
public $SMTPPort = 25;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP Server port
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

#### $SMTPTimeout

```php
public $SMTPTimeout = 5;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP connection timeout in seconds
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

#### $SMTPKeepAlive

```php
public $SMTPKeepAlive = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP persistent connection
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

#### $SMTPCrypto

```php
public $SMTPCrypto = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP Encryption
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

#### $wordWrap

```php
public $wordWrap = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to apply word-wrapping to the message body.
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

#### $wrapChars

```php
public $wrapChars = 76;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Number of characters to wrap at.
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

#### $mailType

```php
public $mailType = 'text';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Message format.
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

#### $charset

```php
public $charset = 'utf-8';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Character set (default: utf-8)
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

#### $altMessage

```php
public $altMessage = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Alternative message (for HTML messages only)
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

#### $validate

```php
public $validate = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to validate e-mail addresses.
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

#### $priority

```php
public $priority = 3;            // Default priority (1 - 5)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
X-Priority header value.
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

#### $newline

```php
public $newline = "\n";            // Default newline. "\r\n" or "\n" (Use "\r\n" to comply with RFC 822)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Newline character sequence.
</td></tr>
</table>

<table>
<tr><td>
Use "\r\n" to comply with RFC 822.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="http://www.ietf.org/rfc/rfc822.txt">http://www.ietf.org/rfc/rfc822.txt</a>

</td>
</tr>
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>string
</td>
</tr>
</table>


<hr>

#### $CRLF

```php
public $CRLF = "\n";
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CRLF character sequence
</td></tr>
</table>

<table>
<tr><td>
RFC 2045 specifies that for 'quoted-printable' encoding,
"\r\n" must be used. However, it appears that some servers
(even on the receiving end) don't handle it properly and
switching to "\n", while improper, is the only solution
that seems to work for all environments.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="http://www.ietf.org/rfc/rfc822.txt">http://www.ietf.org/rfc/rfc822.txt</a>

</td>
</tr>
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>string
</td>
</tr>
</table>


<hr>

#### $DSN

```php
public $DSN = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to use Delivery Status Notification.
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

#### $sendMultipart

```php
public $sendMultipart = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to send multipart alternatives.
</td></tr>
</table>

<table>
<tr><td>
Yahoo! doesn't seem to like these.
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

#### $BCCBatchMode

```php
public $BCCBatchMode = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to send messages to BCC recipients in batches.
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

#### $BCCBatchSize

```php
public $BCCBatchSize = 200;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
BCC Batch max number size.
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

#### $subject

```php
protected $subject = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Subject header
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

#### $body

```php
protected $body = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Message body
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

#### $finalBody

```php
protected $finalBody = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Final message body to be sent.
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

#### $headerStr

```php
protected $headerStr = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Final headers to send
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

#### $SMTPConnect

```php
protected $SMTPConnect = '';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP Connection socket placeholder
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>resource
</td>
</tr>
</table>


<hr>

#### $encoding

```php
protected $encoding = '8bit';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Mail encoding
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

#### $SMTPAuth

```php
protected $SMTPAuth = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to perform SMTP authentication
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

#### $replyToFlag

```php
protected $replyToFlag = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to send a Reply-To header
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

#### $debugMessage

```php
protected $debugMessage = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Debug messages
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

#### $recipients

```php
protected $recipients = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Recipients
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

#### $CCArray

```php
protected $CCArray = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
CC Recipients
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

#### $BCCArray

```php
protected $BCCArray = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
BCC Recipients
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

#### $headers

```php
protected $headers = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Message headers
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

#### $attachments

```php
protected $attachments = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Attachment data
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

#### $protocols

```php
protected $protocols = [
	'mail',
	'sendmail',
	'smtp',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Valid $protocol values
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

#### $baseCharsets

```php
protected $baseCharsets = [
	'us-ascii',
	'iso-2022-',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Base charsets
</td></tr>
</table>

<table>
<tr><td>
Character sets valid for 7-bit encoding,
excluding language suffix.
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

#### $bitDepths

```php
protected $bitDepths = [
	'7bit',
	'8bit',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Bit depths
</td></tr>
</table>

<table>
<tr><td>
Valid mail encodings
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

#### $priorities

```php
protected $priorities = [
	1 => '1 (Highest)',
	2 => '2 (High)',
	3 => '3 (Normal)',
	4 => '4 (Low)',
	5 => '5 (Lowest)',
];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
$priority translations
</td></tr>
</table>

<table>
<tr><td>
Actual values to send with the X-Priority header
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

#### $func_overload

```php
protected static $func_overload;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
mbstring.func_overload flag
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

#### __construct()

```php
public function __construct($config = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Constructor - Sets Email Preferences
</td></tr>
</table>

<table>
<tr><td>
The constructor can be passed an array of config values
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
<td><code>$config</code></td>
<td><em>array<br>null
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 5 lines (377 - 381)</small></summary>

```php
public function __construct($config = null)
{
	$this->initialize($config);
	isset(static::$func_overload) || static::$func_overload = (extension_loaded('mbstring') && ini_get('mbstring.func_overload'));
}
```

</details>


<hr>

#### initialize()

```php
public function initialize($config)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Initialize preferences
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
<td><code>$config</code></td>
<td><em>array<br>\Config\Email
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 26 lines (390 - 415)</small></summary>

```php
public function initialize($config)
{
	$this->clear();
	if ($config instanceof \Config\Email)
	{
		$config = get_object_vars($config);
	}
	foreach (get_class_vars(get_class($this)) as $key => $value)
	{
		if (property_exists($this, $key) && isset($config[$key]))
		{
			$method = 'set' . ucfirst($key);
			if (method_exists($this, $method))
			{
				$this->$method($config[$key]);
			}
			else
			{
				$this->$key = $config[$key];
			}
		}
	}
	$this->charset  = strtoupper($this->charset);
	$this->SMTPAuth = isset($this->SMTPUser[0], $this->SMTPPass[0]);
	return $this;
}
```

</details>


<hr>

#### clear()

```php
public function clear($clearAttachments = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Initialize the Email Data
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
<td><code>$clearAttachments</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 19 lines (424 - 442)</small></summary>

```php
public function clear($clearAttachments = false)
{
	$this->subject      = '';
	$this->body         = '';
	$this->finalBody    = '';
	$this->headerStr    = '';
	$this->replyToFlag  = false;
	$this->recipients   = [];
	$this->CCArray      = [];
	$this->BCCArray     = [];
	$this->headers      = [];
	$this->debugMessage = [];
	$this->setHeader('Date', $this->setDate());
	if ($clearAttachments !== false)
	{
		$this->attachments = [];
	}
	return $this;
}
```

</details>


<hr>

#### setFrom()

```php
public function setFrom($from, $name = '', $returnPath = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set FROM
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
<td><code>$from</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$name</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$returnPath</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td>Return-Path</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 40 lines (453 - 492)</small></summary>

```php
public function setFrom($from, $name = '', $returnPath = null)
{
	if (preg_match('/\<(.*)\>/', $from, $match))
	{
		$from = $match[1];
	}
	if ($this->validate)
	{
		$this->validateEmail($this->stringToArray($from));
		if ($returnPath)
		{
			$this->validateEmail($this->stringToArray($returnPath));
		}
	}

	// Store the plain text values
	$this->tmpArchive['fromEmail'] = $from;
	$this->tmpArchive['fromName']  = $name;

	// prepare the display name
	if ($name !== '')
	{
		// only use Q encoding if there are characters that would require it
		if (! preg_match('/[\200-\377]/', $name))
		{
			// add slashes for non-printing characters, slashes, and double quotes, and surround it in double quotes
			$name = '"' . addcslashes($name, "\0..\37\177'\"\\") . '"';
		}
		else
		{
			$name = $this->prepQEncoding($name);
		}
	}
	$this->setHeader('From', $name . ' <' . $from . '>');
	isset($returnPath) || $returnPath = $from;
	$this->setHeader('Return-Path', '<' . $returnPath . '>');
	$this->tmpArchive['returnPath'] = $returnPath;

	return $this;
}
```

</details>


<hr>

#### setReplyTo()

```php
public function setReplyTo($replyto, $name = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Reply-to
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
<td><code>$replyto</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 31 lines (502 - 532)</small></summary>

```php
public function setReplyTo($replyto, $name = '')
{
	if (preg_match('/\<(.*)\>/', $replyto, $match))
	{
		$replyto = $match[1];
	}
	if ($this->validate)
	{
		$this->validateEmail($this->stringToArray($replyto));
	}
	if ($name !== '')
	{
		$this->tmpArchive['replyName'] = $name;

		// only use Q encoding if there are characters that would require it
		if (! preg_match('/[\200-\377]/', $name))
		{
			// add slashes for non-printing characters, slashes, and double quotes, and surround it in double quotes
			$name = '"' . addcslashes($name, "\0..\37\177'\"\\") . '"';
		}
		else
		{
			$name = $this->prepQEncoding($name);
		}
	}
	$this->setHeader('Reply-To', $name . ' <' . $replyto . '>');
	$this->replyToFlag           = true;
	$this->tmpArchive['replyTo'] = $replyto;

	return $this;
}
```

</details>


<hr>

#### setTo()

```php
public function setTo($to)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Recipients
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
<td><code>$to</code></td>
<td><em>string<br>array
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (541 - 555)</small></summary>

```php
public function setTo($to)
{
	$to = $this->stringToArray($to);
	$to = $this->cleanEmail($to);
	if ($this->validate)
	{
		$this->validateEmail($to);
	}
	if ($this->getProtocol() !== 'mail')
	{
		$this->setHeader('To', implode(', ', $to));
	}
	$this->recipients = $to;
	return $this;
}
```

</details>


<hr>

#### setCC()

```php
public function setCC($cc)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set CC
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
<td><code>$cc</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (564 - 578)</small></summary>

```php
public function setCC($cc)
{
	$cc = $this->cleanEmail($this->stringToArray($cc));
	if ($this->validate)
	{
		$this->validateEmail($cc);
	}
	$this->setHeader('Cc', implode(', ', $cc));
	if ($this->getProtocol() === 'smtp')
	{
		$this->CCArray = $cc;
	}
	$this->tmpArchive['CCArray'] = $cc;
	return $this;
}
```

</details>


<hr>

#### setBCC()

```php
public function setBCC($bcc, $limit = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set BCC
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
<td><code>$bcc</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$limit</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 23 lines (588 - 610)</small></summary>

```php
public function setBCC($bcc, $limit = '')
{
	if ($limit !== '' && is_numeric($limit))
	{
		$this->BCCBatchMode = true;
		$this->BCCBatchSize = $limit;
	}
	$bcc = $this->cleanEmail($this->stringToArray($bcc));
	if ($this->validate)
	{
		$this->validateEmail($bcc);
	}
	if ($this->getProtocol() === 'smtp' || ($this->BCCBatchMode && count($bcc) > $this->BCCBatchSize))
	{
		$this->BCCArray = $bcc;
	}
	else
	{
		$this->setHeader('Bcc', implode(', ', $bcc));
		$this->tmpArchive['BCCArray'] = $bcc;
	}
	return $this;
}
```

</details>


<hr>

#### setSubject()

```php
public function setSubject($subject)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Email Subject
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
<td><code>$subject</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (619 - 626)</small></summary>

```php
public function setSubject($subject)
{
	$this->tmpArchive['subject'] = $subject;

	$subject = $this->prepQEncoding($subject);
	$this->setHeader('Subject', $subject);
	return $this;
}
```

</details>


<hr>

#### setMessage()

```php
public function setMessage($body)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Body
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
<td><code>$body</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (635 - 639)</small></summary>

```php
public function setMessage($body)
{
	$this->body = rtrim(str_replace("\r", '', $body));
	return $this;
}
```

</details>


<hr>

#### attach()

```php
public function attach($file, $disposition = '', $newname = null, $mime = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Assign file attachments
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
<td><code>$file</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Can be local path, URL or buffered content</td>
</tr>

<tr>
<td>2.</td>
<td><code>$disposition</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>'attachment'</td>
</tr>

<tr>
<td>3.</td>
<td><code>$newname</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$mime</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 37 lines (651 - 687)</small></summary>

```php
public function attach($file, $disposition = '', $newname = null, $mime = '')
{
	if ($mime === '')
	{
		if (strpos($file, '://') === false && ! is_file($file))
		{
			$this->setErrorMessage(lang('Email.attachmentMissing', [$file]));
			return false;
		}
		if (! $fp = @fopen($file, 'rb'))
		{
			$this->setErrorMessage(lang('Email.attachmentUnreadable', [$file]));
			return false;
		}
		$fileContent = stream_get_contents($fp);
		$mime        = $this->mimeTypes(pathinfo($file, PATHINFO_EXTENSION));
		fclose($fp);
	}
	else
	{
		$fileContent = & $file; // buffered file
	}
	// declare names on their own, to make phpcbf happy
	$namesAttached       = [
		$file,
		$newname,
	];
	$this->attachments[] = [
		'name'        => $namesAttached,
		'disposition' => empty($disposition) ? 'attachment' : $disposition,
	// Can also be 'inline'  Not sure if it matters
		'type'        => $mime,
		'content'     => chunk_split(base64_encode($fileContent)),
		'multipart'   => 'mixed',
	];
	return $this;
}
```

</details>


<hr>

#### setAttachmentCID()

```php
public function setAttachmentCID($filename)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set and return attachment Content-ID
</td></tr>
</table>

<table>
<tr><td>
Useful for attached inline pictures
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
<td><code>$filename</code></td>
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
<summary><small>Source: 13 lines (698 - 710)</small></summary>

```php
public function setAttachmentCID($filename)
{
	for ($i = 0, $c = count($this->attachments); $i < $c; $i ++)
	{
		if ($this->attachments[$i]['name'][0] === $filename)
		{
			$this->attachments[$i]['multipart'] = 'related';
			$this->attachments[$i]['cid']       = uniqid(basename($this->attachments[$i]['name'][0]) . '@', true);
			return $this->attachments[$i]['cid'];
		}
	}
	return false;
}
```

</details>


<hr>

#### setHeader()

```php
public function setHeader($header, $value)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Add a Header Item
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
<td><code>$header</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (720 - 724)</small></summary>

```php
public function setHeader($header, $value)
{
	$this->headers[$header] = str_replace(["\n", "\r"], '', $value);
	return $this;
}
```

</details>


<hr>

#### stringToArray()

```php
protected function stringToArray($email)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Convert a String to an Array
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
<td><code>$email</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (733 - 740)</small></summary>

```php
protected function stringToArray($email)
{
	if (! is_array($email))
	{
		return (strpos($email, ',') !== false) ? preg_split('/[\s,]/', $email, -1, PREG_SPLIT_NO_EMPTY) : (array) trim($email);
	}
	return $email;
}
```

</details>


<hr>

#### setAltMessage()

```php
public function setAltMessage($str)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Multipart Value
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
<td><code>$str</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (749 - 753)</small></summary>

```php
public function setAltMessage($str)
{
	$this->altMessage = (string) $str;
	return $this;
}
```

</details>


<hr>

#### setMailType()

```php
public function setMailType($type = 'text')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Mailtype
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (762 - 766)</small></summary>

```php
public function setMailType($type = 'text')
{
	$this->mailType = ($type === 'html') ? 'html' : 'text';
	return $this;
}
```

</details>


<hr>

#### setWordWrap()

```php
public function setWordWrap($wordWrap = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Wordwrap
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
<td><code>$wordWrap</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (775 - 779)</small></summary>

```php
public function setWordWrap($wordWrap = true)
{
	$this->wordWrap = (bool) $wordWrap;
	return $this;
}
```

</details>


<hr>

#### setProtocol()

```php
public function setProtocol($protocol = 'mail')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Protocol
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
<td><code>$protocol</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (788 - 792)</small></summary>

```php
public function setProtocol($protocol = 'mail')
{
	$this->protocol = in_array($protocol, $this->protocols, true) ? strtolower($protocol) : 'mail';
	return $this;
}
```

</details>


<hr>

#### setPriority()

```php
public function setPriority($n = 3)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Priority
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
<td><code>$n</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (801 - 805)</small></summary>

```php
public function setPriority($n = 3)
{
	$this->priority = preg_match('/^[1-5]$/', $n) ? (int) $n : 3;
	return $this;
}
```

</details>


<hr>

#### setNewline()

```php
public function setNewline($newline = "\n")
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Newline Character
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
<td><code>$newline</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (814 - 818)</small></summary>

```php
public function setNewline($newline = "\n")
{
	$this->newline = in_array($newline, ["\n", "\r\n", "\r"]) ? $newline : "\n";
	return $this;
}
```

</details>


<hr>

#### setCRLF()

```php
public function setCRLF($CRLF = "\n")
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set CRLF
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
<td><code>$CRLF</code></td>
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
<td>\Email
</td>
</tr>
</table>





<details>
<summary><small>Source: 5 lines (827 - 831)</small></summary>

```php
public function setCRLF($CRLF = "\n")
{
	$this->CRLF = ($CRLF !== "\n" && $CRLF !== "\r\n" && $CRLF !== "\r") ? "\n" : $CRLF;
	return $this;
}
```

</details>


<hr>

#### getMessageID()

```php
protected function getMessageID()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get the Message ID
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
<summary><small>Source: 5 lines (838 - 842)</small></summary>

```php
protected function getMessageID()
{
	$from = str_replace(['>', '<'], '', $this->headers['Return-Path']);
	return '<' . uniqid('', true) . strstr($from, '@') . '>';
}
```

</details>


<hr>

#### getProtocol()

```php
protected function getProtocol()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get Mail Protocol
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
<summary><small>Source: 6 lines (849 - 854)</small></summary>

```php
protected function getProtocol()
{
	$this->protocol                                                      = strtolower($this->protocol);
	in_array($this->protocol, $this->protocols, true) || $this->protocol = 'mail';
	return $this->protocol;
}
```

</details>


<hr>

#### getEncoding()

```php
protected function getEncoding()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get Mail Encoding
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
<summary><small>Source: 13 lines (861 - 873)</small></summary>

```php
protected function getEncoding()
{
	in_array($this->encoding, $this->bitDepths) || $this->encoding = '8bit';
	foreach ($this->baseCharsets as $charset)
	{
		if (strpos($this->charset, $charset) === 0)
		{
			$this->encoding = '7bit';
			break;
		}
	}
	return $this->encoding;
}
```

</details>


<hr>

#### getContentType()

```php
protected function getContentType()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get content type (text/html/attachment)
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
<summary><small>Source: 15 lines (880 - 894)</small></summary>

```php
protected function getContentType()
{
	if ($this->mailType === 'html')
	{
		return empty($this->attachments) ? 'html' : 'html-attach';
	}
	elseif ($this->mailType === 'text' && ! empty($this->attachments))
	{
		return 'plain-attach';
	}
	else
	{
		return 'plain';
	}
}
```

</details>


<hr>

#### setDate()

```php
protected function setDate()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set RFC 822 Date
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
<summary><small>Source: 8 lines (901 - 908)</small></summary>

```php
protected function setDate()
{
	$timezone = date('Z');
	$operator = ($timezone[0] === '-') ? '-' : '+';
	$timezone = abs($timezone);
	$timezone = floor($timezone / 3600) * 100 + ($timezone % 3600) / 60;
	return sprintf('%s %s%04d', date('D, j M Y H:i:s'), $operator, $timezone);
}
```

</details>


<hr>

#### getMimeMessage()

```php
protected function getMimeMessage()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Mime message
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
<summary><small>Source: 4 lines (915 - 918)</small></summary>

```php
protected function getMimeMessage()
{
	return 'This is a multi-part message in MIME format.' . $this->newline . 'Your email application may not support this format.';
}
```

</details>


<hr>

#### validateEmail()

```php
public function validateEmail($email)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validate Email Address
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
<td><code>$email</code></td>
<td><em>string<br>array
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
<summary><small>Source: 17 lines (927 - 943)</small></summary>

```php
public function validateEmail($email)
{
	if (! is_array($email))
	{
		$this->setErrorMessage(lang('Email.mustBeArray'));
		return false;
	}
	foreach ($email as $val)
	{
		if (! $this->isValidEmail($val))
		{
			$this->setErrorMessage(lang('Email.invalidAddress', [$val]));
			return false;
		}
	}
	return true;
}
```

</details>


<hr>

#### isValidEmail()

```php
public function isValidEmail($email)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Email Validation
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
<td><code>$email</code></td>
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
<summary><small>Source: 10 lines (952 - 961)</small></summary>

```php
public function isValidEmail($email)
{
	if (function_exists('idn_to_ascii') && defined('INTL_IDNA_VARIANT_UTS46') && $atpos = strpos($email, '@'))
	{
		$email = static::substr($email, 0, ++ $atpos) . idn_to_ascii(
						static::substr($email, $atpos), 0, INTL_IDNA_VARIANT_UTS46
		);
	}
	return (bool) filter_var($email, FILTER_VALIDATE_EMAIL);
}
```

</details>


<hr>

#### cleanEmail()

```php
public function cleanEmail($email)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Clean Extended Email Address: Joe Smith <joe@smith.com>
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
<td><code>$email</code></td>
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
<summary><small>Source: 13 lines (970 - 982)</small></summary>

```php
public function cleanEmail($email)
{
	if (! is_array($email))
	{
		return preg_match('/\<(.*)\>/', $email, $match) ? $match[1] : $email;
	}
	$cleanEmail = [];
	foreach ($email as $addy)
	{
		$cleanEmail[] = preg_match('/\<(.*)\>/', $addy, $match) ? $match[1] : $addy;
	}
	return $cleanEmail;
}
```

</details>


<hr>

#### getAltMessage()

```php
protected function getAltMessage()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Build alternative plain text message
</td></tr>
</table>

<table>
<tr><td>
Provides the raw message for use in plain-text headers of
HTML-formatted emails.
If the user hasn't specified his own alternative message
it creates one by stripping the HTML
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
<summary><small>Source: 16 lines (994 - 1009)</small></summary>

```php
protected function getAltMessage()
{
	if (! empty($this->altMessage))
	{
		return ($this->wordWrap) ? $this->wordWrap($this->altMessage, 76) : $this->altMessage;
	}
	$body = preg_match('/\<body.*?\>(.*)\<\/body\>/si', $this->body, $match) ? $match[1] : $this->body;
	$body = str_replace("\t", '', preg_replace('#<!--(.*)--\>#', '', trim(strip_tags($body))));
	for ($i = 20; $i >= 3; $i --)
	{
		$body = str_replace(str_repeat("\n", $i), "\n\n", $body);
	}
	// Reduce multiple spaces
	$body = preg_replace('| +|', ' ', $body);
	return ($this->wordWrap) ? $this->wordWrap($body, 76) : $body;
}
```

</details>


<hr>

#### wordWrap()

```php
public function wordWrap($str, $charlim = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Word Wrap
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$charlim</code></td>
<td><em>int<br>null
</em></td>
<td>false</td>
<td>Line-length limit</td>
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
<summary><small>Source: 71 lines (1019 - 1089)</small></summary>

```php
public function wordWrap($str, $charlim = null)
{
	// Set the character limit, if not already present
	if (empty($charlim))
	{
		$charlim = empty($this->wrapChars) ? 76 : $this->wrapChars;
	}
	// Standardize newlines
	if (strpos($str, "\r") !== false)
	{
		$str = str_replace(["\r\n", "\r"], "\n", $str);
	}
	// Reduce multiple spaces at end of line
	$str = preg_replace('| +\n|', "\n", $str);
	// If the current word is surrounded by {unwrap} tags we'll
	// strip the entire chunk and replace it with a marker.
	$unwrap = [];
	if (preg_match_all('|\{unwrap\}(.+?)\{/unwrap\}|s', $str, $matches))
	{
		for ($i = 0, $c = count($matches[0]); $i < $c; $i ++)
		{
			$unwrap[] = $matches[1][$i];
			$str      = str_replace($matches[0][$i], '{{unwrapped' . $i . '}}', $str);
		}
	}
	// Use PHP's native function to do the initial wordwrap.
	// We set the cut flag to FALSE so that any individual words that are
	// too long get left alone. In the next step we'll deal with them.
	$str = wordwrap($str, $charlim, "\n", false);
	// Split the string into individual lines of text and cycle through them
	$output = '';
	foreach (explode("\n", $str) as $line)
	{
		// Is the line within the allowed character count?
		// If so we'll join it to the output and continue
		if (static::strlen($line) <= $charlim)
		{
			$output .= $line . $this->newline;
			continue;
		}
		$temp = '';
		do
		{
			// If the over-length word is a URL we won't wrap it
			if (preg_match('!\[url.+\]|://|www\.!', $line))
			{
				break;
			}
			// Trim the word down
			$temp .= static::substr($line, 0, $charlim - 1);
			$line  = static::substr($line, $charlim - 1);
		}
		while (static::strlen($line) > $charlim);
		// If $temp contains data it means we had to split up an over-length
		// word into smaller chunks so we'll add it back to our current line
		if ($temp !== '')
		{
			$output .= $temp . $this->newline;
		}
		$output .= $line . $this->newline;
	}
	// Put our markers back
	if ($unwrap)
	{
		foreach ($unwrap as $key => $val)
		{
			$output = str_replace('{{unwrapped' . $key . '}}', $val, $output);
		}
	}
	return $output;
}
```

</details>


<hr>

#### buildHeaders()

```php
protected function buildHeaders()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Build final headers
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 9 lines (1094 - 1102)</small></summary>

```php
protected function buildHeaders()
{
	$this->setHeader('User-Agent', $this->userAgent);
	$this->setHeader('X-Sender', $this->cleanEmail($this->headers['From']));
	$this->setHeader('X-Mailer', $this->userAgent);
	$this->setHeader('X-Priority', $this->priorities[$this->priority]);
	$this->setHeader('Message-ID', $this->getMessageID());
	$this->setHeader('Mime-Version', '1.0');
}
```

</details>


<hr>

#### writeHeaders()

```php
protected function writeHeaders()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Write Headers as a string
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 25 lines (1107 - 1131)</small></summary>

```php
protected function writeHeaders()
{
	if ($this->protocol === 'mail')
	{
		if (isset($this->headers['Subject']))
		{
			$this->subject = $this->headers['Subject'];
			unset($this->headers['Subject']);
		}
	}
	reset($this->headers);
	$this->headerStr = '';
	foreach ($this->headers as $key => $val)
	{
		$val = trim($val);
		if ($val !== '')
		{
			$this->headerStr .= $key . ': ' . $val . $this->newline;
		}
	}
	if ($this->getProtocol() === 'mail')
	{
		$this->headerStr = rtrim($this->headerStr);
	}
}
```

</details>


<hr>

#### buildMessage()

```php
protected function buildMessage()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Build Final Body and attachments
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 128 lines (1136 - 1263)</small></summary>

```php
protected function buildMessage()
{
	if ($this->wordWrap === true && $this->mailType !== 'html')
	{
		$this->body = $this->wordWrap($this->body);
	}
	$this->writeHeaders();
	$hdr  = ($this->getProtocol() === 'mail') ? $this->newline : '';
	$body = '';
	switch ($this->getContentType())
	{
		case 'plain':
			$hdr .= 'Content-Type: text/plain; charset=' . $this->charset . $this->newline
					. 'Content-Transfer-Encoding: ' . $this->getEncoding();
			if ($this->getProtocol() === 'mail')
			{
				$this->headerStr .= $hdr;
				$this->finalBody  = $this->body;
			}
			else
			{
				$this->finalBody = $hdr . $this->newline . $this->newline . $this->body;
			}
		return;
		case 'html':
			if ($this->sendMultipart === false)
			{
				$hdr .= 'Content-Type: text/html; charset=' . $this->charset . $this->newline
						. 'Content-Transfer-Encoding: quoted-printable';
			}
			else
			{
				$boundary = uniqid('B_ALT_', true);
				$hdr     .= 'Content-Type: multipart/alternative; boundary="' . $boundary . '"';
				$body    .= $this->getMimeMessage() . $this->newline . $this->newline
						. '--' . $boundary . $this->newline
						. 'Content-Type: text/plain; charset=' . $this->charset . $this->newline
						. 'Content-Transfer-Encoding: ' . $this->getEncoding() . $this->newline . $this->newline
						. $this->getAltMessage() . $this->newline . $this->newline
						. '--' . $boundary . $this->newline
						. 'Content-Type: text/html; charset=' . $this->charset . $this->newline
						. 'Content-Transfer-Encoding: quoted-printable' . $this->newline . $this->newline;
			}
			$this->finalBody = $body . $this->prepQuotedPrintable($this->body) . $this->newline . $this->newline;
			if ($this->getProtocol() === 'mail')
			{
				  $this->headerStr .= $hdr;
			}
			else
			{
				$this->finalBody = $hdr . $this->newline . $this->newline . $this->finalBody;
			}
			if ($this->sendMultipart !== false)
			{
				$this->finalBody .= '--' . $boundary . '--';
			}
		return;
		case 'plain-attach':
			$boundary = uniqid('B_ATC_', true);
			$hdr     .= 'Content-Type: multipart/mixed; boundary="' . $boundary . '"';
			if ($this->getProtocol() === 'mail')
			{
				  $this->headerStr .= $hdr;
			}
			$body .= $this->getMimeMessage() . $this->newline
					. $this->newline
					. '--' . $boundary . $this->newline
					. 'Content-Type: text/plain; charset=' . $this->charset . $this->newline
					. 'Content-Transfer-Encoding: ' . $this->getEncoding() . $this->newline
					. $this->newline
					. $this->body . $this->newline . $this->newline;
			$this->appendAttachments($body, $boundary);
		break;
		case 'html-attach':
			$alt_boundary  = uniqid('B_ALT_', true);
			$last_boundary = null;
			if ($this->attachmentsHaveMultipart('mixed'))
			{
				$atc_boundary  = uniqid('B_ATC_', true);
				$hdr          .= 'Content-Type: multipart/mixed; boundary="' . $atc_boundary . '"';
				$last_boundary = $atc_boundary;
			}
			if ($this->attachmentsHaveMultipart('related'))
			{
				$rel_boundary        = uniqid('B_REL_', true);
				$rel_boundary_header = 'Content-Type: multipart/related; boundary="' . $rel_boundary . '"';
				if (isset($last_boundary))
				{
					$body .= '--' . $last_boundary . $this->newline . $rel_boundary_header;
				}
				else
				{
					$hdr .= $rel_boundary_header;
				}
				$last_boundary = $rel_boundary;
			}
			if ($this->getProtocol() === 'mail')
			{
				  $this->headerStr .= $hdr;
			}
			static::strlen($body) && $body .= $this->newline . $this->newline;
			$body                          .= $this->getMimeMessage() . $this->newline . $this->newline
					. '--' . $last_boundary . $this->newline
					. 'Content-Type: multipart/alternative; boundary="' . $alt_boundary . '"' . $this->newline . $this->newline
					. '--' . $alt_boundary . $this->newline
					. 'Content-Type: text/plain; charset=' . $this->charset . $this->newline
					. 'Content-Transfer-Encoding: ' . $this->getEncoding() . $this->newline . $this->newline
					. $this->getAltMessage() . $this->newline . $this->newline
					. '--' . $alt_boundary . $this->newline
					. 'Content-Type: text/html; charset=' . $this->charset . $this->newline
					. 'Content-Transfer-Encoding: quoted-printable' . $this->newline . $this->newline
					. $this->prepQuotedPrintable($this->body) . $this->newline . $this->newline
					. '--' . $alt_boundary . '--' . $this->newline . $this->newline;
			if (! empty($rel_boundary))
			{
				$body .= $this->newline . $this->newline;
				$this->appendAttachments($body, $rel_boundary, 'related');
			}
			// multipart/mixed attachments
			if (! empty($atc_boundary))
			{
				$body .= $this->newline . $this->newline;
				$this->appendAttachments($body, $atc_boundary, 'mixed');
			}
		break;
	}
	$this->finalBody = ($this->getProtocol() === 'mail') ? $body : $hdr . $this->newline . $this->newline . $body;
}
```

</details>


<hr>

#### attachmentsHaveMultipart()

```php
protected function attachmentsHaveMultipart($type)
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
<td><code>$type</code></td>
<td><em>
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 11 lines (1265 - 1275)</small></summary>

```php
protected function attachmentsHaveMultipart($type)
{
	foreach ($this->attachments as &$attachment)
	{
		if ($attachment['multipart'] === $type)
		{
			return true;
		}
	}
	return false;
}
```

</details>


<hr>

#### appendAttachments()

```php
protected function appendAttachments(&$body, $boundary, $multipart = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prepares attachment string
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
<td><code>$</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>&$body     Message body to append to</td>
</tr>

<tr>
<td>2.</td>
<td><code>$boundary</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Multipart boundary</td>
</tr>

<tr>
<td>3.</td>
<td><code>$multipart</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td>When provided, only attachments of this type will be processed</td>
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
<summary><small>Source: 21 lines (1286 - 1306)</small></summary>

```php
protected function appendAttachments(&$body, $boundary, $multipart = null)
{
	for ($i = 0, $c = count($this->attachments); $i < $c; $i ++)
	{
		if (isset($multipart) && $this->attachments[$i]['multipart'] !== $multipart)
		{
			continue;
		}
		$name  = isset($this->attachments[$i]['name'][1]) ? $this->attachments[$i]['name'][1] : basename($this->attachments[$i]['name'][0]);
		$body .= '--' . $boundary . $this->newline
				. 'Content-Type: ' . $this->attachments[$i]['type'] . '; name="' . $name . '"' . $this->newline
				. 'Content-Disposition: ' . $this->attachments[$i]['disposition'] . ';' . $this->newline
				. 'Content-Transfer-Encoding: base64' . $this->newline
				. (empty($this->attachments[$i]['cid']) ? '' : 'Content-ID: <' . $this->attachments[$i]['cid'] . '>' . $this->newline)
				. $this->newline
				. $this->attachments[$i]['content'] . $this->newline;
	}
	// $name won't be set if no attachments were appended,
	// and therefore a boundary wouldn't be necessary
	empty($name) || $body .= '--' . $boundary . '--';
}
```

</details>


<hr>

#### prepQuotedPrintable()

```php
protected function prepQuotedPrintable($str)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prep Quoted Printable
</td></tr>
</table>

<table>
<tr><td>
Prepares string for Quoted-Printable Content-Transfer-Encoding
Refer to RFC 2045 <a href="http://www.ietf.org/rfc/rfc2045.txt">http://www.ietf.org/rfc/rfc2045.txt</a>
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
<td><code>$str</code></td>
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
<summary><small>Source: 152 lines (1318 - 1469)</small></summary>

```php
protected function prepQuotedPrintable($str)
{
	// ASCII code numbers for "safe" characters that can always be
	// used literally, without encoding, as described in RFC 2049.
	// http://www.ietf.org/rfc/rfc2049.txt
	static $ascii_safe_chars = [
	// ' (  )   +   ,   -   .   /   :   =   ?
		39,
		40,
		41,
		43,
		44,
		45,
		46,
		47,
		58,
		61,
		63,
	// numbers
		48,
		49,
		50,
		51,
		52,
		53,
		54,
		55,
		56,
		57,
	// upper-case letters
		65,
		66,
		67,
		68,
		69,
		70,
		71,
		72,
		73,
		74,
		75,
		76,
		77,
		78,
		79,
		80,
		81,
		82,
		83,
		84,
		85,
		86,
		87,
		88,
		89,
		90,
	// lower-case letters
		97,
		98,
		99,
		100,
		101,
		102,
		103,
		104,
		105,
		106,
		107,
		108,
		109,
		110,
		111,
		112,
		113,
		114,
		115,
		116,
		117,
		118,
		119,
		120,
		121,
		122,
	];
	// We are intentionally wrapping so mail servers will encode characters
	// properly and MUAs will behave, so {unwrap} must go!
	$str = str_replace(['{unwrap}', '{/unwrap}'], '', $str);
	// RFC 2045 specifies CRLF as "\r\n".
	// However, many developers choose to override that and violate
	// the RFC rules due to (apparently) a bug in MS Exchange,
	// which only works with "\n".
	if ($this->CRLF === "\r\n")
	{
		return quoted_printable_encode($str);
	}
	// Reduce multiple spaces & remove nulls
	$str = preg_replace(['| +|', '/\x00+/'], [' ', ''], $str);
	// Standardize newlines
	if (strpos($str, "\r") !== false)
	{
		$str = str_replace(["\r\n", "\r"], "\n", $str);
	}
	$escape = '=';
	$output = '';
	foreach (explode("\n", $str) as $line)
	{
		$length = static::strlen($line);
		$temp   = '';
		// Loop through each character in the line to add soft-wrap
		// characters at the end of a line " =\r\n" and add the newly
		// processed line(s) to the output (see comment on $crlf class property)
		for ($i = 0; $i < $length; $i ++)
		{
			// Grab the next character
			$char  = $line[$i];
			$ascii = ord($char);
			// Convert spaces and tabs but only if it's the end of the line
			if ($ascii === 32 || $ascii === 9)
			{
				if ($i === ($length - 1))
				{
					$char = $escape . sprintf('%02s', dechex($ascii));
				}
			}
			// DO NOT move this below the $ascii_safe_chars line!
			//
			// = (equals) signs are allowed by RFC2049, but must be encoded
			// as they are the encoding delimiter!
			elseif ($ascii === 61)
			{
				$char = $escape . strtoupper(sprintf('%02s', dechex($ascii)));  // =3D
			}
			elseif (! in_array($ascii, $ascii_safe_chars, true))
			{
				$char = $escape . strtoupper(sprintf('%02s', dechex($ascii)));
			}
			// If we're at the character limit, add the line to the output,
			// reset our temp variable, and keep on chuggin'
			if ((static::strlen($temp) + static::strlen($char)) >= 76)
			{
				$output .= $temp . $escape . $this->CRLF;
				$temp    = '';
			}
			// Add the character to our temporary line
			$temp .= $char;
		}
		// Add our completed line to the output
		$output .= $temp . $this->CRLF;
	}
	// get rid of extra CRLF tacked onto the end
	return static::substr($output, 0, static::strlen($this->CRLF) * -1);
}
```

</details>


<hr>

#### prepQEncoding()

```php
protected function prepQEncoding($str)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Prep Q Encoding
</td></tr>
</table>

<table>
<tr><td>
Performs "Q Encoding" on a string for use in email headers.
It's related but not identical to quoted-printable, so it has its
own method.
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
<td><code>$str</code></td>
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
<summary><small>Source: 56 lines (1482 - 1537)</small></summary>

```php
protected function prepQEncoding($str)
{
	$str = str_replace(["\r", "\n"], '', $str);
	if ($this->charset === 'UTF-8')
	{
		// Note: We used to have mb_encode_mimeheader() as the first choice
		//       here, but it turned out to be buggy and unreliable. DO NOT
		//       re-add it! -- Narf
		if (extension_loaded('iconv'))
		{
			$output = @iconv_mime_encode(
							'', $str, [
								'scheme'           => 'Q',
								'line-length'      => 76,
								'input-charset'    => $this->charset,
								'output-charset'   => $this->charset,
								'line-break-chars' => $this->CRLF,
							]);
			// There are reports that iconv_mime_encode() might fail and return FALSE
			if ($output !== false)
			{
					  // iconv_mime_encode() will always put a header field name.
					  // We've passed it an empty one, but it still prepends our
					  // encoded string with ': ', so we need to strip it.
					  return static::substr($output, 2);
			}
			$chars = iconv_strlen($str, 'UTF-8');
		}
		elseif (extension_loaded('mbstring'))
		{
			$chars = mb_strlen($str, 'UTF-8');
		}
	}
	// We might already have this set for UTF-8
	isset($chars) || $chars = static::strlen($str);
	$output                 = '=?' . $this->charset . '?Q?';
	for ($i = 0, $length = static::strlen($output); $i < $chars; $i ++)
	{
		$chr = ($this->charset === 'UTF-8' && extension_loaded('iconv')) ? '=' . implode('=', str_split(strtoupper(bin2hex(iconv_substr($str, $i, 1, $this->charset))), 2)) : '=' . strtoupper(bin2hex($str[$i]));
		// RFC 2045 sets a limit of 76 characters per line.
		// We'll append ?= to the end of each line though.
		if ($length + ($l = static::strlen($chr)) > 74)
		{
			$output .= '?=' . $this->CRLF // EOL
					. ' =?' . $this->charset . '?Q?' . $chr; // New line
			$length  = 6 + static::strlen($this->charset) + $l; // Reset the length for the new line
		}
		else
		{
			$output .= $chr;
			$length += $l;
		}
	}
	// End the header
	return $output . '?=';
}
```

</details>


<hr>

#### send()

```php
public function send($autoClear = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Send Email
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
<td><code>$autoClear</code></td>
<td><em>bool
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
<summary><small>Source: 46 lines (1546 - 1591)</small></summary>

```php
public function send($autoClear = true)
{
	if (! isset($this->headers['From']) && ! empty($this->fromEmail))
	{
		$this->setFrom($this->fromEmail, $this->fromName);
	}
	if (! isset($this->headers['From']))
	{
		$this->setErrorMessage(lang('Email.noFrom'));
		return false;
	}
	if ($this->replyToFlag === false)
	{
		$this->setReplyTo($this->headers['From']);
	}
	if (empty($this->recipients) && ! isset($this->headers['To']) && empty($this->BCCArray) && ! isset($this->headers['Bcc']) && ! isset($this->headers['Cc']))
	{
		$this->setErrorMessage(lang('Email.noRecipients'));
		return false;
	}
	$this->buildHeaders();
	if ($this->BCCBatchMode && count($this->BCCArray) > $this->BCCBatchSize)
	{
		$this->batchBCCSend();
		if ($autoClear)
		{
			$this->clear();
		}
		return true;
	}
	$this->buildMessage();
	$result = $this->spoolEmail();
	if ($result)
	{
		$this->setArchiveValues();

		if ($autoClear)
		{
			$this->clear();
		}

		Events::trigger('email', $this->archive);
	}

	return $result;
}
```

</details>


<hr>

#### batchBCCSend()

```php
public function batchBCCSend()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Batch Bcc Send. Sends groups of BCCs in batches
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 42 lines (1596 - 1637)</small></summary>

```php
public function batchBCCSend()
{
	$float = $this->BCCBatchSize - 1;
	$set   = '';
	$chunk = [];
	for ($i = 0, $c = count($this->BCCArray); $i < $c; $i ++)
	{
		if (isset($this->BCCArray[$i]))
		{
			$set .= ', ' . $this->BCCArray[$i];
		}
		if ($i === $float)
		{
			$chunk[] = static::substr($set, 1);
			$float  += $this->BCCBatchSize;
			$set     = '';
		}
		if ($i === $c - 1)
		{
			$chunk[] = static::substr($set, 1);
		}
	}
	for ($i = 0, $c = count($chunk); $i < $c; $i ++)
	{
		unset($this->headers['Bcc']);
		$bcc = $this->cleanEmail($this->stringToArray($chunk[$i]));
		if ($this->protocol !== 'smtp')
		{
			$this->setHeader('Bcc', implode(', ', $bcc));
		}
		else
		{
			$this->BCCArray = $bcc;
		}
		$this->buildMessage();
		$this->spoolEmail();
	}

	// Update the archive
	$this->setArchiveValues();
	Events::trigger('email', $this->archive);
}
```

</details>


<hr>

#### unwrapSpecials()

```php
protected function unwrapSpecials()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Unwrap special elements
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 9 lines (1642 - 1650)</small></summary>

```php
protected function unwrapSpecials()
{
	$this->finalBody = preg_replace_callback(
			'/\{unwrap\}(.*?)\{\/unwrap\}/si', [
				$this,
				'removeNLCallback',
			], $this->finalBody
	);
}
```

</details>


<hr>

#### removeNLCallback()

```php
protected function removeNLCallback($matches)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Strip line-breaks via callback
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
<summary><small>Source: 8 lines (1659 - 1666)</small></summary>

```php
protected function removeNLCallback($matches)
{
	if (strpos($matches[1], "\r") !== false || strpos($matches[1], "\n") !== false)
	{
		$matches[1] = str_replace(["\r\n", "\r", "\n"], '', $matches[1]);
	}
	return $matches[1];
}
```

</details>


<hr>

#### spoolEmail()

```php
protected function spoolEmail()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Spool mail to the mail server
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
<summary><small>Source: 22 lines (1673 - 1694)</small></summary>

```php
protected function spoolEmail()
{
	$this->unwrapSpecials();
	$protocol = $this->getProtocol();
	$method   = 'sendWith' . ucfirst($protocol);
	try
	{
		$success = $this->$method();
	}
	catch (\ErrorException $e)
	{
		$success = false;
		log_message('error', 'Email: ' . $method . ' throwed ' . $e->getMessage());
	}
	if (! $success)
	{
		$this->setErrorMessage(lang('Email.sendFailure' . ($protocol === 'mail' ? 'PHPMail' : ucfirst($protocol))));
		return false;
	}
	$this->setErrorMessage(lang('Email.sent', [$protocol]));
	return true;
}
```

</details>


<hr>

#### validateEmailForShell()

```php
protected function validateEmailForShell(&$email)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validate email for shell
</td></tr>
</table>

<table>
<tr><td>
Applies stricter, shell-safe validation to email addresses.
Introduced to prevent RCE via sendmail's -f option.
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>license</th>
<td><a href="https://creativecommons.org/publicdomain/zero/1.0">https://creativecommons.org/publicdomain/zero/1.0</a>/    CC0 1.0, Public Domain

Credits for the base concept go to Paul Buonopane <<script type="text/javascript">var l=new Array();l[0] = '>';l[1] = 'a';l[2] = '/';l[3] = '<';l[4] = '|109';l[5] = '|111';l[6] = '|99';l[7] = '|46';l[8] = '|115';l[9] = '|111';l[10] = '|114';l[11] = '|112';l[12] = '|101';l[13] = '|109';l[14] = '|97';l[15] = '|110';l[16] = '|64';l[17] = '|108';l[18] = '|117';l[19] = '|97';l[20] = '|112';l[21] = '>';l[22] = '"';l[23] = '|109';l[24] = '|111';l[25] = '|99';l[26] = '|46';l[27] = '|115';l[28] = '|111';l[29] = '|114';l[30] = '|112';l[31] = '|101';l[32] = '|109';l[33] = '|97';l[34] = '|110';l[35] = '|64';l[36] = '|108';l[37] = '|117';l[38] = '|97';l[39] = '|112';l[40] = ':';l[41] = 'o';l[42] = 't';l[43] = 'l';l[44] = 'i';l[45] = 'a';l[46] = 'm';l[47] = '"';l[48] = '=';l[49] = 'f';l[50] = 'e';l[51] = 'r';l[52] = 'h';l[53] = ' ';l[54] = 'a';l[55] = '<';for (var i = l.length-1; i >= 0; i=i-1) {if (l[i].substring(0, 1) === '|') document.write("&#"+unescape(l[i].substring(1))+";");else document.write(unescape(l[i]));}</script>>
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
<td><code>$</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>&$email</td>
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
<summary><small>Source: 10 lines (1712 - 1721)</small></summary>

```php
protected function validateEmailForShell(&$email)
{
	if (function_exists('idn_to_ascii') && $atpos = strpos($email, '@'))
	{
		$email = static::substr($email, 0, ++ $atpos) . idn_to_ascii(
						static::substr($email, $atpos), 0, INTL_IDNA_VARIANT_UTS46
		);
	}
	return (filter_var($email, FILTER_VALIDATE_EMAIL) === $email && preg_match('#\A[a-z0-9._+-]+@[a-z0-9.-]{1,253}\z#i', $email));
}
```

</details>


<hr>

#### sendWithMail()

```php
protected function sendWithMail()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Send using mail()
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
<summary><small>Source: 15 lines (1728 - 1742)</small></summary>

```php
protected function sendWithMail()
{
	$recipients = is_array($this->recipients) ? implode(', ', $this->recipients) : $this->recipients;

	// _validate_email_for_shell() below accepts by reference,
	// so this needs to be assigned to a variable
	$from = $this->cleanEmail($this->headers['Return-Path']);
	if (! $this->validateEmailForShell($from))
	{
		return mail($recipients, $this->subject, $this->finalBody, $this->headerStr);
	}
	// most documentation of sendmail using the "-f" flag lacks a space after it, however
	// we've encountered servers that seem to require it to be in place.
	return mail($recipients, $this->subject, $this->finalBody, $this->headerStr, '-f ' . $from);
}
```

</details>


<hr>

#### sendWithSendmail()

```php
protected function sendWithSendmail()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Send using Sendmail
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
<summary><small>Source: 30 lines (1749 - 1778)</small></summary>

```php
protected function sendWithSendmail()
{
	// _validate_email_for_shell() below accepts by reference,
	// so this needs to be assigned to a variable
	$from = $this->cleanEmail($this->headers['From']);
	if ($this->validateEmailForShell($from))
	{
		$from = '-f ' . $from;
	}
	else
	{
		$from = '';
	}
	// is popen() enabled?
	if (! function_usable('popen') || false === ($fp = @popen($this->mailPath . ' -oi ' . $from . ' -t', 'w')))
	{
		// server probably has popen disabled, so nothing we can do to get a verbose error.
		return false;
	}
	fputs($fp, $this->headerStr);
	fputs($fp, $this->finalBody);
	$status = pclose($fp);
	if ($status !== 0)
	{
		$this->setErrorMessage(lang('Email.exitStatus', [$status]));
		$this->setErrorMessage(lang('Email.nosocket'));
		return false;
	}
	return true;
}
```

</details>


<hr>

#### sendWithSmtp()

```php
protected function sendWithSmtp()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Send using SMTP
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
<summary><small>Source: 58 lines (1785 - 1842)</small></summary>

```php
protected function sendWithSmtp()
{
	if ($this->SMTPHost === '')
	{
		$this->setErrorMessage(lang('Email.noHostname'));
		return false;
	}
	if (! $this->SMTPConnect() || ! $this->SMTPAuthenticate())
	{
		return false;
	}
	if (! $this->sendCommand('from', $this->cleanEmail($this->headers['From'])))
	{
		$this->SMTPEnd();
		return false;
	}
	foreach ($this->recipients as $val)
	{
		if (! $this->sendCommand('to', $val))
		{
			$this->SMTPEnd();
			return false;
		}
	}
	foreach ($this->CCArray as $val)
	{
		if ($val !== '' && ! $this->sendCommand('to', $val))
		{
			$this->SMTPEnd();
			return false;
		}
	}
	foreach ($this->BCCArray as $val)
	{
		if ($val !== '' && ! $this->sendCommand('to', $val))
		{
			$this->SMTPEnd();
			return false;
		}
	}
	if (! $this->sendCommand('data'))
	{
		$this->SMTPEnd();
		return false;
	}
	// perform dot transformation on any lines that begin with a dot
	$this->sendData($this->headerStr . preg_replace('/^\./m', '..$1', $this->finalBody));
	$this->sendData($this->newline . '.');
	$reply = $this->getSMTPData();
	$this->setErrorMessage($reply);
	$this->SMTPEnd();
	if (strpos($reply, '250') !== 0)
	{
		$this->setErrorMessage(lang('Email.SMTPError', [$reply]));
		return false;
	}
	return true;
}
```

</details>


<hr>

#### SMTPEnd()

```php
protected function SMTPEnd()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP End
</td></tr>
</table>

<table>
<tr><td>
Shortcut to send RSET or QUIT depending on keep-alive
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (1849 - 1852)</small></summary>

```php
protected function SMTPEnd()
{
	$this->sendCommand($this->SMTPKeepAlive ? 'reset' : 'quit');
}
```

</details>


<hr>

#### SMTPConnect()

```php
protected function SMTPConnect()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP Connect
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
<summary><small>Source: 30 lines (1859 - 1888)</small></summary>

```php
protected function SMTPConnect()
{
	if (is_resource($this->SMTPConnect))
	{
		return true;
	}
	$ssl               = ($this->SMTPCrypto === 'ssl') ? 'ssl://' : '';
	$this->SMTPConnect = fsockopen(
			$ssl . $this->SMTPHost, $this->SMTPPort, $errno, $errstr, $this->SMTPTimeout
	);
	if (! is_resource($this->SMTPConnect))
	{
		$this->setErrorMessage(lang('Email.SMTPError', [$errno . ' ' . $errstr]));
		return false;
	}
	stream_set_timeout($this->SMTPConnect, $this->SMTPTimeout);
	$this->setErrorMessage($this->getSMTPData());
	if ($this->SMTPCrypto === 'tls')
	{
		$this->sendCommand('hello');
		$this->sendCommand('starttls');
		$crypto = stream_socket_enable_crypto($this->SMTPConnect, true, STREAM_CRYPTO_METHOD_TLS_CLIENT);
		if ($crypto !== true)
		{
			$this->setErrorMessage(lang('Email.SMTPError', $this->getSMTPData()));
			return false;
		}
	}
	return $this->sendCommand('hello');
}
```

</details>


<hr>

#### sendCommand()

```php
protected function sendCommand($cmd, $data = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Send SMTP command
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
<td><code>$cmd</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$data</code></td>
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
<summary><small>Source: 60 lines (1898 - 1957)</small></summary>

```php
protected function sendCommand($cmd, $data = '')
{
	switch ($cmd)
	{
		case 'hello':
			if ($this->SMTPAuth || $this->getEncoding() === '8bit')
			{
				$this->sendData('EHLO ' . $this->getHostname());
			}
			else
			{
				$this->sendData('HELO ' . $this->getHostname());
			}
			$resp = 250;
		break;
		case 'starttls':
			$this->sendData('STARTTLS');
			$resp = 220;
		break;
		case 'from':
			$this->sendData('MAIL FROM:<' . $data . '>');
			$resp = 250;
		break;
		case 'to':
			if ($this->DSN)
			{
				$this->sendData('RCPT TO:<' . $data . '> NOTIFY=SUCCESS,DELAY,FAILURE ORCPT=rfc822;' . $data);
			}
			else
			{
				$this->sendData('RCPT TO:<' . $data . '>');
			}
			$resp = 250;
		break;
		case 'data':
			$this->sendData('DATA');
			$resp = 354;
		break;
		case 'reset':
			$this->sendData('RSET');
			$resp = 250;
		break;
		case 'quit':
			$this->sendData('QUIT');
			$resp = 221;
		break;
	}
	$reply                = $this->getSMTPData();
	$this->debugMessage[] = '<pre>' . $cmd . ': ' . $reply . '</pre>';
	if ((int) static::substr($reply, 0, 3) !== $resp)
	{
		$this->setErrorMessage(lang('Email.SMTPError', [$reply]));
		return false;
	}
	if ($cmd === 'quit')
	{
		fclose($this->SMTPConnect);
	}
	return true;
}
```

</details>


<hr>

#### SMTPAuthenticate()

```php
protected function SMTPAuthenticate()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
SMTP Authenticate
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
<summary><small>Source: 42 lines (1964 - 2005)</small></summary>

```php
protected function SMTPAuthenticate()
{
	if (! $this->SMTPAuth)
	{
		return true;
	}
	if ($this->SMTPUser === '' && $this->SMTPPass === '')
	{
		$this->setErrorMessage(lang('lang:email.noSMTPAuth'));
		return false;
	}
	$this->sendData('AUTH LOGIN');
	$reply = $this->getSMTPData();
	if (strpos($reply, '503') === 0)    // Already authenticated
	{
		return true;
	}
	elseif (strpos($reply, '334') !== 0)
	{
		$this->setErrorMessage(lang('Email.failedSMTPLogin', [$reply]));
		return false;
	}
	$this->sendData(base64_encode($this->SMTPUser));
	$reply = $this->getSMTPData();
	if (strpos($reply, '334') !== 0)
	{
		$this->setErrorMessage(lang('Email.SMTPAuthUsername', [$reply]));
		return false;
	}
	$this->sendData(base64_encode($this->SMTPPass));
	$reply = $this->getSMTPData();
	if (strpos($reply, '235') !== 0)
	{
		$this->setErrorMessage(lang('Email.SMTPAuthPassword', [$reply]));
		return false;
	}
	if ($this->SMTPKeepAlive)
	{
		$this->SMTPAuth = false;
	}
	return true;
}
```

</details>


<hr>

#### sendData()

```php
protected function sendData($data)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Send SMTP data
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
<td><code>$data</code></td>
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
<summary><small>Source: 36 lines (2014 - 2049)</small></summary>

```php
protected function sendData($data)
{
	$data .= $this->newline;
	for ($written = $timestamp = 0, $length = static::strlen($data); $written < $length; $written += $result)
	{
		if (($result = fwrite($this->SMTPConnect, static::substr($data, $written))) === false)
		{
			break;
		}
		// See https://bugs.php.net/bug.php?id=39598 and http://php.net/manual/en/function.fwrite.php#96951
		elseif ($result === 0)
		{
			if ($timestamp === 0)
			{
				$timestamp = time();
			}
			elseif ($timestamp < (time() - $this->SMTPTimeout))
			{
				$result = false;
				break;
			}
			usleep(250000);
			continue;
		}
		else
		{
			$timestamp = 0;
		}
	}
	if ($result === false)
	{
		$this->setErrorMessage(lang('Email.SMTPDataFailure', $data));
		return false;
	}
	return true;
}
```

</details>


<hr>

#### getSMTPData()

```php
protected function getSMTPData()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get SMTP data
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
<summary><small>Source: 13 lines (2056 - 2068)</small></summary>

```php
protected function getSMTPData()
{
	$data = '';
	while ($str = fgets($this->SMTPConnect, 512))
	{
		$data .= $str;
		if ($str[3] === ' ')
		{
			break;
		}
	}
	return $data;
}
```

</details>


<hr>

#### getHostname()

```php
protected function getHostname()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get Hostname
</td></tr>
</table>

<table>
<tr><td>
There are only two legal types of hostname - either a fully
qualified domain name (eg: "mail.example.com") or an IP literal
(eg: "[1.2.3.4]").
</td></tr>
</table>

</details>



<table style="text-align:left">
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="https://tools.ietf.org/html/rfc5321#section-2.3.5">https://tools.ietf.org/html/rfc5321#section-2.3.5</a>

</td>
</tr>
<tr style="vertical-align:top;">
<th>link</th>
<td><a href="http://cbl.abuseat.org/namingproblems.html">http://cbl.abuseat.org/namingproblems.html</a>

</td>
</tr>
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>string
</td>
</tr>
</table>





<details>
<summary><small>Source: 8 lines (2082 - 2089)</small></summary>

```php
protected function getHostname()
{
	if (isset($_SERVER['SERVER_NAME']))
	{
		return $_SERVER['SERVER_NAME'];
	}
	return isset($_SERVER['SERVER_ADDR']) ? '[' . $_SERVER['SERVER_ADDR'] . ']' : '[127.0.0.1]';
}
```

</details>


<hr>

#### printDebugger()

```php
public function printDebugger($include = array('headers', 'subject', 'body'))
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Get Debug Message
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
<td><code>$include</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>List of raw data chunks to include in the output
Valid options are: 'headers', 'subject', 'body'</td>
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
<summary><small>Source: 11 lines (2099 - 2109)</small></summary>

```php
public function printDebugger($include = ['headers', 'subject', 'body'])
{
	$msg = implode('', $this->debugMessage);
	// Determine which parts of our raw data needs to be printed
	$raw_data                                         = '';
	is_array($include) || $include                    = [$include];
	in_array('headers', $include, true) && $raw_data  = htmlspecialchars($this->headerStr) . "\n";
	in_array('subject', $include, true) && $raw_data .= htmlspecialchars($this->subject) . "\n";
	in_array('body', $include, true) && $raw_data    .= htmlspecialchars($this->finalBody);
	return $msg . ($raw_data === '' ? '' : '<pre>' . $raw_data . '</pre>');
}
```

</details>


<hr>

#### setErrorMessage()

```php
protected function setErrorMessage($msg)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set Message
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
<td><code>$msg</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 4 lines (2116 - 2119)</small></summary>

```php
protected function setErrorMessage($msg)
{
	$this->debugMessage[] = $msg . '<br />';
}
```

</details>


<hr>

#### mimeTypes()

```php
protected function mimeTypes($ext = '')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Mime Types
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
<td><code>$ext</code></td>
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
<summary><small>Source: 5 lines (2128 - 2132)</small></summary>

```php
protected function mimeTypes($ext = '')
{
	$mime = Mimes::guessTypeFromExtension(strtolower($ext));
	return ! empty($mime) ? $mime : 'application/x-unknown-content-type';
}
```

</details>


<hr>

#### __destruct()

```php
public function __destruct()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Destructor
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>










<details>
<summary><small>Source: 4 lines (2137 - 2140)</small></summary>

```php
public function __destruct()
{
	is_resource($this->SMTPConnect) && $this->sendCommand('quit');
}
```

</details>


<hr>

#### strlen()

```php
protected static function strlen($str)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Byte-safe strlen()
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
<td><code>$str</code></td>
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
<summary><small>Source: 4 lines (2149 - 2152)</small></summary>

```php
protected static function strlen($str)
{
	return (static::$func_overload) ? mb_strlen($str, '8bit') : strlen($str);
}
```

</details>


<hr>

#### substr()

```php
protected static function substr($str, $start, $length = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Byte-safe substr()
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
<td><code>$str</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$start</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$length</code></td>
<td><em>int<br>null
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
<summary><small>Source: 8 lines (2163 - 2170)</small></summary>

```php
protected static function substr($str, $start, $length = null)
{
	if (static::$func_overload)
	{
		return mb_substr($str, $start, $length, '8bit');
	}
	return isset($length) ? substr($str, $start, $length) : substr($str, $start);
}
```

</details>


<hr>

#### setArchiveValues()

```php
protected function setArchiveValues() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Determines the values that should be stored in $archive.
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
<summary><small>Source: 11 lines (2177 - 2187)</small></summary>

```php
protected function setArchiveValues(): array
{
	// Get property values and add anything prepped in tmpArchive
	$this->archive = array_merge(get_object_vars($this), $this->tmpArchive);
	unset($this->archive['archive']);

	// Clear tmpArchive for next run
	$this->tmpArchive = [];

	return $this->archive;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Email/Email.php</em></td>
<td><a href="../../../../../../api/index.md">index</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Debug/Toolbar/Collectors/Views.md">prev</a></td>
<td><a href="../../../../../../api/vendor/codeigniter4/framework/system/Encryption/EncrypterInterface.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:11**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>