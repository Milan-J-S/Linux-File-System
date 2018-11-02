# Linux-File-System

This is a  custom limux file system implemented with the FUSE library.

All functions of the file system including reading files, listing files, writing files, and editing the same are provided.
Directory acccess is supported with nested directories

Persistence of the storage of the file system has been achieved, and the entire directory structure is stored in the root folder

To compile the filesystem
gcc filesys.c -o ssfs `pkg-config fuse --cflags --libs`

To mount the file system
`./ssfs -f [mount point]`            
( mount point is the directory to mount to )

Now open the directory on which it was mounted using a new terminal window or the file browser
