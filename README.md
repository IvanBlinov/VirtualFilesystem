# VirtualFilesystem
Virtual Filesystem written using Scala

Support such methods: 

`mkdir <dir_name>` - create a dir with <dir_name>

`cd <path> ` - navigate to <path> inside of virtual filesystem <br>
Support **absolute** and **relative** paths: <br>
-`cd /dir1/dir2` - navigate to root dir `dir1` and then to `dir2` <br>
-`cd dir1/dir2` - navigate to relative to current directory `dir1` and then to `dir2`
    
`touch <filename>` - create a file with name `<filename>`

`ls` - shows all files and dirs inside of current directory 

`pwd` - shows current path in filesystem

`rm <name>` - remove file or directory with name `name` <br>
Support name with absolute path, e.g.: <br>
`rm /dir1/dir2/filename` - remove file with name `filename` inside of root dir `dir1` and `dir2` <br>
`rm dir3` - remove directory with name `dir3` with all files and dirs inside  

`echo <something>` - print `something` <br>
Can be used to write some data to file, e.g: <br>
`echo Hello World > filename` - will write `Hello World` to file `filename` if such exists **with** overwriting all data inside of file <br>
`echo Hello World >> filename` - will append `Hello World` to file `filename` if such exists **without** overwriting all data inside of file <br>

`cat <filename>` - print all data inside of file with name `filename`
