# learning-LINUX
INTRODUCTION TO LINUX:
'LINUX IS EVERYWHERE'. Let us define in a traditional way, Linux is an operating System and by operating system I mean that a software that caries out all the functionality like file management, process management , device management etc.
From automobiles to rockets, televisions to watches, linux has gained many users.Linux is now being used everywhere like in servers, IOT devices, networking equipments etc.

WHY USE LINUX ?
We use windows operating system, and it is preffered by many of us because of its GUI, i.e. we can open any software by just a click.
Then why use Linux?
we use Linux because of the CLI(Command Line Interface), we write cammand and then actions is performed. The commands gives us the better understanding of what the system is doing at any particular moment.

Linux has many commands, we'll be learning many of them.

Before learning about the commands, let's see what is options and arguments.
-- Options: This is used to alter the behaviour of the command.
-- Arguments: These are the items or the values upon which the command acts.

BASIC SYNTAX OF COMMAND:
command [options] [arguments]

1--- cd command: change directory command cd is used to change the current directory. syntax: cd [options] [path]

eg: cd / (moves to the root directory)

Path: Path specifies the location of the file. These are of 2 types:
1- Absolute Path- Starts from the root of file system..
2- Relative Path- Starts from current location.

2--- ls command: listing of files ls command is used to list the content of directory. Syntax: [options] [file]

-l option: This option gets the details of the file like the file type,permission,ownership,timestamp..Syntax:-l ls

Now, let us understand what is file type, how to find the file type

File type- The first character points the type of file.

d         directory                  A file used to store other file.
-         regular file               Includes relatable files like image files, binary files.
l         symbolic link              Points to other file.
s         socket                     Allow for communication between process.
p         pipe                       Allow for communication between process.
b         block file                 Used to communicate with hardware.
c         character file             Used to communicate with hardware.

lets consider the details of a file, d  rwxr-xr-x 2 root root 4096 April 11 2014 upstart
 d - directory
 rwxr-xr-x- permission
  2- hard link count
  root- user 
  root- group
  4096-file size
  April 11 2014- file size
  upstart- directory name.
  
  **NOTE**-lt will sort file by timestamp
  ls will sort file by filesize
  tr will reverse the order of file
  r will sort inreverse alphabetical order.
  
                                    


