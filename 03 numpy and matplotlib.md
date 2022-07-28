# Numpy

First install Numpy into your Python environment and load it 


## For Linux/ Ubuntu 
```python
sudo apt-get install python-numpy
```
## For Windows 
Use PIP installer
```python
pip install numpy
```

Numpy can be imported in Python interface by typing the command 
```python
from numpy import *    # or use
import numpy as np
```
Once you import the package in to the Python environment, it is ready to use. Ready, Steady, Go!!!

```python
import numpy as np 
A= np.array ([[78, 41, 53], [65, 86, 49], [94, 49, 56]])
```

Like most modern programming languages, indexing starts from 0. The element 78 is referred to as A[0,0]. Type the following:

```python
A[0]   # first row  
A[-1]  # last row 
A[0,0] # first row, first column 
A[0,1] # first row, second column 
A[:2] # first two rows  
A[:,1] # second column
```

To create an array with elements in the range 0–99, the following code can be used. 

```python
import numpy as np		
x =np.array(range(100))
```

Here is another Python magic, if you would like to convert the array created just now into three 4x2 matrices, you can simply use the following command:

```python
x.reshape((4,5,5)) 
```

To define matrices consisting only of zeroes or ones, or an identity matrix, try the following:

```python
np.zeros((2,4)) 
```
Identity Matrix

```python
np.identity(3)
```

If you wish to create a matrix with a dimension same as that of another matrix, but containing elements as only zeroes, or only ones, it is very easy in Python! Try the following:

```python
np.ones_like(A)
```

To split an array with elements 0 to 19 into three, try the following command:
```python
x =array(range(20))
split=array_split(x, 3)
```
Easy way to define a matrix
```python
B=np.mat('23,24;25,26')
print(B)

```
Eigen values and vectors 
```python
from numpy import linalg as LA
M=np.mat('5,0,0;1,2,1;1,1,2')
eigval,eigvect=LA.eig(A) 
print(eigval)			# Eigen values of matrix M
print(eigvect)			# Eigen vector of matrix M
```



A polynomial can be represented by
```python
eq=np.poly1d([1,-5,6])
print(eq)
print(np.roots(eq))
```
Derivative and integrals
```python
print(eq.deriv())	  # derivative of eq	
print(eq.integ(k=4))    #integral of eq with constant of integration 4
```
The statistical tool box consists of statistical functions. The data from a Numpy array or in the word file can be imported into python and we can find mean, median, variance, correlation etc

Have a look at some of the examples
```python
x=np.arange(-10.,10.,1)	
print(np.mean(x))				# mean 
print(np.var(x))				# variance 
print(np.amin(x))				# minimum value in observation 
print(np.amax(x))				# maximum value in observation 
print(np.std(x))				# standard deviation of observation
```


# Matplotlib
Matplotlib is an object-oriented plotting library for python. It is a MATLAB/Scilab-like application programming interface (API) and provides accurate high-quality figures, which can be used for publication purposes. 
matplotlib contains pylab interface, which is the set of functions provided by matplotlib.pylab to plot graph. matplotlib. pyplot is a collection of command-style functions that helps matplotlib to work like MATLAB.

Let us install Matplotlib
```python
pip install matplotlib
```

To start a plotting experiment, first we need to import matplotlib.pylab

```python
import matplotlib.pyplot as plt
```

Here library - matplotlib.pyplot - is imported and labeled as plt for easy future reference of the module.

```python
import matplotlib.pyplot as plt
plt.plot([ 1 , 2, 3 ,4 ], [ 4 ,3 , 2, 1 ]) 
plt.axis([ 0 , 5 , 0 , 5]) 
plt.show()
```

The plot function accepts the plotting points as two arrays with x, y coordinate respectively. Pyplot fits a straight line to the points. If you need only a scatter diagram of the points try the following code.

```python
plt.plot([ 1 , 2, 3 ,4 ], [ 4 ,3 , 2, 1 ], 'ro')
```

You can plot the graph using different colors and styles by putting an argument after the plot function.

```python
import matplotlib.pyplot as plt
import numpy as np 
x=np.arange(1.,10.,0.1) 
y=x*x 
plt.plot(x,y,'g--')
```

After plotting the graph, to view it, you need to type show()command. 

Here you will get a green line graph; try with r for red, y for yellow etc. We can specify shapes with cryptic reference such as  S for square, ^ for triangle etc.

```python
plot(x,y,'rs')		# Red square 
plot(x,y,'g^')		# Green triangle
```

Standard mathematical function can also be plotted. Let us plot sine curve.

```python
import matplotlib.pyplot as plt
import numpy as np 

x = np.arange(0.,10.,0.1)	                # to define x values 
y = np.sin(x)				# function definition 
plt.plot(x,y)				# to plot 
plt.grid(True)				# to show graph in grid 

```
