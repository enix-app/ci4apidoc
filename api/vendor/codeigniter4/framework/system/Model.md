


 



<table>
<tr>
<td style="width:100%"><em>framework/system/Model.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Log/Logger.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Modules/Modules.md">next</a></td>
</tr>
</table>







# CodeIgniter 
<table style="text-align:left">
<tr><th>namespace</th><td>CodeIgniter</td></tr>
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
<td>framework/system/Model.php
</td>
</tr>
</table>

 


 
 ## Uses

<table style="text-align:left;">
<tr>
<td>
<strong>Closure</strong>
</td>
<td>Closure</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Database/BaseBuilder.md"><strong>CodeIgniter\Database\BaseBuilder</strong></a>
</td>
<td>BaseBuilder</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Database/BaseConnection.md"><strong>CodeIgniter\Database\BaseConnection</strong></a>
</td>
<td>BaseConnection</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Database/BaseResult.md"><strong>CodeIgniter\Database\BaseResult</strong></a>
</td>
<td>BaseResult</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Database/ConnectionInterface.md"><strong>CodeIgniter\Database\ConnectionInterface</strong></a>
</td>
<td>ConnectionInterface</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DatabaseException.md"><strong>CodeIgniter\Database\Exceptions\DatabaseException</strong></a>
</td>
<td>DatabaseException</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Database/Exceptions/DataException.md"><strong>CodeIgniter\Database\Exceptions\DataException</strong></a>
</td>
<td>DataException</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Exceptions/ModelException.md"><strong>CodeIgniter\Exceptions\ModelException</strong></a>
</td>
<td>ModelException</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/I18n/Time.md"><strong>CodeIgniter\I18n\Time</strong></a>
</td>
<td>Time</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Pager/Pager.md"><strong>CodeIgniter\Pager\Pager</strong></a>
</td>
<td>Pager</td>
</tr>
<tr>
<td>
<a href="../../../../../api/vendor/codeigniter4/framework/system/Validation/ValidationInterface.md"><strong>CodeIgniter\Validation\ValidationInterface</strong></a>
</td>
<td>ValidationInterface</td>
</tr>
<tr>
<td>
<strong>Config\Database</strong>
</td>
<td>Database</td>
</tr>
<tr>
<td>
<strong>ReflectionClass</strong>
</td>
<td>ReflectionClass</td>
</tr>
<tr>
<td>
<strong>ReflectionProperty</strong>
</td>
<td>ReflectionProperty</td>
</tr>
<tr>
<td>
<strong>stdClass</strong>
</td>
<td>stdClass</td>
</tr>
</table>



 
## CodeIgniter\Model

<table style="text-align:left">
<tr><th>Class</th><td>Model</td></tr>
<tr><th>Fully Qualified Name</th><td>CodeIgniter\Model</td></tr>
</table>


<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Class Model
</td></tr>
</table>

<table>
<tr><td>
The Model class provides a number of convenient features that
makes working with a database table less painful.

It will:
     - automatically connect to database
     - allow intermingling calls between db connection, the builder,
         and methods in this class.
     - simplifies pagination
     - removes the need to use Result object directly in most cases
     - allow specifying the return type (array, object, etc) with each call
     - ensure validation is run against objects when saving items
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
<th>mixin</th>
<td>BaseBuilder
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
<th><a href="#pager"><strong>pager</strong></a></th>
<td>prop</td>
<td>
public

</td>
<td>Pager instance.</td>
</tr>
<tr>
<th><a href="#table"><strong>table</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Name of database table</td>
</tr>
<tr>
<th><a href="#primaryKey"><strong>primaryKey</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The table&#039;s primary key.</td>
</tr>
<tr>
<th><a href="#insertID"><strong>insertID</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Last insert ID</td>
</tr>
<tr>
<th><a href="#DBGroup"><strong>DBGroup</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The Database connection group that
should be instantiated.</td>
</tr>
<tr>
<th><a href="#returnType"><strong>returnType</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The format that the results should be returned as.</td>
</tr>
<tr>
<th><a href="#useSoftDeletes"><strong>useSoftDeletes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>If this model should use &quot;softDeletes&quot; and
simply set a date when rows are deleted, or
do hard deletes.</td>
</tr>
<tr>
<th><a href="#allowedFields"><strong>allowedFields</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>An array of field names that are allowed
to be set by the user in inserts/updates.</td>
</tr>
<tr>
<th><a href="#useTimestamps"><strong>useTimestamps</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>If true, will set created_at, and updated_at
values during insert and update routines.</td>
</tr>
<tr>
<th><a href="#dateFormat"><strong>dateFormat</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The type of column that created_at and updated_at
are expected to.</td>
</tr>
<tr>
<th><a href="#createdField"><strong>createdField</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The column used for insert timestamps</td>
</tr>
<tr>
<th><a href="#updatedField"><strong>updatedField</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The column used for update timestamps</td>
</tr>
<tr>
<th><a href="#tempUseSoftDeletes"><strong>tempUseSoftDeletes</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Used by withDeleted to override the
model&#039;s softDelete setting.</td>
</tr>
<tr>
<th><a href="#deletedField"><strong>deletedField</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>The column used to save soft delete state</td>
</tr>
<tr>
<th><a href="#tempReturnType"><strong>tempReturnType</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Used by asArray and asObject to provide
temporary overrides of model default.</td>
</tr>
<tr>
<th><a href="#protectFields"><strong>protectFields</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether we should limit fields in inserts
and updates to those available in $allowedFields or not.</td>
</tr>
<tr>
<th><a href="#db"><strong>db</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Database Connection</td>
</tr>
<tr>
<th><a href="#builder"><strong>builder</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Query Builder object</td>
</tr>
<tr>
<th><a href="#validationRules"><strong>validationRules</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Rules used to validate data in insert, update, and save methods.</td>
</tr>
<tr>
<th><a href="#validationMessages"><strong>validationMessages</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Contains any custom error messages to be
used during data validation.</td>
</tr>
<tr>
<th><a href="#skipValidation"><strong>skipValidation</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Skip the model&#039;s validation. Used in conjunction with skipValidation()
to skip data validation for any future calls.</td>
</tr>
<tr>
<th><a href="#cleanValidationRules"><strong>cleanValidationRules</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether rules should be removed that do not exist
in the passed in data. Used between inserts/updates.</td>
</tr>
<tr>
<th><a href="#validation"><strong>validation</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Our validator instance.</td>
</tr>
<tr>
<th><a href="#allowCallbacks"><strong>allowCallbacks</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Whether to trigger the defined callbacks</td>
</tr>
<tr>
<th><a href="#tempAllowCallbacks"><strong>tempAllowCallbacks</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Used by allowCallbacks() to override the
model&#039;s allowCallbacks setting.</td>
</tr>
<tr>
<th><a href="#beforeInsert"><strong>beforeInsert</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Callbacks for beforeInsert</td>
</tr>
<tr>
<th><a href="#afterInsert"><strong>afterInsert</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Callbacks for afterInsert</td>
</tr>
<tr>
<th><a href="#beforeUpdate"><strong>beforeUpdate</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Callbacks for beforeUpdate</td>
</tr>
<tr>
<th><a href="#afterUpdate"><strong>afterUpdate</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Callbacks for afterUpdate</td>
</tr>
<tr>
<th><a href="#beforeFind"><strong>beforeFind</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Callbacks for beforeFind</td>
</tr>
<tr>
<th><a href="#afterFind"><strong>afterFind</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Callbacks for afterFind</td>
</tr>
<tr>
<th><a href="#beforeDelete"><strong>beforeDelete</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Callbacks for beforeDelete</td>
</tr>
<tr>
<th><a href="#afterDelete"><strong>afterDelete</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Callbacks for afterDelete</td>
</tr>
<tr>
<th><a href="#tempData"><strong>tempData</strong></a></th>
<td>prop</td>
<td>
protected

