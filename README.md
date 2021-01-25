# Shell Data Processing


### Description: 

In this project we will learn how to 

1. Shell Programming
1. Build a Markdown page in Git
1. Use mapping, sorting, and reducing to find the most common words in a body of text. 

### Useful PowerShell commands

- ```cd``` : Sets the current working directory to the specified location
- ```ls, dir``` : Gets the files and folders in the current directory
- ```ni``` : New Item. Creates new file of the preffered type
- ```mkdir``` : Creates new directory
- ```rm, del``` : Removes/Deletes files and folders
- ```pwd``` : Displays currend working directory
- ```mv, mi``` : Moves item from one directory to another
- ```ps``` : Displays running processes
- ```curl``` : Gets content from a specified webpage
- ```cat``` : Gets the content of a file



### Commands and their uses 

- Get the content of the website in a text file  
```
curl "url" -O text.txt
``` 
                 
```
curl "url" > text.txt
```
- Each line into individual words
``` 
tr ' ' '\12' < text.txt 
```
- Pipe output to sort
```
tr ' ' '\12' < text.txt | sort
```
- Count unique characters
```
tr ' ' '\12' < text.txt | sort | uniq -c
```
- Redirect output to result.txt
``` 
tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt
```

### Commands meaning
- Hint: Arrow up in bash for using previous commands again
- ```sort -n ```:  numberic sort
- ```sort -r``` :  reverse sort
- ```sort -nr``` : numeric and reverse sort
- ```sort uniq``` : unique characters
- ```sort uniq -c``` : count unique characters 
 
