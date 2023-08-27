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
sqlite> 
```
