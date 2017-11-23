
## PANDAS
### shuffle  DF
```python
df.sample(frac=1)
```
### renaming columns
```python
df = df.rename(columns={oldName1: newName1, oldName2: newName2})
```
### different groupby on columns
 ```python
f = {'Field1':'sum','Field2':['max','mean']}
grouped = df.groupby('mykey').agg(f)
```
### multi-index loc
 ```python
df.xs('index_value', level='index_name', axis=1)
```
### *ELEGANT* - Getting the Row which has the max value in groups with no groupby
 ```python
df.sort_values('value_col', ascending=False).drop_duplicates(id_col)
```

## NUMPY & NUMERIC PACKS
### sample from list or array
```python
random.sample(xrange(len(mylist)), sample_size)
```
### sparse groupby 
```python
# X is the matrix to gorupby
for idx, group_values in itertools.groupby(enumerate(X), key = lambda x: group_key[x[0]]):
	gb_sparse = coo_matrix(groupby_func([matrow[1] for matrow in group_values], axis = 0))
```


## TEXT
### remove no-arabic chars from string
```python
re.findall(r`[\u0600-\u06FF]+`, my_string)
```
### translate/map characters to other characters (abcd->ABCD)
```python
str.translate(str.maketrans('abcd','ABCD'))
```

## MISC
### unpacking operator *
in this example we turn a list of sets to 1 giant set in a very efficient way using the unpacking operator *
```python
foo = set()
foo.union(*list_of_sets) # == foo.union(list_of_sets[0],list_of_sets[1],...)
```
