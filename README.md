# A FUSE Filesystem
FUSE is an interface that allows us to call our own functions instead of using the default kernel functions when a system call is used. Using it, we have implemented the following functionalities: 
- Create and remove a directory.
- Create, read and write to a file.
- Delete a file.
- Append to and truncate a file.
- Access, modified and status change time updates.
- Open and close a file

## Usage:
1. ```cd``` into the directory and create a mount point:
```
cd FUSE-filesystem
mkdir mountpoint
```
2. Compile and run the code:
```
$ gcc FUSE-filesystem.c -o FUSE-filesystem `pkg-config fuse --cflags --libs`
$ ./ FUSE-filsystem - f path/ to/ mountpoint
```
3. Change your working directory to ```mountpoint``` and use your custom-made filesystem!
