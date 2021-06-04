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
  
  
  Administrative Priviledges- This means the user is the creater of the directory. He/she is the root user, therefore has many administrative priviledges.
  3--- Su command:This command creates a new shell. The shell is simple Input console to write commands. By default if user account is not specified , the su command will open shell as the root user, therefore will give adminitrative previlidges.
  How to login to new shell?
  use any of the three
  1. su -
  2. su - l
  3. su -- login.
  
  To logout : 'exit' command is used to logout out from the shell.
  
  4--- sudo command- Allows the user to execute a command without creating a new shell. Syntax sudo [command]
  
  
  Permission- It describes which user is authorized to access a file and for how much time.
  
  There are three types of permission-
  Permission              Effect on file                  
  
  read(r)                 Allows to read or copy file    
  write(w)                Allows to modify or override
  execute(x)              Allows for a file to run as a process
  
  
  Changing file Permission: There are two techniquie to change the permission :symbolic and octal.
  symboli:To change one set of permission.
  octal:To change multiple permission
  
  5---chmod- Change the mode of access .Syntax : chmod [<SET><ACTION><PERMISSIONS>]...FILE
 <SET>-----> u: user, g: group, o: others, a: all 
  <ACTION>-----> +: add permission, =: specify exact permission, -: remove the permission
   <PERMISSION>----> read:r, write:w, execute:x
    
    eg: We have to add execute permission to the user in the file hello.sh
    chmod u+x hello.sh
    
   6----Changing file ownership-The chown command is used to change the ownership of the files and directories
    Syntax: chown[options][owner]  FILE
    eg: sudo chown root hello.sh
  
  Viewing Files
  7----Cat-This command is used to view all the details of small files.
  SYSNTAX- cat [options] [file
  
  Limitations of cat command- used only for small file. If it is udes for big file then it can result long list of details.
    
    8---head-This command is used to view details from the top of the file.
      SYNTAX- head [option][file]
    
    9---tail-This command is used to view details from the bottom of the file.
       SYNTAX- tail [option] [file]
    
    -n option- With head and tail command we can display the amout of lines to display.
    eg- head -n 5 file, this means that it will display the detail of 1st 5 lines from the top of file.
    
    Copying File- 1. To have the original document secured .
                  2. Act as a template for new files.
    10---cp -This command is used to copy the file.
    SYNTAX- cp [options] source destination
    source- the file to be copied.
    destination-Where the file is to be copied.
    eg- cp /etc/passwd .
    . specifies the current directory.
  
  
                                    


