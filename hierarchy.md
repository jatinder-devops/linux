## Hierarchy Structure:
The linux file system structured in a hierarchy manner, starts from the root directory and its represenrted by “/” slash. Beneath the root, directories branch out, creating a tree like structure. Each directory contains files and subdirectories, forming a cohesive and organized framework for storing data.

## “Root directory,” 
the top of the file system hierarchy. All other directories and files are located beneath the root directory and its represented by “/” and should not be confused with the root home directory “/root”.

## bin
/bin contains essential executable programs (commands) that users can run, such as cat, ls, and cp.
These programs are stored as binary/machine-readable files that the computer can execute.

## boot
This directory contains static files required to boot a system. Such as Linux kernel. These files are essential for the system to boot.

## cdrom

## dev
This directory contains device nodes that either represent devices that are attached to the system or virtual devices provided by the kernel. 

## etc
This is where you will find configuration files. Configuration files control how the operating system or applications behave.

## home
/home contains the personal directories of users, where each user can keep their own files and data.
For example, users can store documents, pictures, music, videos, and other personal files there.

## lib
The /lib directory contains libraries needed by essential binaries in the /bin and /sbin folder.

## lib64

## lost+found

## media
Media directory is a mount point for removable devices (eg. USB drives, external hard disks).

## mnt
The mnt directory is where the system administrators mount temporary files systems
 
## opt

## proc
Contains special files that prevent system and process information . It represents system and process information. 

## root
This is the home directory of the root user. /root directory content is only accessed by the root user 

## run
This directory gives applications a standard place to store Run-time variable data
## sbin

## snap

## srv
This directory is often used for data related to services running on the system.

## swap.img

## sys

## tmp 
Temporary files are stored in /tmp.
Most linux distros clear tmp at boot time.
So if you store files in /tmp and you reboot your server , you will loose these files. 

## usr

User-related programs, libraries, and documentation are stored in /usr.
It is a large directory containing subdirectories like /usr/bin, /usr/lib, and /usr/share.

## var
stores data that changes frequently, such as log files, temporary data, and spool files.
It is commonly used by the Linux system and applications to store regularly updated information.
