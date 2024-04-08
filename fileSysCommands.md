# `cd` command
1. Using `cd` with no arguments
```
jackiezhong@Jackies-MBP ~ % pwd
/Users/jackiezhong
jackiezhong@Jackies-MBP ~ % cd 
jackiezhong@Jackies-MBP ~ %

```
When you use `cd` with no arguments, it doesn't invoke any changes in directory because no argument was passed. Thus, you remain in the same directory.

2. Using `cd` with path to a directory as argument
```
jackiezhong@Jackies-MBP / % pwd
/
jackiezhong@Jackies-MBP / % cd Users/jackiezhong/cse15l_lab0/cse15l_extras
jackiezhong@Jackies-MBP cse15l_extras %

```
Here, I'm starting at the root directory, which is why `pwd` prints `/` as my directory. Providing a path to the cse15l_extras directory, `cd` places me in that directory. 

3. Using `cd` with a path to a file as argument
```
jackiezhong@Jackies-MBP ~ % pwd
/Users/jackiezhong
jackiezhong@Jackies-MBP ~ % cd cse15l_lab0/lab0.txt
cd: not a directory: cse15l_lab0/lab0.txt
jackiezhong@Jackies-MBP ~ %
```
We're getting this error because `cd` is only meant to change directories to allow us to look into different directories. If we wanted to look into a file, we would need to use a different command.


# `ls` command
1. Using `ls` with no arguments
```
jackiezhong@Jackies-MBP ~ % pwd
/Users/jackiezhong
jackiezhong@Jackies-MBP ~ % ls
Applications    Downloads    Music      cse15l_lab0
Library         Pictures     Projects   Desktop
```

Using `ls` with no arguments list us directories and files nested within the directory we're currently in. 

2. Using `ls` with path to a directory as argument
```

jackiezhong@Jackies-MBP / % pwd
/
jackiezhong@Jackies-MBP / % ls /Users/jackiezhong/cse15l_lab0
cse15l_extras lab0.txt
jackiezhong@Jackies-MBP / %

```
Using `ls` in this way prints the contents within that directory.

3. Using `ls` with a path to a file as argument
```
jackiezhong@Jackies-MBP / % pwd
/
jackiezhong@Jackies-MBP / % ls /Users/jackiezhong/cse15l_lab0/lab0.txt
/Users/jackiezhong/cse15l_lab0/lab0.txt
jackiezhong@Jackies-MBP / %
```
Using `ls` in this way just prints out the file path that you used as argument. The command is supposed to be used on directories only, to list files and directories nested within 
the directory you're in.



`cat` command
1. Using `cat` with no arguments
```
jackiezhong@Jackies-MBP ~ % pwd
/Users/jackiezhong
jackiezhong@Jackies-MBP ~ % cat
hello
hello
```
Using `cat` without arguments just allows you to type in inputs and upon enter, your input is printed again on the terminal. 

2. Using `cat` with path to a directory as argument
```
jackiezhong@Jackies-MBP ~ % pwd
/Users/jackiezhong
jackiezhong@Jackies-MBP ~ % cat cse15l_lab0
cat: cse15l_lab0: Is a directory
```
The command's purpose is to print out contents of a file, which is why when supplied a directory as the argument, it gives us the error that the argument is a directory.


3. Using `cat` with a path to a file as argument
```
jackiezhong@Jackies-MBP ~ % pwd
/Users/jackiezhong
jackiezhong@Jackies-MBP ~ % cat cse15l_lab0/lab0.txt
hello cse15l, this is my lab 0 file
jackiezhong@Jackies-MBP ~ %

```   
By specifying a file path, `cat` prints out the contents of that file onto the terminal.







   
