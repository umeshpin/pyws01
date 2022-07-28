# Pandas
Pandas is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.

## Import first
```python
import pandas as pd 
```

### Create Your own Data Frame
```python
classes = pd.Series(["Mathematics","Chemistry","Physics","History","Geography","Hindi"])
grades  = pd.Series([90,54,77,22,25])
pd.DataFrame({"Classes": classes, "Grades": grades})
```

# working with columns 
```python
pd.DataFrame({'Yes': [50, 21], 'No': [131, 2]})
```

# Series
Simple way to create a data
```Python
pd.Series([1, 2, 3, 4, 5])
```
One-dimensional ndarray with axis labels (including time series).

Labels need not be unique but must be a hashable type. The object supports both integer- and label-based indexing and provides a host of methods for performing operations involving the index. Statistical methods from ndarray have been overridden to automatically exclude missing data (currently represented as NaN).

> :warning:  Tip: To create random values 
```python
np.random.randn(5, 3)
```
To read more : https://numpy.org/doc/1.16/reference/routines.random.html


```python
import numpy as np
s = pd.Series(['Lal', 'Mammooty', 'DK', 'Fahad', np.nan, '1234','Manju'])
```

# Operationns on data file 
We can ask questions to the data
```python
print(s.str.upper())
```
```python
print(s.str.replace('1234','Parvathi'))
```
```python
print(s.str. startswith ('y'))
```
```python
print(s.str. endswith ('y'))
```
```python
print(s.str.upper())
```
## To deal with Multiple Column
Lets Try an Example
```python
import pandas as pd
import numpy as np

df = pd.DataFrame(np.random.randn(5, 3),
index = ['a','b','c','d','e'], columns = ['A', 'B', 'C'])

# Select all rows for multiple columns, say list[]
print(df.loc[:,['A','C']])
```
Also Try
```python
print(df.loc['a':'c'])
```
```python
print(df.iloc[[1, 3], [1, 2]])
```

### Lets Create a new dataframe 
```python
classes = pd.Series(["Mathematics","Chemistry","Physics","History","Geography","Hindi"])
grades  = pd.Series([90,54,77,22,25])
pd.DataFrame({"Classes": classes, "Grades": grades})
```
# Google Drive and Colab :tada: :tada: :tada:

```python
from google.colab import drive
drive.mount('/content/drive')
```
## Upload files to workspace 
for a sample data downlaod the file  https://drive.google.com/file/d/1iWO_FJ_C-olnpmj4Z-nNtLnWOjyQop3r/view?usp=sharing

```python
from google.colab import files
uploaded = files.upload()
```

Read files and head it 
```python
import pandas as pd
df=pd.read_csv("data_neet.csv")
df.head(4)
```
```python
df.shape
```

```python
print(df.columns)
```
```python
print(df["Student"])
```

### Another way
```python
%cd /content/drive/My Drive/Data_FDP/
df=pd.read_csv("data_neet.csv")
df.head(4)
```

## Writing Files from Pandas
```python
Lines = ["This is line A\n", "This is line B\n", "This is line C\n"]
Lines
```
Now lets write
```python
with open('Example2.txt', 'w') as writefile:
    for line in Lines:
        print(line)
        writefile.write(line)
```
Or More specifically to some drive locations 
```python
with open('/content/drive/My Drive/Data_FDP/file.txt', 'w') as f:
  f.write('content')
```