</td>
<td>Holds information passed in via &#039;set&#039;
so that we can capture it (not the builder)
and ensure it gets validated first.</td>
</tr>

<tr>
<th><a href="#__construct"><strong>__construct</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Model constructor.</td>
</tr>
<tr>
<th><a href="#find"><strong>find</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Fetches the row of database from $this-&gt;table with a primary key
matching $id.</td>
</tr>
<tr>
<th><a href="#findColumn"><strong>findColumn</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Fetches the column of database from $this-&gt;table</td>
</tr>
<tr>
<th><a href="#findAll"><strong>findAll</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Works with the current Query Builder instance to return
all results, while optionally limiting them.</td>
</tr>
<tr>
<th><a href="#first"><strong>first</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the first row of the result set. Will take any previous
Query Builder calls into account when determining the result set.</td>
</tr>
<tr>
<th><a href="#set"><strong>set</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Captures the builder&#039;s set() method so that we can validate the
data here. This allows it to be used with any of the other
builder methods and still get validated data, like replace.</td>
</tr>
<tr>
<th><a href="#save"><strong>save</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>A convenience method that will attempt to determine whether the
data should be inserted or updated. Will work with either
an array or object. When using with custom class objects,
you must ensure that the class will provide access to the class
variables, even if through a magic method.</td>
</tr>
<tr>
<th><a href="#classToArray"><strong>classToArray</strong>()</a></th>
<td>method</td>
<td>
public<br>static

</td>
<td>Takes a class an returns an array of it&#039;s public and protected
properties as an array suitable for use in creates and updates.</td>
</tr>
<tr>
<th><a href="#getInsertID"><strong>getInsertID</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns last insert ID or 0.</td>
</tr>
<tr>
<th><a href="#insert"><strong>insert</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Inserts data into the current table. If an object is provided,
it will attempt to convert it to an array.</td>
</tr>
<tr>
<th><a href="#insertBatch"><strong>insertBatch</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Compiles batch insert strings and runs the queries, validating each row prior.</td>
</tr>
<tr>
<th><a href="#update"><strong>update</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Updates a single record in $this-&gt;table. If an object is provided,
it will attempt to convert it into an array.</td>
</tr>
<tr>
<th><a href="#updateBatch"><strong>updateBatch</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Update_Batch</td>
</tr>
<tr>
<th><a href="#delete"><strong>delete</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Deletes a single record from $this-&gt;table where $id matches
the table&#039;s primaryKey</td>
</tr>
<tr>
<th><a href="#purgeDeleted"><strong>purgeDeleted</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Permanently deletes all rows that have been marked as deleted
through soft deletes (deleted = 1)</td>
</tr>
<tr>
<th><a href="#withDeleted"><strong>withDeleted</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets $useSoftDeletes value so that we can temporarily override
the softdeletes settings. Can be used for all find* methods.</td>
</tr>
<tr>
<th><a href="#onlyDeleted"><strong>onlyDeleted</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Works with the find* methods to return only the rows that
have been deleted.</td>
</tr>
<tr>
<th><a href="#replace"><strong>replace</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Replace</td>
</tr>
<tr>
<th><a href="#asArray"><strong>asArray</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the return type of the results to be as an associative array.</td>
</tr>
<tr>
<th><a href="#asObject"><strong>asObject</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets the return type to be of the specified type of object.</td>
</tr>
<tr>
<th><a href="#chunk"><strong>chunk</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Loops over records in batches, allowing you to operate on them.</td>
</tr>
<tr>
<th><a href="#paginate"><strong>paginate</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Works with $this-&gt;builder to get the Compiled Select to operate on.</td>
</tr>
<tr>
<th><a href="#protect"><strong>protect</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets whether or not we should whitelist data set during
updates or inserts against $this-&gt;availableFields.</td>
</tr>
<tr>
<th><a href="#builder"><strong>builder</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Provides a shared instance of the Query Builder.</td>
</tr>
<tr>
<th><a href="#doProtectFields"><strong>doProtectFields</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Ensures that only the fields that are allowed to be updated
are in the data array.</td>
</tr>
<tr>
<th><a href="#setDate"><strong>setDate</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A utility function to allow child models to use the type of
date/time format that they prefer. This is primarily used for
setting created_at, updated_at and deleted_at values, but can be
used by inheriting classes.</td>
</tr>
<tr>
<th><a href="#setTable"><strong>setTable</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Specify the table associated with a model</td>
</tr>
<tr>
<th><a href="#errors"><strong>errors</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Grabs the last error(s) that occurred. If data was validated,
it will first check for errors there, otherwise will try to
grab the last error from the Database connection.</td>
</tr>
<tr>
<th><a href="#skipValidation"><strong>skipValidation</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Set the value of the skipValidation flag.</td>
</tr>
<tr>
<th><a href="#setValidationMessages"><strong>setValidationMessages</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows to set validation messages.</td>
</tr>
<tr>
<th><a href="#setValidationMessage"><strong>setValidationMessage</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows to set field wise validation message.</td>
</tr>
<tr>
<th><a href="#setValidationRules"><strong>setValidationRules</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows to set validation rules.</td>
</tr>
<tr>
<th><a href="#setValidationRule"><strong>setValidationRule</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Allows to set field wise validation rules.</td>
</tr>
<tr>
<th><a href="#cleanRules"><strong>cleanRules</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Should validation rules be removed before saving?
Most handy when doing updates.</td>
</tr>
<tr>
<th><a href="#validate"><strong>validate</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Validate the data against the validation rules (or the validation group)
specified in the class property, $validationRules.</td>
</tr>
<tr>
<th><a href="#cleanValidationRules"><strong>cleanValidationRules</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Removes any rules that apply to fields that have not been set
currently so that rules don&#039;t block updating when only updating
a partial row.</td>
</tr>
<tr>
<th><a href="#fillPlaceholders"><strong>fillPlaceholders</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>Replace any placeholders within the rules with the values that
match the &#039;key&#039; of any properties being set. For example, if
we had the following $data array:</td>
</tr>
<tr>
<th><a href="#getValidationRules"><strong>getValidationRules</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the model&#039;s defined validation rules so that they
can be used elsewhere, if needed.</td>
</tr>
<tr>
<th><a href="#getValidationMessages"><strong>getValidationMessages</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Returns the model&#039;s define validation messages so they
can be used elsewhere, if needed.</td>
</tr>
<tr>
<th><a href="#countAllResults"><strong>countAllResults</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Override countAllResults to account for soft deleted accounts.</td>
</tr>
<tr>
<th><a href="#allowCallbacks"><strong>allowCallbacks</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Sets $tempAllowCallbacks value so that we can temporarily override
the setting. Resets after the next method that uses triggers.</td>
</tr>
<tr>
<th><a href="#trigger"><strong>trigger</strong>()</a></th>
<td>method</td>
<td>
protected

</td>
<td>A simple event trigger for Model Events that allows additional
data manipulation within the model. Specifically intended for
usage by child models this can be used to format data,
save/load related classes, etc.</td>
</tr>
<tr>
<th><a href="#__get"><strong>__get</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Provides/instantiates the builder/db connection and model&#039;s table/primary key names and return type.</td>
</tr>
<tr>
<th><a href="#__isset"><strong>__isset</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Checks for the existence of properties across this model, builder, and db connection.</td>
</tr>
<tr>
<th><a href="#__call"><strong>__call</strong>()</a></th>
<td>method</td>
<td>
public

</td>
<td>Provides direct access to method in the builder (if available)
and the database connection.</td>
</tr>

</table>





### Properties


<hr>

#### $pager

```php
public $pager;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Pager instance.
</td></tr>
</table>

<table>
<tr><td>
Populated after calling $this->paginate()
</td></tr>
</table>

</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\Pager
</td>
</tr>
</table>


<hr>

#### $table

```php
protected $table;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Name of database table
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

