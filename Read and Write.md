# Read and write file
While using Python you may come across situations where you need to read data from a text file or write your results into a file etc. It is very easy to do this in Python. There are many ways of doing it. We can open a text file using Python and can read data from it or pass it to some variable. Otherwise the file can be opened outside Python using its default program. Depending on the context we can do in either way.

A text file can be opened in Python by using its built-in functions - open() and readlines(). 

To read a text file, first we need to open the file by giving its path. 

Here the pointer to the text file is stored to the variable f. The second attribute in parentheses gives the path of the file that you are going to open. Here ‘r’ stands for “read” mode of the file. There are other modes such as:

w - overwrite to a file (if such file does not exist, then create and write)
a - append to a file
rb - read binary
wb - overwrite a binary file 
r+ - open the file for both reading and writing
a+ - open the file for both appending and reading.

The following snippet illustrates how to create and write in a text file using Python

```python
text = open("file.txt", "w") 
l1= "This is my notepad file written using Python" 
text.writelines(l1) 
text.close()
```

There is a simple way in Python to open a program. Let us see an example for opening an executable file outside Python. Write the following code and run in Python.

```python
import os os.startfile('C:\Program Files\Google\Google Talk\googletalk.exe')
```

This facility ensures seamless integration of Python programs with operating system utilities and applications.

Excel files are the common data storing file format. We can read and write excel files using Python script. A package to support this task (xlrd package) needs to be installed. You can download the package and install or use easy installer for windows and Linux users can use the terminal for this (sudo apt-get install python- xlrd)

If you are done with the xlrd package, try the following: 

```python
import xlrd 
wb = xlsxrd.open_workbook('data.xls')
```

Now let us write an excel file. For this xlwt module has to be installed. This can be done by following the instructions that has been given above. Then follow the codes given below.

```python
import xlwt book = xlwt.Workbook(encoding="utf-8") 
sheet1 = book.add_sheet("New Sheet 1")  
sheet2 = book.add_sheet("New Sheet 2")  
sheet1.write(0, 0, "I have written first Cell of the First Sheet") 
sheet1.write(1, 0, "I have written in the second Cell of the First Sheet") 
sheet2.write(0, 0, "I have written in the First Cell of the Second Sheet")  
sheet2.write(1, 10, "This is written to eleventh Cell of the Second Sheet")  
book.save("New_Excel.xls")
```

Here book.add_sheet is the syntax for adding new sheet. sheet1.write followed by the cell id and text writes the text  in the specified cell. 

