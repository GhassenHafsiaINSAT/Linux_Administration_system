## What is Shell?
- Shell is a command-line interface will enable you effectively work on your linux machine
- While the graphial interface may be apealing to the user, it may be quite limited in the level of functionality
- Shell is a text-based program to interact with the operating system

## The Home directory 
- The default directory you will find yourself in when opening a linux machine
- It is represented by ~

## Command types 
- Commands in Linux can be generally categorized into two types:
  - **Internal or Built in commands**: like echo, cd, pwd, e.t.c, are part of shell itself 
  - **External commands**: like mv, date, uptime, cp e.t.c, are binary programs located in destinct files, usually installed by the package manager
## Viewing file size
- `DU` to inspect the size of file
- `-sh` prints the size if file in human readable format

## Archiving files 
- `tar` is used to group multiple files or directories into a single file, archiving data
- **`tar` options**
  - `-c` is used to create archive
  - `-f` is used to specify the name of the tar file to be created  
  - `-t` is used to see the content of the tarball
  - `-x` is used to extract the contents from the tarball
  - `-z` is used to compress the tarball to reduce its size
## Compression 
- **bzip2** : adds `.bz2` to the compressed file
- **gzip** adds `.gz` to the compressed file
- **`gz`** adds `.xz` to the compressed file
- You can uncompress these compressed files using respectively `bunzip2`, `gunzip` and `unxz`

## Searching for files and directories 
- Before using locate you should update the database mlocate.db 
- ```sh
  sudo updatedb 
  locate EXAMPLE.cpp
  /Path/To/Your/EXAMPLE.cpp
  ```

- ```sh
  find /home/ghassen -name Example.cpp
  ```

- Search for a workd in file use the command `grep`, it will only print out the line matching the search pattern
```sh
grep main example.cpp
```
- When you dont know which file in directory use the `-r` to search recursively 
- When you want to print out the lines that does not contain the word, use the option `-v`

## IO redirection 
  
