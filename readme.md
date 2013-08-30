IN query bundle
===============
Sometimes you need to query a table in one database, and use the values returned by the query – say ids – to query another table in a different database on a different host. Typically, you'd take the values from the first query and use them in an IN query on the second host. 

I use Sequel Pro and recently discovered that is support bundles written by users. I wrote a bundle that allows you to copy the returned values as a comma separated string which you can use as part of an IN query.  The bundle acts on the first column of the selected rows. If the selected values are numeric, they are not quoted, otherwise, they are.

Installation:
-------------
Clone this repository (or download it as a zip file) and double-click the the CopyAsIN.spbundle file. This should launch Sequel Pro and take care of the installation automatically.

Usage:
------
The following animated gif shows an example of how you can use it:
![screencast showing usage](https://raw.github.com/deepakg/sequel-pro-in-query/master/img/screencast.gif)
