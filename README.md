# CATV
Some useful CATV related items

## catv.db
A sqlite database containing the video EIA and center frequencies

```
% sqlite3 catv.db
SQLite version 3.39.5 2022-10-14 20:58:05
Enter ".help" for usage hints.
sqlite> .schema
CREATE TABLE eia (id NUMERIC, eia NUMERIC, center_freq_mhz NUMERIC);

sqlite> select * from eia limit 5;
id|eia|center_freq_mhz
1|2|57
2|3|63
3|4|69
4|5|79
5|6|85
sqlite> 
```

## sources.dat
A simple two column file of TiVo iGuide.source_id(s) and source_name(s).  I read in this file for some scripts and it has been useful over the years. Especially for a script that cannot get to a database.
