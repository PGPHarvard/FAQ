# Navigation

* [Back to FAQ Home](README.md)
* [Back to Harvard PGP Home](http://my.pgp-hms.org)

# Researcher Requests for PGP Data
We've recently created a consolidated database of the Harvard PGP data.  We're in the process of putting a link up to the database from the Harvard PGP site but in the mean time you can get a SQLite version of the database by downloading it from the following page:

  http://curoverse.link/22d61dd43786c65cd175b04ad6954af0+3119/html/index.html

 The gzipped database is called 'hu-pgp.sqlite3.gz'.  The database can also be explored in the browser.  By hitting the 'examples' tab on the left and selecting the 'uploaded_data' entry, you can explore participants uploaded data.  For example, the following query gives results that might have data you're interested in:

select * from uploaded_data where (name like 'LF%' or name like '%exome%')

Some participants have uploaded their 23andMe data but did not label it.  Some of this data can be captured by filtering on names that begin with "LF".

Attached are the results of the above query in the form of CSV files.  The 'download_url' is relative to the 'https://my.pgp-hms.org' site.  For example, a 'download_url' entry of '/user_file/download/671' would translate to 'https://my.pgp-hms.org/user_file/download/671'.

The above query does not necessarily represent a complete list of all exome data available through the Harvard PGP site.  Since participants are able to upload data it is difficult for us to definitively determine which of the uploaded data represents exome data.  With the database snapshot available you'll be able to explore this data yourself and might be able to pick out other exome data that might have been missed in the above query.

If you have any problems accessing the database snapshot or have any further questions, please let us know.
