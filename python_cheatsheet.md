
## PANDAS
### shuffle  DF
```python
df.sample(frac=1)
```
### renaming columns
```python
df = df.rename(columns={oldName1: newName1, oldName2: newName2})
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