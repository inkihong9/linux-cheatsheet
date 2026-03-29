# permissions in linux
* **read** 
  * (file) read file contents
  * (directoriy) read all contents in the directory including both files and subdirectories
* **write**
  * (file) make modifications to the file
  * (directory) create, update or delete files in the directory
* execute
  * (file) execute file if it's a program or script
  * (directory) enter the directory and access its files
## file permission representation `drwxrwxrwx`
* `d` indicates a directory, if it's a regular file, this character would be `-` instead
* `rwx` means read, write and execute. If any of those permissions are not granted, then they would be `-` instead
  * 1st set of `rwx` belongs to **user**
  * 2nd set of `rwx` belongs to **group**
  * and 3rd set belongs to **other**

# types of owners
* **users:** the owner of the file/directory
* **group:** a larger group that the owner is part of
* **other:** all other users on the system