#### $primaryKey

```php
protected $primaryKey = 'id';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The table's primary key.
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

#### $insertID

```php
protected $insertID = 0;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Last insert ID
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

#### $DBGroup

```php
protected $DBGroup;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The Database connection group that
should be instantiated.
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

#### $returnType

```php
protected $returnType = 'array';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The format that the results should be returned as.
</td></tr>
</table>

<table>
<tr><td>
Will be overridden if the as* methods are used.
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

#### $useSoftDeletes

```php
protected $useSoftDeletes = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
If this model should use "softDeletes" and
simply set a date when rows are deleted, or
do hard deletes.
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

#### $allowedFields

```php
protected $allowedFields = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
An array of field names that are allowed
to be set by the user in inserts/updates.
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

#### $useTimestamps

```php
protected $useTimestamps = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
If true, will set created_at, and updated_at
values during insert and update routines.
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

#### $dateFormat

```php
protected $dateFormat = 'datetime';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The type of column that created_at and updated_at
are expected to.
</td></tr>
</table>

<table>
<tr><td>
Allowed: 'datetime', 'date', 'int'
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

#### $createdField

```php
protected $createdField = 'created_at';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The column used for insert timestamps
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

#### $updatedField

```php
protected $updatedField = 'updated_at';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The column used for update timestamps
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

#### $tempUseSoftDeletes

```php
protected $tempUseSoftDeletes;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used by withDeleted to override the
model's softDelete setting.
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

#### $deletedField

```php
protected $deletedField = 'deleted_at';
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
The column used to save soft delete state
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

#### $tempReturnType

```php
protected $tempReturnType;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used by asArray and asObject to provide
temporary overrides of model default.
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

#### $protectFields

```php
protected $protectFields = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether we should limit fields in inserts
and updates to those available in $allowedFields or not.
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

#### $db

```php
protected $db;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Database Connection
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\ConnectionInterface
</td>
</tr>
</table>


<hr>

#### $builder

```php
protected $builder;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Query Builder object
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\BaseBuilder
</td>
</tr>
</table>


<hr>

#### $validationRules

```php
protected $validationRules = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Rules used to validate data in insert, update, and save methods.
</td></tr>
</table>

<table>
<tr><td>
The array must match the format of data passed to the Validation
library.
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

#### $validationMessages

```php
protected $validationMessages = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Contains any custom error messages to be
used during data validation.
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

#### $skipValidation

```php
protected $skipValidation = false;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Skip the model's validation. Used in conjunction with skipValidation()
to skip data validation for any future calls.
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

#### $cleanValidationRules

```php
protected $cleanValidationRules = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether rules should be removed that do not exist
in the passed in data. Used between inserts/updates.
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

#### $validation

```php
protected $validation;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Our validator instance.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>




<table>
<tr>
<th style="vertical-align:top;">var</th>
<td>\CodeIgniter\Validation\Validation
</td>
</tr>
</table>


<hr>

#### $allowCallbacks

```php
protected $allowCallbacks = true;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Whether to trigger the defined callbacks
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

#### $tempAllowCallbacks

```php
protected $tempAllowCallbacks;
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Used by allowCallbacks() to override the
model's allowCallbacks setting.
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

#### $beforeInsert

```php
protected $beforeInsert = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callbacks for beforeInsert
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

#### $afterInsert

```php
protected $afterInsert = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callbacks for afterInsert
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

#### $beforeUpdate

```php
protected $beforeUpdate = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callbacks for beforeUpdate
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

#### $afterUpdate

```php
protected $afterUpdate = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callbacks for afterUpdate
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

#### $beforeFind

```php
protected $beforeFind = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callbacks for beforeFind
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

#### $afterFind

```php
protected $afterFind = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callbacks for afterFind
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

#### $beforeDelete

```php
protected $beforeDelete = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callbacks for beforeDelete
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

#### $afterDelete

