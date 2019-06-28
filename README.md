# bash_tutorial
search in a directory or hole computer using grep
-------------------------------------------------
```
grep -rnw -e 'search_text'
```
How to change file creaion/modified time using touch
----------------------------------------------------
```
sudo touch -t 201809150200 CM_dump_NM-LEM01_201807310200.csv
```
allows a user to set certain attributes of a file residing on a Linux file system.
----------------------------------------------------------------------------------
```
chattr -i 001_SP1708/
```

Get file created/creation time?
---------------------------------
The stat command may output this - (dash). I guess it depends on the filesystem you are using. stat calls it the "Birth time". On my ext4 fs it is empty, though.

%w Time of file birth, human-readable; - if unknown

%W Time of file birth, seconds since Epoch; 0 if unknown

```
stat foo.txt
  File: `foo.txt'
  Size: 239             Blocks: 8          IO Block: 4096   regular file
Device: 900h/2304d      Inode: 121037111   Links: 1
Access: (0644/-rw-r--r--)  Uid: ( 1000/  adrian)   Gid: (  100/   users)
Access: 2011-10-26 13:57:15.000000000 -0600
Modify: 2011-10-26 13:57:15.000000000 -0600
Change: 2011-10-26 13:57:15.000000000 -0600
 Birth: -
```
All directory size
-----------------------------
```
du -h --max-depth=1
```


-bash bad interpreter: No such file or directory
----------------------------------------

vi /path/to/scriptfile

When file is opened, change the format of the script to the right one by entering
: set fileformat=unix

or just simply

: set ff=unix

Finally, save the script for the new format taking effect and exit the vi program by entering
: x
