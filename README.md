# FileUtils
![projectstage](https://img.shields.io/badge/project%20stage-alpha-yellow)
![projectstage](https://img.shields.io/badge/version-1.0-yellow)
[![license](https://img.shields.io/github/license/PentagonLP/fileutils)](https://github.com/PentagonLP/fileutils/blob/main/LICENSE)
[![issues](https://img.shields.io/github/issues/PentagonLP/fileutils)](https://github.com/PentagonLP/fileutils/issues)<br>
[![contributors](https://img.shields.io/github/contributors/PentagonLP/fileutils)](https://github.com/PentagonLP/fileutils/graphs/contributors)
[![activity](https://img.shields.io/github/commit-activity/m/PentagonLP/fileutils)](https://github.com/PentagonLP/fileutils/commits/main)
[![lastcommit](https://img.shields.io/github/last-commit/PentagonLP/fileutils)](https://github.com/PentagonLP/fileutils/commits/main)<br>
![size](https://img.shields.io/github/languages/code-size/PentagonLP/fileutils)
![files](https://img.shields.io/github/directory-file-count/PentagonLP/fileutils)
![languages](https://img.shields.io/github/languages/count/PentagonLP/fileutils)<br>

Library for the Minecraft mod **ComputerCraft/CC: Tweaked** for better interaction with files  

## How to install 
FileUtils can be installed using the [ComputerCraft Package Tool](https://github.com/PentagonLP/ccpt) by using the following commands:

Install CCPT, only run if you havn't installed it yet:
```
pastebin run syAUmLaF
```
Install the library:
```
ccpt install fileutils
```
The library will now be stored in "/lib/fileutils".

## How to use

### **1. Check if file exists**  
The function **file_exists([filepath])** returns true if the file exists or false if it doesn't.

*Example:*  
Content of *"test"*:
```
hi, how are you?
```
Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/file_exists.png"
/><br>  

### **2. Store some content in a file**  
The function **storeFile([filepath],[content])** stores [content], given as a string, in a file specified by the given [filepath]. This will overwrite the file if it already exists!

*Example:*  
Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/storeFile.png"
/><br> 
Content of *"test"*:
```
hi, how are you?
```

### **3. Read some content from a file**  
The function **readFile([filepath],[createnew])** reads a file specified by the given [filepath]. If [createnew] is nil and the file doesn't exist, false is returned. If [createnew] is some string and the file doesn't exist, a new file with the content [createnew] is created and [createnew] is returned. This is useful if you don't know wether the file was already created, and if not some basic file structure should be built.

*Examples:*<br>1) Content of *"test"*:
```
hi, how are you?
```
Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/readFileFalseExists.png"
/><br> 
2) *"test"* does not exist.

Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/readFileFalseMissing.png"
/><br> 
3) *"test"* does not exist.

Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/readFileTrueMissing.png"
/><br> 
Content of *"test"*:
```
:)
```

### **4. Store a table in a file**  
The function **storeData([filepath],[content])** stores [content], given as a table, in a file specified by the given [filepath]. This will overwrite the file if it already exists!

*Example:*  
Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/storeData.png"
/><br> 
Content of *"test"*:
```lua
{  greeting = "'ello",}
```
### **3. Read a table from a file**  
The function **readFile([filepath],[createnew])** reads a file specified by the given [filepath] as a table. If [createnew] is false and the file doesn't exist, false is returned. If [createnew] is true and the file doesn't exist, a new file with the content "{}" is created and an empty table is returned.

*Examples:*<br>1) Content of *"test"*:
```lua
{  greeting = "'ello",}
```
Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/readDataFalseExists.png"
/><br> 
2) *"test"* does not exist.

Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/readDataFalseMissing.png"
/><br> 
3) *"test"* does not exist.

Example code and output:
<br><img
    alt="missing image :("
    src="https://raw.githubusercontent.com/PentagonLP/fileutils/main/img/readDataTrueMissing.png"
/><br> 
Content of *"test"*:
```
{}
```

## Changelog
Nothing here yet, we are still on 1.0 :)

## Last words
First of all, thanks for reading! This library is not the biggest library ever, but it turned out to be really useful for one of my projects, and maybe it is for yours too :)  
If you find bugs, please create an issue so I can fix them.  
I'm still very new to Github, so feel free to point out things I could do better. Also, english is not my first language, so if you find any spelling/language-related mistakes, please do also create an issue.  
Have a nice day,  
PentagonLP