```php
protected $afterDelete = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Callbacks for afterDelete
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

#### $tempData

```php
protected $tempData = [];
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Holds information passed in via 'set'
so that we can capture it (not the builder)
and ensure it gets validated first.
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
public function __construct(ConnectionInterface &$db = null, ValidationInterface $validation = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Model constructor.
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
<td><code>$db</code></td>
<td><em>\ConnectionInterface
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$validation</code></td>
<td><em>\ValidationInterface
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>








<details>
<summary><small>Source: 22 lines (351 - 372)</small></summary>

```php
public function __construct(ConnectionInterface &$db = null, ValidationInterface $validation = null)
{
	if ($db instanceof ConnectionInterface)
	{
		$this->db = & $db;
	}
	else
	{
		$this->db = Database::connect($this->DBGroup);
	}

	$this->tempReturnType     = $this->returnType;
	$this->tempUseSoftDeletes = $this->useSoftDeletes;
	$this->tempAllowCallbacks = $this->allowCallbacks;

	if (is_null($validation))
	{
		$validation = \Config\Services::validation(null, false);
	}

	$this->validation = $validation;
}
```

</details>


<hr>

#### find()

```php
public function find($id = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetches the row of database from $this->table with a primary key
matching $id.
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
<td><code>$id</code></td>
<td><em>mixed<br>array<br>null
</em></td>
<td>false</td>
<td>One primary key or an array of primary keys</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>object<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 53 lines (387 - 439)</small></summary>

```php
public function find($id = null)
{
	if ($this->tempAllowCallbacks)
	{
		// Call the before event and check for a return
		$eventData = $this->trigger('beforeFind', ['id' => $id, 'method' => 'find']);
		if (! empty($eventData['returnData']))
		{
			return $eventData['data'];
		}
	}
	$builder = $this->builder();

	if ($this->tempUseSoftDeletes === true)
	{
		$builder->where($this->table . '.' . $this->deletedField, null);
	}

	if (is_array($id))
	{
		$row = $builder->whereIn($this->table . '.' . $this->primaryKey, $id)
				->get();
		$row = $row->getResult($this->tempReturnType);
	}
	elseif (is_numeric($id) || is_string($id))
	{
		$row = $builder->where($this->table . '.' . $this->primaryKey, $id)
				->get();

		$row = $row->getFirstRow($this->tempReturnType);
	}
	else
	{
		$row = $builder->get();

		$row = $row->getResult($this->tempReturnType);
	}

	$eventData = [
		'id'   => $id,
		'data' => $row,
	];
	if ($this->tempAllowCallbacks)
	{
		$eventData = $this->trigger('afterFind', $eventData);
	}

	$this->tempReturnType     = $this->returnType;
	$this->tempUseSoftDeletes = $this->useSoftDeletes;
	$this->tempAllowCallbacks = $this->allowCallbacks;

	return $eventData['data'];
}
```

</details>


<hr>

#### findColumn()

```php
public function findColumn(string $columnName)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Fetches the column of database from $this->table
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
<td><code>$columnName</code></td>
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
<td>array<br>null
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Database\Exceptions\DataException
</td>
</tr>
</table>



<details>
<summary><small>Source: 13 lines (451 - 463)</small></summary>

```php
public function findColumn(string $columnName)
{
	if (strpos($columnName, ',') !== false)
	{
		throw DataException::forFindColumnHaveMultipleColumns();
	}

	$resultSet = $this->select($columnName)
					  ->asArray()
					  ->find();

	return (! empty($resultSet)) ? array_column($resultSet, $columnName) : null;
}
```

</details>


<hr>

#### findAll()

```php
public function findAll(int $limit = 0, int $offset = 0)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Works with the current Query Builder instance to return
all results, while optionally limiting them.
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
<td><code>$limit</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$offset</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 40 lines (476 - 515)</small></summary>

```php
public function findAll(int $limit = 0, int $offset = 0)
{
	if ($this->tempAllowCallbacks)
	{
		// Call the before event and check for a return
		$eventData = $this->trigger('beforeFind', ['method' => 'findAll', 'limit' => $limit, 'offset' => $offset]);
		if (! empty($eventData['returnData']))
		{
			return $eventData['data'];
		}
	}

	$builder = $this->builder();

	if ($this->tempUseSoftDeletes === true)
	{
		$builder->where($this->table . '.' . $this->deletedField, null);
	}

	$row = $builder->limit($limit, $offset)
			->get();

	$row = $row->getResult($this->tempReturnType);

	$eventData = [
		'data'   => $row,
		'limit'  => $limit,
		'offset' => $offset,
	];
	if ($this->tempAllowCallbacks)
	{
		$eventData = $this->trigger('afterFind', $eventData);
	}

	$this->tempReturnType     = $this->returnType;
	$this->tempUseSoftDeletes = $this->useSoftDeletes;
	$this->tempAllowCallbacks = $this->allowCallbacks;

	return $eventData['data'];
}
```

</details>


<hr>

#### first()

```php
public function first()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the first row of the result set. Will take any previous
Query Builder calls into account when determining the result set.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>object<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 50 lines (525 - 574)</small></summary>

```php
public function first()
{
	if ($this->tempAllowCallbacks)
	{
		// Call the before event and check for a return
		$eventData = $this->trigger('beforeFind', ['method' => 'first']);
		if (! empty($eventData['returnData']))
		{
			return $eventData['data'];
		}
	}

	$builder = $this->builder();

	if ($this->tempUseSoftDeletes === true)
	{
		$builder->where($this->table . '.' . $this->deletedField, null);
	}
	else
	{
		if ($this->useSoftDeletes === true && empty($builder->QBGroupBy) && ! empty($this->primaryKey))
		{
			$builder->groupBy($this->table . '.' . $this->primaryKey);
		}
	}

	// Some databases, like PostgreSQL, need order
	// information to consistently return correct results.
	if (! empty($builder->QBGroupBy) && empty($builder->QBOrderBy) && ! empty($this->primaryKey))
	{
		$builder->orderBy($this->table . '.' . $this->primaryKey, 'asc');
	}

	$row = $builder->limit(1, 0)
				   ->get();

	$row = $row->getFirstRow($this->tempReturnType);

	$eventData = ['data' => $row];
	if ($this->tempAllowCallbacks)
	{
		$eventData = $this->trigger('afterFind', $eventData);
	}

	$this->tempReturnType     = $this->returnType;
	$this->tempUseSoftDeletes = $this->useSoftDeletes;
	$this->tempAllowCallbacks = $this->allowCallbacks;

	return $eventData['data'];
}
```

</details>


<hr>

#### set()

```php
public function set($key, ?string $value = '', bool $escape = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Captures the builder's set() method so that we can validate the
data here. This allows it to be used with any of the other
builder methods and still get validated data, like replace.
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
<td><code>$key</code></td>
<td><em>mixed
</em></td>
<td>false</td>
<td>Field name, or an array of field/value pairs</td>
</tr>

<tr>
<td>2.</td>
<td><code>$value</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Field value, if $key is a single field</td>
</tr>

<tr>
<td>3.</td>
<td><code>$escape</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to escape values and identifiers</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (589 - 599)</small></summary>

```php
public function set($key, ?string $value = '', bool $escape = null)
{
	$data = is_array($key)
		? $key
		: [$key => $value];

	$this->tempData['escape'] = $escape;
	$this->tempData['data']   = array_merge($this->tempData['data'] ?? [], $data);

	return $this;
}
```

</details>


<hr>

#### save()

```php
public function save($data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A convenience method that will attempt to determine whether the
data should be inserted or updated. Will work with either
an array or object. When using with custom class objects,
you must ensure that the class will provide access to the class
variables, even if through a magic method.
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
<td><em>array<br>object
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 31 lines (615 - 645)</small></summary>

```php
public function save($data): bool
{
	if (empty($data))
	{
		return true;
	}

	if (is_object($data) && isset($data->{$this->primaryKey}))
	{
		$response = $this->update($data->{$this->primaryKey}, $data);
	}
	elseif (is_array($data) && ! empty($data[$this->primaryKey]))
	{
		$response = $this->update($data[$this->primaryKey], $data);
	}
	else
	{
		$response = $this->insert($data, false);

		if ($response instanceof BaseResult)
		{
			$response = $response->resultID !== false;
		}
		elseif ($response !== false)
		{
			$response = true;
		}
	}

	return $response;
}
```

</details>


<hr>

#### classToArray()

```php
public static function classToArray($data, $primaryKey = null, string $dateFormat = 'datetime', bool $onlyChanged = true) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Takes a class an returns an array of it's public and protected
properties as an array suitable for use in creates and updates.
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
<td><em>string<br>object
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$primaryKey</code></td>
<td><em>string<br>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>3.</td>
<td><code>$dateFormat</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>4.</td>
<td><code>$onlyChanged</code></td>
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
<td>array
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 59 lines (659 - 717)</small></summary>

```php
public static function classToArray($data, $primaryKey = null, string $dateFormat = 'datetime', bool $onlyChanged = true): array
{
	if (method_exists($data, 'toRawArray'))
	{
		$properties = $data->toRawArray($onlyChanged);

		// Always grab the primary key otherwise updates will fail.
		if (! empty($properties) && ! empty($primaryKey) && ! in_array($primaryKey, $properties) && ! empty($data->{$primaryKey}))
		{
			$properties[$primaryKey] = $data->{$primaryKey};
		}
	}
	else
	{
		$mirror = new ReflectionClass($data);
		$props  = $mirror->getProperties(ReflectionProperty::IS_PUBLIC | ReflectionProperty::IS_PROTECTED);

		$properties = [];

		// Loop over each property,
		// saving the name/value in a new array we can return.
		foreach ($props as $prop)
		{
			// Must make protected values accessible.
			$prop->setAccessible(true);
			$propName              = $prop->getName();
			$properties[$propName] = $prop->getValue($data);
		}
	}

	// Convert any Time instances to appropriate $dateFormat
	if ($properties)
	{
		foreach ($properties as $key => $value)
		{
			if ($value instanceof Time)
			{
				switch ($dateFormat)
				{
					case 'datetime':
						$converted = $value->format('Y-m-d H:i:s');
						break;
					case 'date':
						$converted = $value->format('Y-m-d');
						break;
					case 'int':
						$converted = $value->getTimestamp();
						break;
					default:
						$converted = (string)$value;
				}

				$properties[$key] = $converted;
			}
		}
	}

	return $properties;
}
```

</details>


<hr>

#### getInsertID()

```php
public function getInsertID() : int
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns last insert ID or 0.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (726 - 729)</small></summary>

```php
public function getInsertID(): int
{
	return $this->insertID;
}
```

</details>


<hr>

#### insert()

```php
public function insert($data = null, bool $returnID = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Inserts data into the current table. If an object is provided,
it will attempt to convert it to an array.
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
<td><em>array<br>object
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$returnID</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether insert ID should be returned or not.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BaseResult<br>int<br>string<br>false
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 103 lines (743 - 845)</small></summary>

```php
public function insert($data = null, bool $returnID = true)
{
	$escape = null;

	$this->insertID = 0;

	if (empty($data))
	{
		$data           = $this->tempData['data'] ?? null;
		$escape         = $this->tempData['escape'] ?? null;
		$this->tempData = [];
	}

	if (empty($data))
	{
		throw DataException::forEmptyDataset('insert');
	}

	// If $data is using a custom class with public or protected
	// properties representing the table elements, we need to grab
	// them as an array.
	if (is_object($data) && ! $data instanceof stdClass)
	{
		$data = static::classToArray($data, $this->primaryKey, $this->dateFormat, false);
	}

	// If it's still a stdClass, go ahead and convert to
	// an array so doProtectFields and other model methods
	// don't have to do special checks.
	if (is_object($data))
	{
		$data = (array) $data;
	}

	if (empty($data))
	{
		throw DataException::forEmptyDataset('insert');
	}

	// Validate data before saving.
	if ($this->skipValidation === false)
	{
		if ($this->cleanRules()->validate($data) === false)
		{
			return false;
		}
	}

	// Must be called first so we don't
	// strip out created_at values.
	$data = $this->doProtectFields($data);

	// Set created_at and updated_at with same time
	$date = $this->setDate();

	if ($this->useTimestamps && ! empty($this->createdField) && ! array_key_exists($this->createdField, $data))
	{
		$data[$this->createdField] = $date;
	}

	if ($this->useTimestamps && ! empty($this->updatedField) && ! array_key_exists($this->updatedField, $data))
	{
		$data[$this->updatedField] = $date;
	}

	$eventData = ['data' => $data];
	if ($this->tempAllowCallbacks)
	{
		$eventData = $this->trigger('beforeInsert', $eventData);
	}

	// Must use the set() method to ensure objects get converted to arrays
	$result = $this->builder()
			->set($eventData['data'], '', $escape)
			->insert();

	// If insertion succeeded then save the insert ID
	if ($result->resultID)
	{
		$this->insertID = $this->db->insertID();
	}

	$eventData = [
		'id'     => $this->insertID,
		'data'   => $eventData['data'],
		'result' => $result,
	];
	if ($this->tempAllowCallbacks)
	{
		// Trigger afterInsert events with the inserted data and new ID
		$this->trigger('afterInsert', $eventData);
	}
	$this->tempAllowCallbacks = $this->allowCallbacks;

	// If insertion failed, get out of here
	if (! $result)
	{
		return $result;
	}

	// otherwise return the insertID, if requested.
	return $returnID ? $this->insertID : $result;
}
```

</details>


<hr>

#### insertBatch()

```php
public function insertBatch(array $set = null, bool $escape = null, int $batchSize = 100, bool $testing = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Compiles batch insert strings and runs the queries, validating each row prior.
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
<td><code>$set</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>An associative array of insert values</td>
</tr>

<tr>
<td>2.</td>
<td><code>$escape</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Whether to escape values and identifiers</td>
</tr>

<tr>
<td>3.</td>
<td><code>$batchSize</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The size of the batch to run</td>
</tr>

<tr>
<td>4.</td>
<td><code>$testing</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>True means only number of records is returned, false will execute the query</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>int<br>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 15 lines (859 - 873)</small></summary>

```php
public function insertBatch(array $set = null, bool $escape = null, int $batchSize = 100, bool $testing = false)
{
	if (is_array($set) && $this->skipValidation === false)
	{
		foreach ($set as $row)
		{
			if ($this->cleanRules()->validate($row) === false)
			{
				return false;
			}
		}
	}

	return $this->builder()->testMode($testing)->insertBatch($set, $escape, $batchSize);
}
```

</details>


<hr>

#### update()

```php
public function update($id = null, $data = null) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Updates a single record in $this->table. If an object is provided,
it will attempt to convert it into an array.
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
<td><code>$id</code></td>
<td><em>int<br>array<br>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$data</code></td>
<td><em>array<br>object
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


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\ReflectionException
</td>
</tr>
</table>



<details>
<summary><small>Source: 95 lines (887 - 981)</small></summary>

```php
public function update($id = null, $data = null): bool
{
	$escape = null;

	if (is_numeric($id) || is_string($id))
	{
		$id = [$id];
	}

	if (empty($data))
	{
		$data           = $this->tempData['data'] ?? null;
		$escape         = $this->tempData['escape'] ?? null;
		$this->tempData = [];
	}

	if (empty($data))
	{
		throw DataException::forEmptyDataset('update');
	}

	// If $data is using a custom class with public or protected
	// properties representing the table elements, we need to grab
	// them as an array.
	if (is_object($data) && ! $data instanceof stdClass)
	{
		$data = static::classToArray($data, $this->primaryKey, $this->dateFormat);
	}

	// If it's still a stdClass, go ahead and convert to
	// an array so doProtectFields and other model methods
	// don't have to do special checks.
	if (is_object($data))
	{
		$data = (array) $data;
	}

	// If it's still empty here, means $data is no change or is empty object
	if (empty($data))
	{
		throw DataException::forEmptyDataset('update');
	}

	// Validate data before saving.
	if ($this->skipValidation === false)
	{
		if ($this->cleanRules(true)->validate($data) === false)
		{
			return false;
		}
	}

	// Must be called first so we don't
	// strip out updated_at values.
	$data = $this->doProtectFields($data);

	if ($this->useTimestamps && ! empty($this->updatedField) && ! array_key_exists($this->updatedField, $data))
	{
		$data[$this->updatedField] = $this->setDate();
	}

	$eventData = [
		'id'   => $id,
		'data' => $data,
	];
	if ($this->tempAllowCallbacks)
	{
		$eventData = $this->trigger('beforeUpdate', $eventData);
	}

	$builder = $this->builder();

	if ($id)
	{
		$builder = $builder->whereIn($this->table . '.' . $this->primaryKey, $id);
	}

	// Must use the set() method to ensure objects get converted to arrays
	$result = $builder
			->set($eventData['data'], '', $escape)
			->update();

	$eventData = [
		'id'     => $id,
		'data'   => $eventData['data'],
		'result' => $result,
	];
	if ($this->tempAllowCallbacks)
	{
		$this->trigger('afterUpdate', $eventData);
	}
	$this->tempAllowCallbacks = $this->allowCallbacks;

	return $result;
}
```

</details>


<hr>

#### updateBatch()

```php
public function updateBatch(array $set = null, string $index = null, int $batchSize = 100, bool $returnSQL = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Update_Batch
</td></tr>
</table>

<table>
<tr><td>
Compiles an update string and runs the query
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
<td><code>$set</code></td>
<td><em>array
</em></td>
<td>false</td>
<td>An associative array of update values</td>
</tr>

<tr>
<td>2.</td>
<td><code>$index</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>The where key</td>
</tr>

<tr>
<td>3.</td>
<td><code>$batchSize</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>The size of the batch to run</td>
</tr>

<tr>
<td>4.</td>
<td><code>$returnSQL</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>True means SQL is returned, false will execute the query</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Database\Exceptions\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 15 lines (998 - 1012)</small></summary>

```php
public function updateBatch(array $set = null, string $index = null, int $batchSize = 100, bool $returnSQL = false)
{
	if (is_array($set) && $this->skipValidation === false)
	{
		foreach ($set as $row)
		{
			if ($this->cleanRules(true)->validate($row) === false)
			{
				return false;
			}
		}
	}

	return $this->builder()->testMode($returnSQL)->updateBatch($set, $index, $batchSize);
}
```

</details>


<hr>

#### delete()

```php
public function delete($id = null, bool $purge = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Deletes a single record from $this->table where $id matches
the table's primaryKey
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
<td><code>$id</code></td>
<td><em>int<br>string<br>array<br>null
</em></td>
<td>false</td>
<td>The rows primary key(s)</td>
</tr>

<tr>
<td>2.</td>
<td><code>$purge</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Allows overriding the soft deletes setting.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\BaseResult<br>bool
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Database\Exceptions\DatabaseException
</td>
</tr>
</table>



<details>
<summary><small>Source: 62 lines (1026 - 1087)</small></summary>

```php
public function delete($id = null, bool $purge = false)
{
	if (! empty($id) && (is_numeric($id) || is_string($id)))
	{
		$id = [$id];
	}

	$builder = $this->builder();
	if (! empty($id))
	{
		$builder = $builder->whereIn($this->primaryKey, $id);
	}

	$eventData = [
		'id'    => $id,
		'purge' => $purge,
	];
	if ($this->tempAllowCallbacks)
	{
		$this->trigger('beforeDelete', $eventData);
	}

	if ($this->useSoftDeletes && ! $purge)
	{
		if (empty($builder->getCompiledQBWhere()))
		{
			if (CI_DEBUG)
			{
				throw new DatabaseException('Deletes are not allowed unless they contain a "where" or "like" clause.');
			}
			// @codeCoverageIgnoreStart
			return false;
			// @codeCoverageIgnoreEnd
		}
		$set[$this->deletedField] = $this->setDate();

		if ($this->useTimestamps && ! empty($this->updatedField))
		{
			$set[$this->updatedField] = $this->setDate();
		}

		$result = $builder->update($set);
	}
	else
	{
		$result = $builder->delete();
	}

	$eventData = [
		'id'     => $id,
		'purge'  => $purge,
		'result' => $result,
		'data'   => null,
	];
	if ($this->tempAllowCallbacks)
	{
		$this->trigger('afterDelete', $eventData);
	}
	$this->tempAllowCallbacks = $this->allowCallbacks;

	return $result;
}
```

</details>


<hr>

#### purgeDeleted()

```php
public function purgeDeleted()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Permanently deletes all rows that have been marked as deleted
through soft deletes (deleted = 1)
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>bool<br>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 11 lines (1097 - 1107)</small></summary>

```php
public function purgeDeleted()
{
	if (! $this->useSoftDeletes)
	{
		return true;
	}

	return $this->builder()
			->where($this->table . '.' . $this->deletedField . ' IS NOT NULL')
			->delete();
}
```

</details>


<hr>

#### withDeleted()

```php
public function withDeleted($val = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets $useSoftDeletes value so that we can temporarily override
the softdeletes settings. Can be used for all find* methods.
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
<td><code>$val</code></td>
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
<td>\Model
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1119 - 1124)</small></summary>

```php
public function withDeleted($val = true)
{
	$this->tempUseSoftDeletes = ! $val;

	return $this;
}
```

</details>


<hr>

#### onlyDeleted()

```php
public function onlyDeleted()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Works with the find* methods to return only the rows that
have been deleted.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Model
</td>
</tr>
</table>





<details>
<summary><small>Source: 9 lines (1134 - 1142)</small></summary>

```php
public function onlyDeleted()
{
	$this->tempUseSoftDeletes = false;

	$this->builder()
		 ->where($this->table . '.' . $this->deletedField . ' IS NOT NULL');

	return $this;
}
```

</details>


<hr>

#### replace()

```php
public function replace($data = null, bool $returnSQL = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replace
</td></tr>
</table>

<table>
<tr><td>
Compiles an replace into string and runs the query
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
<td><em>null
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$returnSQL</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 13 lines (1156 - 1168)</small></summary>

```php
public function replace($data = null, bool $returnSQL = false)
{
	// Validate data before saving.
	if (! empty($data) && $this->skipValidation === false)
	{
		if ($this->cleanRules(true)->validate($data) === false)
		{
			return false;
		}
	}

	return $this->builder()->replace($data, $returnSQL);
}
```

</details>


<hr>

#### asArray()

```php
public function asArray()
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the return type of the results to be as an associative array.
</td></tr>
</table>


</details>



<table style="text-align:left">
</table>





<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>\Model
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1179 - 1184)</small></summary>

```php
public function asArray()
{
	$this->tempReturnType = 'array';

	return $this;
}
```

</details>


<hr>

#### asObject()

```php
public function asObject(string $class = 'object')
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets the return type to be of the specified type of object.
</td></tr>
</table>

<table>
<tr><td>
Defaults to a simple object, but can be any class that has
class vars with the same name as the table columns, or at least
allows them to be created.
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
<td><code>$class</code></td>
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
<td>\Model
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1198 - 1203)</small></summary>

```php
public function asObject(string $class = 'object')
{
	$this->tempReturnType = $class;

	return $this;
}
```

</details>


<hr>

#### chunk()

```php
public function chunk(int $size, Closure $userFunc)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Loops over records in batches, allowing you to operate on them.
</td></tr>
</table>

<table>
<tr><td>
Works with $this->builder to get the Compiled select to
determine the rows to operate on.
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
<td><code>$size</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$userFunc</code></td>
<td><em>\Closure
</em></td>
<td>false</td>
<td></td>
</tr>


</tbody>
</table>





<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Database\Exceptions\DataException
</td>
</tr>
</table>



<details>
<summary><small>Source: 36 lines (1217 - 1252)</small></summary>

```php
public function chunk(int $size, Closure $userFunc)
{
	$total = $this->builder()
			->countAllResults(false);

	$offset = 0;

	while ($offset <= $total)
	{
		$builder = clone($this->builder());

		$rows = $builder->get($size, $offset);

		if ($rows === false)
		{
			throw DataException::forEmptyDataset('chunk');
		}

		$rows = $rows->getResult($this->tempReturnType);

		$offset += $size;

		if (empty($rows))
		{
			continue;
		}

		foreach ($rows as $row)
		{
			if ($userFunc($row) === false)
			{
				return;
			}
		}
	}
}
```

</details>


<hr>

#### paginate()

```php
public function paginate(int $perPage = null, string $group = 'default', int $page = null, int $segment = 0)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Works with $this->builder to get the Compiled Select to operate on.
</td></tr>
</table>

<table>
<tr><td>
Expects a GET variable (?page=2) that specifies the page of results
to display.
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
<td><code>$perPage</code></td>
<td><em>int
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$group</code></td>
<td><em>string
</em></td>
<td>false</td>
<td>Will be used by the pagination library
to identify a unique pagination set.</td>
</tr>

<tr>
<td>3.</td>
<td><code>$page</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Optional page number (useful when the page number is provided in different way)</td>
</tr>

<tr>
<td>4.</td>
<td><code>$segment</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>Optional URI segment number (if page number is provided by URI segment)</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 21 lines (1269 - 1289)</small></summary>

```php
public function paginate(int $perPage = null, string $group = 'default', int $page = null, int $segment = 0)
{
	$pager = \Config\Services::pager(null, null, false);

	if ($segment)
	{
		$pager->setSegment($segment);
	}

	$page = $page >= 1 ? $page : $pager->getCurrentPage($group);

	$total = $this->countAllResults(false);

	// Store it in the Pager library so it can be
	// paginated in the views.
	$this->pager = $pager->store($group, $page, $perPage, $total, $segment);
	$perPage     = $this->pager->getPerPage($group);
	$offset      = ($page - 1) * $perPage;

	return $this->findAll($perPage, $offset);
}
```

</details>


<hr>

#### protect()

```php
public function protect(bool $protect = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets whether or not we should whitelist data set during
updates or inserts against $this->availableFields.
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
<td><code>$protect</code></td>
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
<td>\Model
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1301 - 1306)</small></summary>

```php
public function protect(bool $protect = true)
{
	$this->protectFields = $protect;

	return $this;
}
```

</details>


<hr>

#### builder()

```php
protected function builder(string $table = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides a shared instance of the Query Builder.
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
<td><code>$table</code></td>
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
<td>\BaseBuilder
</td>
</tr>
</table>





<details>
<summary><small>Source: 27 lines (1318 - 1344)</small></summary>

```php
protected function builder(string $table = null)
{
	if ($this->builder instanceof BaseBuilder)
	{
		return $this->builder;
	}

	// We're going to force a primary key to exist
	// so we don't have overly convoluted code,
	// and future features are likely to require them.
	if (empty($this->primaryKey))
	{
		throw ModelException::forNoPrimaryKey(get_class($this));
	}

	$table = empty($table) ? $this->table : $table;

	// Ensure we have a good db connection
	if (! $this->db instanceof BaseConnection)
	{
		$this->db = Database::connect($this->DBGroup);
	}

	$this->builder = $this->db->table($table);

	return $this->builder;
}
```

</details>


<hr>

#### doProtectFields()

```php
protected function doProtectFields(array $data) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Ensures that only the fields that are allowed to be updated
are in the data array.
</td></tr>
</table>

<table>
<tr><td>
Used by insert() and update() to protect against mass assignment
vulnerabilities.
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
<td>array
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Database\Exceptions\DataException
</td>
</tr>
</table>



<details>
<summary><small>Source: 22 lines (1360 - 1381)</small></summary>

```php
protected function doProtectFields(array $data): array
{
	if ($this->protectFields === false)
	{
		return $data;
	}

	if (empty($this->allowedFields))
	{
		throw DataException::forInvalidAllowedFields(get_class($this));
	}

	foreach ($data as $key => $val)
	{
		if (! in_array($key, $this->allowedFields))
		{
			unset($data[$key]);
		}
	}

	return $data;
}
```

</details>


<hr>

#### setDate()

```php
protected function setDate(int $userData = null)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A utility function to allow child models to use the type of
date/time format that they prefer. This is primarily used for
setting created_at, updated_at and deleted_at values, but can be
used by inheriting classes.
</td></tr>
</table>

<table>
<tr><td>
The available time formats are:
- 'int'      - Stores the date as an integer timestamp
- 'datetime' - Stores the data in the SQL datetime format
- 'date'     - Stores the date (only) in the SQL date format.
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
<td><code>$userData</code></td>
<td><em>int
</em></td>
<td>false</td>
<td>An optional PHP timestamp to be converted.</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 16 lines (1401 - 1416)</small></summary>

```php
protected function setDate(int $userData = null)
{
	$currentDate = is_numeric($userData) ? (int) $userData : time();

	switch ($this->dateFormat)
	{
		case 'int':
			return $currentDate;
		case 'datetime':
			return date('Y-m-d H:i:s', $currentDate);
		case 'date':
			return date('Y-m-d', $currentDate);
		default:
			throw ModelException::forNoDateFormat(get_class($this));
	}
}
```

</details>


<hr>

#### setTable()

```php
public function setTable(string $table)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Specify the table associated with a model
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
<td><code>$table</code></td>
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
<td>\Model
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1427 - 1432)</small></summary>

```php
public function setTable(string $table)
{
	$this->table = $table;

	return $this;
}
```

</details>


<hr>

#### errors()

```php
public function errors(bool $forceDB = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Grabs the last error(s) that occurred. If data was validated,
it will first check for errors there, otherwise will try to
grab the last error from the Database connection.
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
<td><code>$forceDB</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td>Always grab the db error, not validation</td>
</tr>


</tbody>
</table>



<table>
<tr>
<th style="vertical-align:top;">return</th>
<td>array<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (1445 - 1462)</small></summary>

```php
public function errors(bool $forceDB = false)
{
	// Do we have validation errors?
	if ($forceDB === false && $this->skipValidation === false)
	{
		$errors = $this->validation->getErrors();

		if (! empty($errors))
		{
			return $errors;
		}
	}

	// Still here? Grab the database-specific error, if any.
	$error = $this->db->error();

	return $error['message'] ?? null;
}
```

</details>


<hr>

#### skipValidation()

```php
public function skipValidation(bool $skip = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Set the value of the skipValidation flag.
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
<td><code>$skip</code></td>
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
<td>\Model
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1476 - 1481)</small></summary>

```php
public function skipValidation(bool $skip = true)
{
	$this->skipValidation = $skip;

	return $this;
}
```

</details>


<hr>

#### setValidationMessages()

```php
public function setValidationMessages(array $validationMessages)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows to set validation messages.
</td></tr>
</table>

<table>
<tr><td>
It could be used when you have to change default or override current validate messages.
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
<td><code>$validationMessages</code></td>
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (1493 - 1496)</small></summary>

```php
public function setValidationMessages(array $validationMessages)
{
	$this->validationMessages = $validationMessages;
}
```

</details>


<hr>

#### setValidationMessage()

```php
public function setValidationMessage(string $field, array $fieldMessages)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows to set field wise validation message.
</td></tr>
</table>

<table>
<tr><td>
It could be used when you have to change default or override current validate messages.
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
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$fieldMessages</code></td>
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (1508 - 1511)</small></summary>

```php
public function setValidationMessage(string $field, array $fieldMessages)
{
	$this->validationMessages[$field] = $fieldMessages;
}
```

</details>


<hr>

#### setValidationRules()

```php
public function setValidationRules(array $validationRules)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows to set validation rules.
</td></tr>
</table>

<table>
<tr><td>
It could be used when you have to change default or override current validate rules.
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
<td><code>$validationRules</code></td>
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (1523 - 1526)</small></summary>

```php
public function setValidationRules(array $validationRules)
{
	$this->validationRules = $validationRules;
}
```

</details>


<hr>

#### setValidationRule()

```php
public function setValidationRule(string $field, $fieldRules)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Allows to set field wise validation rules.
</td></tr>
</table>

<table>
<tr><td>
It could be used when you have to change default or override current validate rules.
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
<td><code>$field</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$fieldRules</code></td>
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
<td>void
</td>
</tr>
</table>





<details>
<summary><small>Source: 4 lines (1539 - 1542)</small></summary>

```php
public function setValidationRule(string $field, $fieldRules)
{
	$this->validationRules[$field] = $fieldRules;
}
```

</details>


<hr>

#### cleanRules()

```php
public function cleanRules(bool $choice = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Should validation rules be removed before saving?
Most handy when doing updates.
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
<td><code>$choice</code></td>
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
<td>$this
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1554 - 1559)</small></summary>

```php
public function cleanRules(bool $choice = false)
{
	$this->cleanValidationRules = $choice;

	return $this;
}
```

</details>


<hr>

#### validate()

```php
public function validate($data) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Validate the data against the validation rules (or the validation group)
specified in the class property, $validationRules.
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
<td><em>array<br>object
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
<summary><small>Source: 39 lines (1571 - 1609)</small></summary>

```php
public function validate($data): bool
{
	$rules = $this->getValidationRules();

	if ($this->skipValidation === true || empty($rules) || empty($data))
	{
		return true;
	}

	// Query Builder works with objects as well as arrays,
	// but validation requires array, so cast away.
	if (is_object($data))
	{
		$data = (array) $data;
	}

	// ValidationRules can be either a string, which is the group name,
	// or an array of rules.
	if (is_string($rules))
	{
		$rules = $this->validation->loadRuleGroup($rules);
	}

	$rules = $this->cleanValidationRules
		? $this->cleanValidationRules($rules, $data)
		: $rules;

	// If no data existed that needs validation
	// our job is done here.
	if (empty($rules))
	{
		return true;
	}

	$this->validation->setRules($rules, $this->validationMessages);
	$valid = $this->validation->run($data, null, $this->DBGroup);

	return (bool) $valid;
}
```

</details>


<hr>

#### cleanValidationRules()

```php
protected function cleanValidationRules(array $rules, array $data = null) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Removes any rules that apply to fields that have not been set
currently so that rules don't block updating when only updating
a partial row.
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
<td><code>$rules</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$data</code></td>
<td><em>array<br>null
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
<summary><small>Source: 17 lines (1624 - 1640)</small></summary>

```php
protected function cleanValidationRules(array $rules, array $data = null): array
{
	if (empty($data))
	{
		return [];
	}

	foreach ($rules as $field => $rule)
	{
		if (! array_key_exists($field, $data))
		{
			unset($rules[$field]);
		}
	}

	return $rules;
}
```

</details>


<hr>

#### fillPlaceholders()

```php
protected function fillPlaceholders(array $rules, array $data) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Replace any placeholders within the rules with the values that
match the 'key' of any properties being set. For example, if
we had the following $data array:
</td></tr>
</table>

<table>
<tr><td>
[ 'id' => 13 ]

and the following rule:

 'required|is_unique[users,email,id,{id}]'

The value of {id} would be replaced with the actual id in the form data:

 'required|is_unique[users,email,id,13]'
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
<td><code>$rules</code></td>
<td><em>array
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$data</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 35 lines (1666 - 1700)</small></summary>

```php
protected function fillPlaceholders(array $rules, array $data): array
{
	$replacements = [];

	foreach ($data as $key => $value)
	{
		$replacements["{{$key}}"] = $value;
	}

	if (! empty($replacements))
	{
		foreach ($rules as &$rule)
		{
			if (is_array($rule))
			{
				foreach ($rule as &$row)
				{
					// Should only be an `errors` array
					// which doesn't take placeholders.
					if (is_array($row))
					{
						continue;
					}

					$row = strtr($row, $replacements);
				}
				continue;
			}

			$rule = strtr($rule, $replacements);
		}
	}

	return $rules;
}
```

</details>


<hr>

#### getValidationRules()

```php
public function getValidationRules(array $options = array()) : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the model's defined validation rules so that they
can be used elsewhere, if needed.
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
<td><code>$options</code></td>
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
<td>array
</td>
</tr>
</table>





<details>
<summary><small>Source: 22 lines (1712 - 1733)</small></summary>

```php
public function getValidationRules(array $options = []): array
{
	$rules = $this->validationRules;

	// ValidationRules can be either a string, which is the group name,
	// or an array of rules.
	if (is_string($rules))
	{
		$rules = $this->validation->loadRuleGroup($rules);
	}

	if (isset($options['except']))
	{
		$rules = array_diff_key($rules, array_flip($options['except']));
	}
	elseif (isset($options['only']))
	{
		$rules = array_intersect_key($rules, array_flip($options['only']));
	}

	return $rules;
}
```

</details>


<hr>

#### getValidationMessages()

```php
public function getValidationMessages() : array
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Returns the model's define validation messages so they
can be used elsewhere, if needed.
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
<summary><small>Source: 4 lines (1743 - 1746)</small></summary>

```php
public function getValidationMessages(): array
{
	return $this->validationMessages;
}
```

</details>


<hr>

#### countAllResults()

```php
public function countAllResults(bool $reset = true, bool $test = false)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Override countAllResults to account for soft deleted accounts.
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
<td><code>$reset</code></td>
<td><em>bool
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$test</code></td>
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 18 lines (1758 - 1775)</small></summary>

```php
public function countAllResults(bool $reset = true, bool $test = false)
{
	if ($this->tempUseSoftDeletes === true)
	{
		$this->builder()->where($this->table . '.' . $this->deletedField, null);
	}

	// When $reset === false, the $tempUseSoftDeletes will be
	// dependant on $useSoftDeletes value because we don't
	// want to add the same "where" condition for the second time
	$this->tempUseSoftDeletes = ($reset === true)
		? $this->useSoftDeletes
		: ($this->useSoftDeletes === true
			? false
			: $this->useSoftDeletes);

	return $this->builder()->testMode($test)->countAllResults($reset);
}
```

</details>


<hr>

#### allowCallbacks()

```php
public function allowCallbacks(bool $val = true)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Sets $tempAllowCallbacks value so that we can temporarily override
the setting. Resets after the next method that uses triggers.
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
<td><code>$val</code></td>
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
<td>\Model
</td>
</tr>
</table>





<details>
<summary><small>Source: 6 lines (1785 - 1790)</small></summary>

```php
public function allowCallbacks(bool $val = true)
{
	$this->tempAllowCallbacks = $val;

	return $this;
}
```

</details>


<hr>

#### trigger()

```php
protected function trigger(string $event, array $eventData)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
A simple event trigger for Model Events that allows additional
data manipulation within the model. Specifically intended for
usage by child models this can be used to format data,
save/load related classes, etc.
</td></tr>
</table>

<table>
<tr><td>
It is the responsibility of the callback methods to return
the data itself.

Each $eventData array MUST have a 'data' key with the relevant
data for callback methods (like an array of key/value pairs to insert
or update, an array of results, etc)

If callbacks are not allowed then returns $eventData immediately.
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
<td><code>$event</code></td>
<td><em>string
</em></td>
<td>false</td>
<td></td>
</tr>

<tr>
<td>2.</td>
<td><code>$eventData</code></td>
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
<td>mixed
</td>
</tr>
</table>


<table>
<tr>
<th style="vertical-align:top;">throw</th>
<td>\CodeIgniter\Database\Exceptions\DataException
</td>
</tr>
</table>



<details>
<summary><small>Source: 20 lines (1813 - 1832)</small></summary>

```php
protected function trigger(string $event, array $eventData)
{
	// Ensure it's a valid event
	if (! isset($this->{$event}) || empty($this->{$event}))
	{
		return $eventData;
	}

	foreach ($this->{$event} as $callback)
	{
		if (! method_exists($this, $callback))
		{
			throw DataException::forInvalidMethodTriggered($callback);
		}

		$eventData = $this->{$callback}($eventData);
	}

	return $eventData;
}
```

</details>


<hr>

#### __get()

```php
public function __get(string $name)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides/instantiates the builder/db connection and model's table/primary key names and return type.
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
<td>mixed
</td>
</tr>
</table>





<details>
<summary><small>Source: 17 lines (1847 - 1863)</small></summary>

```php
public function __get(string $name)
{
	if (property_exists($this, $name))
	{
		return $this->{$name};
	}
	elseif (isset($this->db->$name))
	{
		return $this->db->$name;
	}
	elseif (isset($this->builder()->$name))
	{
		return $this->builder()->$name;
	}

	return null;
}
```

</details>


<hr>

#### __isset()

```php
public function __isset(string $name) : bool
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Checks for the existence of properties across this model, builder, and db connection.
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
<td>bool
</td>
</tr>
</table>





<details>
<summary><small>Source: 17 lines (1872 - 1888)</small></summary>

```php
public function __isset(string $name): bool
{
	if (property_exists($this, $name))
	{
		return true;
	}
	elseif (isset($this->db->$name))
	{
		return true;
	}
	elseif (isset($this->builder()->$name))
	{
		return true;
	}

	return false;
}
```

</details>


<hr>

#### __call()

```php
public function __call(string $name, array $params)
```

<details>
<summary style="margin-bottom:12px;"><strong>Description</strong></summary>

<table>
<tr><td>
Provides direct access to method in the builder (if available)
and the database connection.
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

<tr>
<td>2.</td>
<td><code>$params</code></td>
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
<td>\Model<br>null
</td>
</tr>
</table>





<details>
<summary><small>Source: 32 lines (1901 - 1932)</small></summary>

```php
public function __call(string $name, array $params)
{
	$result = null;

	if (method_exists($this->db, $name))
	{
		$result = $this->db->$name(...$params);
	}
	elseif (method_exists($builder = $this->builder(), $name))
	{
		$result = $builder->$name(...$params);
	}

	// Don't return the builder object unless specifically requested
	//, since that will interrupt the usability flow
	// and break intermingling of model and builder methods.
	if ($name !== 'builder' && empty($result))
	{
		if (! method_exists($this->builder(), $name))
		{
			$className = get_class($this);
			throw new \BadMethodCallException("Call to undefined method $className::$name");
		}
		return $result;
	}
	if ($name !== 'builder' && ! $result instanceof BaseBuilder)
	{
		return $result;
	}

	return $this;
}
```

</details>





 


 
  




<hr>

<table>
<tr>
<td style="width:100%"><em>framework/system/Model.php</em></td>
<td><a href="../../../../../api/index.md">index</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Log/Logger.md">prev</a></td>
<td><a href="../../../../../api/vendor/codeigniter4/framework/system/Modules/Modules.md">next</a></td>
<td><a href="#">top</a></td></tr>
</table>




<div style="text-align:right;">

<small>_Generated at **2020-08-14 07:35:14**_ *([EnixApp](https://github.com/enix-app) - [ApiDoc](https://github.com/enix-app/apidoc))*</small>
</div>