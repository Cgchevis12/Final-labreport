**In the lab report 3, I've choosen 'find' command. For lab report 5, I'm going to choose command 'grep'.**

Here are four interesting command-line options or alternate ways to use grep:

1. -r or --recursive: This option searches recursively through all files and directories within a specified directory.

```
grep -r "example" ./written_2

```
 This command searches for the string "example" in all files and directories under the ./written_2 directory recursively.
 
 
 2.-n or --line-number: This option displays the line numbers of the matched lines.

```
grep -n "example" ./written_2/file1.txt
```
This command searches for the string "example" in the file1.txt file under the ./written_2 directory and displays the line numbers of the matched lines.

3.-i or --ignore-case: This option performs a case-insensitive search.

```
grep -i "EXAMPLE" ./written_2/file2.txt
```
This command searches for the string "EXAMPLE" in the file2.txt file under the ./written_2 directory, regardless of case sensitivity.

4. -v or --invert-match: This option displays lines that do not match the search string.

```
grep -v "example" ./written_2/file1.txt

```
This command displays all lines in the file1.txt file under the ./written_2 directory that do not contain the string "example".

**For further showing the functionality of the 'grep', 8 compelete examples shown below**

Option 1: -i
This option makes the search case-insensitive.

Example 1:
```
$ grep -i 'dog' ./written_2/file1.txt
The quick brown fox jumps over the lazy DOG.
This is another line with dog in it.

```

Example 2: 
```
$ grep -i 'cat' ./written_2/*
./written_2/file2.txt:This line has a cat in it.
./written_2/file3.txt:This is a line with a CAT in it.
./written_2/file3.txt:This is another line with a cat in it.

```

Option 2: -v
This option inverts the search and prints all lines that do not match the pattern.

Example 1:
```
$ grep -v 'fox' ./written_2/file1.txt
This is a line without any keyword.
The quick brown jumps over the lazy dog.
This is another line with dog in it.

```

Example 2:
```
$ grep -v -r 'file1' ./written_2/
./written_2/file2.txt:This line has a cat in it.
./written_2/file3.txt:This is a line with a CAT in it.
./written_2/file3.txt:This is another line with a cat in it.

```

Option 3: -n
This option shows the line number of the matched pattern.

Example 1:
```
$ grep -n 'brown' ./written_2/file1.txt
2:The quick brown fox jumps over the lazy dog.

```

Example 2:
```
$ grep -n -r 'line' ./written_2/
./written_2/file1.txt:1:This is a line without any keyword.
./written_2/file1.txt:2:The quick brown fox jumps over the lazy dog.
./written_2/file1.txt:3:This is another line with dog in it.
./written_2/file2.txt:1:This line has a cat in it.
./written_2/file3.txt:1:This is a line with a CAT in it.
./written_2/file3.txt:2:This is another line with a cat in it.

```

Option 4: -w
This option matches the whole word instead of just a substring.

Example 1:
```
$ grep -w 'dog' ./written_2/file1.txt
The quick brown fox jumps over the lazy dog.

```

Example 2: 
```
$ grep -w 'cat' ./written_2/*
./written_2/file2.txt:This line has a cat in it.
```


**Resources from: links provided by ChatGPT 
-https://www.geeksforgeeks.org/grep-command-in-linux-with-examples/
https://www.computerhope.com/unix/ugrep.htm **
