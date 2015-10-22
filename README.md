write_rmm_db.py
===============

Generate and populate a SQL database with RMM index data obtained from a daily text file.

Installation
------------

```
git clone <this project>
```

Usage
-----
The text file, rmmBom.txt, is passed into write_rmm_db.py, which converts each
column into a Python list, and zips the lists together. The sqlite3 Python
library is then utilized to build a table, 'rmm', in the datbase 'rmm_index.db',
and the zipped list is inserted into the table.
