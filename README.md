# LOG
Simple way to write log information into txt file from PHP

## Key features

<ul>
<li>easy way to write variable information into a file</li>
<li>Supports diferent kinds of information, such as: string, integer, array, boolean, null</li>
</ul>
 
## Some examples

```php
LOG::setPath('Here path to log folder');
LOG::clear();
LOG::write('Here is your log information','Log title');
LOG::writeError('Here is your error log information','Error log title');
LOG::writeException('Here is exception object','Exception information');
LOG::border('Border title');
```
