
## INSER ROW
### insert blob value
```sql
insert into ... VALUE (..., utl_raw.cast_to_raw('mystring'),...)
```

### CREATE TABLE
## enum column type
```sql
col_name varchar(10) default 'def_value' not null check( col_name in ('enum_val_1','enum_val_2','enum_val_3' ))
```

### UNREGISTERED
