# LOG
Simple way to write log information into txt file from PHP

## Key features

<ul>
<li>easy way to write variable information into a file</li>
<li>Supports diferent kinds of information, such as: string, integer, array, boolean, null</li>
</ul>
 
## Some examples

### setPath
Setting path to log files folder.
```php
// Description:
void setPath ( string $path )

// example:
LOG::setPath('Here path to log folder');
```
### clear
Clear current log file.
```php
// Description:
void clear ()

// example:
LOG::clear();
```
### write
```php
// Description:
void write ( string|array|boolean|int|null $text [, string $title = null [, string $filename = null ]] )

// example:
LOG::write('Here is your log information','Log title', 'test');

// result in file - 25.06.2017.test.log.txt
// [2017.06.25][06:50:30][Log title] string(28) "Here is your log information"
```
### writeError
```php
// Description:
void writeError ( string $text [, string $title = null ] )

// example:
LOG::writeError('Here is your error log information','Error log title');

// result in file - 25.06.2017.error.log.txt
// [2017.06.25][07:22:01][Error log title] string(34) "Here is your error log information"
```
### writeException
```php
// Description:
void writeException ( Exception $e [, string $title = null ] )

// example:
LOG::writeException('Here is exception object','Exception information');
```
### border
```php
// Description:
void border ( [ string $title = 'BORDER' ] )

// example:
LOG::border('Border title');
// result in file - 25.06.2017.log.txt
//////////Border title////////////////////////////////////////////////////////////////////////////////
```
