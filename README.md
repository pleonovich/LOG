# LOG
Simple way to write log information into txt file from PHP

Key features:

<ul>
<li>easy way to write variable information into a file</li>
<li>Supports diferent kinds of information, such as: string, integer, array, boolean, null</li>
</ul>
 
Some examples:

<ul>
<li>LOG::setPath('Here path to log folder');</li>
<li>LOG::write('Here is your log information','Log title');</li>
<li>LOG::writeError('Here is your error log information','Error log title');</li>
<li>LOG::writeException('Here is exception object','Exception information');</li>
<li>LOG::clear();</li>
<li>LOG::border('Border title');</li>
</ul>
