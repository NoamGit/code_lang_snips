
## INSER ROW
### insert blob value
```sql
insert into ... VALUE (..., utl_raw.cast_to_raw('mystring'),...)
```

## CREATE TABLE
### enum column type
```sql
col_name varchar(10) default 'def_value' not null check( col_name in ('enum_val_1','enum_val_2','enum_val_3' ))
```

## CAST
### blob to str
```sql
select utl_raw.cast_to_varchar2(dbms_lob.substr(BLOB_FIELD)) from TABLE_WITH_BLOB where ID = '<row id>';
```

## TABLE OPERATIONS
### concat text in cols
```sql
CONCAT(COL_NAME1, COL_NAME2)
```

### MISC

