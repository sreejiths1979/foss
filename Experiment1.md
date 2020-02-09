# <center>Experiment 1 </center>
## <center>Getting started with Linux basic commands for directory operations</center>
### Aim:
Getting started with Linux basic commands for directory operations, displaying direc-tory structure in tree format etc.
### Baisc Commands:
<table boarder="3" width="90%">
<tr>
<td width="2%"><center>Command</center></td><td width="6%"><center>Operation</center></td>
</tr>
<tr>
<td >touch file name</td><td>Create an empty file</td>
</tr>
<tr>
<td>mkdir directory name</td><td>Create a directory</td>
</tr>
<tr>
<td>pwd</td><td>Shows the Present Working Directory</td>
</tr>
<tr>
<td>cd directory name</td><td>Change directory</td>
</tr>
<tr>
<td>cat file name</td><td>To view the contents of a file</td>
</tr>
<tr>
<td>more file name</td><td>To view the contents in a single stretch</td>
</tr>
<tr>
<td>less file name</td><td>Similar but faster than more </td>
</tr>
<tr>
<td>ls</td><td>Lists files in a directory </td>
</tr>
<tr>
<td>ls -l</td><td>Provide long listing of all the files </td>
</tr>
<tr>
<td>ls -l ih</td><td>Provides sizes in human readable form </td>
</tr>
<tr>
<td>ls -F</td><td>Mark all executables with * and directories with /m </td>
</tr>
<tr>
<td>ls -a</td><td>Show all files in the present directory with special dot files</td></tr>
<td>cp file1 file2</td><td>Copying files</td></tr>
<td>cp -r dirname1 dirname2</td><td>Copy directories</td></tr>
<td>rm filename</td><td>Remove a file</td></tr>
<td>rmdir -r dirname</td><td>Remove a non empty directory</td></tr>
<td>clear</td><td>Clear the contents of the terminal</td></tr>
<td>locate</td><td>Search for a specified filename</td></tr>
<td>man command name</td><td>View help of the specified command name</td></tr>
<td>chmod [options] mode filename</td><td>Change file permissions</td></tr>
<td>chown [options] filename</td><td>Change file ownership</td></tr>
<td>kill [options] pid</td><td>Kill a process</td></tr>
<td>who [options]</td><td>Display who is logged in</td></tr>
<td>top</td><td>Display the resources being used in your system</td></tr>
<td>ln [options] source [desitination]</td><td>Create a shortcut</td></tr>
<td>tree</td><td>Print the directory structure in tree format</td></tr>
</table>

### Directory Structure:
<table boarder="3" width="90%">
<tr>
<td width="2%"><center>File Name</center></td><td width="6%"><center>Content</center></td>
</tr>
<td>/bin</td><td>Essential user command binaries</td></tr>
<td>/boot</td><td>Static files and boot loader</td></tr>
<td>/dev</td><td>Device files</td></tr>
<td>/etc</td><td>Host specific system configuration</td></tr>
<td>/home</td><td>User home directories</td></tr>
<td>/lib</td><td>Essential shared libraries and kernel modules</td></tr>
<td>/mnt</td><td>Mount point for devices</td></tr>
<td>/opt</td><td>Add on application software packages</td></tr>
<td>/sbin</td><td>System binaries</td></tr>
<td>/tmp</td><td>Temporary files</td></tr>
<td>/usr</td><td>User utilities and applications</td></tr>
<td>/var</td><td>Variable files</td></tr>
<td>/root</td><td>Home directory for the root user</td></tr>

</table>

### Output:
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/Screenshot%20from%202020-02-04%2000-34-35.png)
### Result:
Basic Linux commands and the direcotry structure of linux were studied. The directory structure was printed in tree format using tree command

# <center>Experiment 2 </center>
## <center>LINUX COMMANDS FOR OPERATIONS SUCH AS REDIRECTION, PIPES, FILTERS, JOB CONTROL, CHANGING OWNERSHIP/PERMISSIONS OF FILES/LINKS/DIRECTORY
</center>
### Aim:
Linux commands for operations such as redirection, pipes, filters, job control, changing
ownership/permissions of files/links/directory.
### Overview:
<u>Redirection of standard Input/Output</u>

<li>By default most command line programs send their output to the standard output which by default displays it on the display unit.<br>
commandName > fileName -	Overwrites the file with the output of the command.<br>
commandName >> fileName - 	Appends the file with the output of the command.<br>&nbsp

<li>Most of the command line programs accept its input from the standard input and by default gets its contents from the keyboard. Similar to standard output it can also be redirected.<br>
sort < filename - sort command processes the contents of the file with the name filename.
sort < file1 > file2 processes the contents of file 1 and redirects its output to file 2.<br>
<u>Pipes</u>
<br><li>
Pipes are used to redirect the standard output of one command to the standard input of another command.
command1 | command2 the standard output of command 1 is redirected to the standard input of command 2.

<u>Filters:</u> Filters take the standard input and perform an operation upon it and sends the results to the standard output. This can be used to process information in powerful ways.

<li>sort - sorts the standard input and sends the output to standard output.
<br>‘sort filename’ rearranges each line of file in alphabetical order and outputs it to the standard output.
<li>uniq - Given a sorted stream of data from standard input it removes the duplicate lines of data and returns the result to the standard output.
<li>grep - examines each line of data it receives from standard input and outputs all lines that contains a specific pattern of characters.<br>
‘grep “string” new.txt’ outputs lines of text in new.txt which contain the word string.<br>

<li>fmt - reads text from standard input and outputs formatted text to standard output.<br>
‘fmt filename’ formats contents of filename and outputs it in standard output.<br>
<li>pr - Takes data from the standard input and splits the data into pages with page breaks, footers and headers in preparation for printing.<br>
‘pr filename’ displays the contents of the file one page after the other and returns the output to the standard output.<br>
<li>head - Outputs the first few lines of the file and returns it to the standard output.
<li>tail - Outputs the last few lines of the file and returns it to the standard output.
<li>tr - Translates Characters. Can be used to perform tasks such as uppercase to lowercase conversions or changing the line termination characters from one type to another.
<br>‘tr [:lower:] [:upper:]’ takes input from the keyboard and outputs each character of the input to uppercase characters and outputs it to the standard output.

<u>Job Control</u><br>
There are several commands used to control processes in Linux.
<li>ps - The ps commands lists the processes running in the system.<br>
‘ps lists’ all processes running in the system<br>
‘ps aux’ lists all processes running in the system.<br>
<li>kill - sends a signal to the specified processes usually to stop the execution of the
processes.<br>
‘kill -l’ lists the signal names that can be sent to processes in Linux.<br>
‘kill pid’ to kill the processes specified by the process id (pid) which can be obtained by the ps command.<br>
‘kill -s SIGKILL pid’ is used to send SIGKILL signal to process with process id
‘pid’. This command is used to forcefully kill a process without memory cleanup.<br>
A signal is an asynchronous notification sent to a process or to a specific thread within the same process in order to notify it of an event that occurred.<br>
<li>jobs - An alternate way of listing the processes. jobs is a shell builtin command which gives you information internal to the shell such as the job numbers.<br>
‘jobs’ lists the jobs that the current shell is managing.<br>
<li>bg - used to put a process in background.
<li>fg - used to put a process in foreground.

<u>Permissions</u>

<table>
<tr>
<td>chmod</td><td> modify file access rights</td>
</tr>
<tr>
<td>su</td><td>temporarily become super user</td>
</tr>
<tr>
<td>chown</td><td>change file ownership</td>
</tr>
</tr>
<tr>
<td>chgrp</td><td>change group ownership</td>
</tr>
</table>

<u>Link</u><br>
A link provides a connection between files. This provides the ability to have a single file or directory referred to through different names.<br>
The nearest comparison with the Windows world is of a shortcut, but that is an unfair comparison as a link in Linux is far more powerful. A Windows shortcut is just a way of launching a file from a different place, whereas a link can make a file appear in multiple locations which is invisible to the applications.<br>
There are two types of links that can be created. <br><ol><li>Hard link<li>Soft link (sometimes called symbolic link or symlink).</ol> The command to create these is the same - ln.<br>
<li align=justify>Hard Link:- A hard link creates a second file that refers to the same file on the physical disk. This is achieved by having two filenames that point directly at the same file. This is normally used where file entries (links) are on the same filesystem. When a hard link is created then all the names that link to that file are given the same status. Deleting one of the files will break the link, but the file can still exist under the other linked filenames. This works by maintaining a counter of the number of filenames that the file has. When the number of filenames reaches zero then the file is considered to be deleted and is removed. The number of filenames for a file can be seen using the ‘ls -l’ command. The number following the file permissions indicates the number of linked filenames.<br>
<li align=justify>The following screenshot shows that filename1 and filename2 are to linked files with one of the file denoted by the 2 (in this case the same file, but they could be to completely different files), the file not link is a single file denoted by the 1.<br>
ls -l<be>
total 2432<br>
-rw-r–r– 2 stewart stewart 1241088 2009-01-23 15:26 filename1<br>
-rw-r–r– 2 stewart stewart 1241088 2009-01-23 15:26 filename2<br>
-rw-r–r– 1 stewart stewart 0 2009-01-23 15:26 not link<br>
du -h<br>
1.2M<br>
ln filename1 filename2<br>
The default for the ln command is a hard link. Assuming filename1 already exists filename2 is created using: ln filename1 filename2
<li align=justify>Soft Link:- A soft link is sometimes referred to as a symbolic link or symlink. A filename created as a soft link is a special file that has the pathname of the file to redirect to. Behind the scenes when you try and access a symlink it just goes to the filename referred to instead.<br>

In the following example a file has been created called original file with a soft link to that same file called softlink tofile. As you can see the ls command makes it clear that this is a link through the l at the beginning of the file permissions and due to the reference notation after the filename.<br>
ls -l<br>
total 440<br>
-rw-r–r– 1 stewart stewart 446464 2009-01-23 15:21 original file<br>
lrwxrwxrwx 1 stewart stewart 13 2009-01-23 15:20 softlink tofile -> original file<br>
$ rm original file<br>
$ ls -l<br>
total 0<br>
lrwxrwxrwx 1 stewart stewart 13 2009-01-23 15:20 softlink tofile -> original file<br>
$ cat softlink tofile<br>
cat: softlink tofile: No such file or directory<br>
The -s option is used on the ln command to create a softlink.<br>
ln -s original file softlink tofile<br>

### Pitfalls while using links
<ol><li>There are some things that you need to be aware of, particularly when using softlinks.
<li>Some programs (e.g. Apache) can be configured to not follow soft links (from 18a security
<li>When creating backup files you need to be aware of how the particular backup program / tool
<li>Using one method the program may not backup the file referenced resulting in an incomplete backup 
<li>Using another method the program may end up backing up both as individualvfiles using double the space for that
<li>Using the second method of the above could result in the file being restored asva real file rather than as a link, breaking their connection
<li>The original file could be deleted without realising that there are other symlinked files referring to it
</ol>
Despite these pitfalls there are many advantages to using both hard and soft links
to provide multiple references to files.


### Output:
<ahref="img.jpg> </a>
### Result:
The Linux commands for redirection of standard I/O, pipes, filters, job control and links in linux were studied and output was verified.

# <center>Experiment 3 </center>
## <center>ADVANCE LINUX COMMANDS</center>
### Aim:
Advanced linux commands curl, wget, ftp, ssh and grep.
### Overview:
<li>curl<br>
curl is a tool to transfer data from or to a server, using one of the supported protocols (DICT, FILE, FTP, FTPS, GOPHER, HTTP, HTTPS, IMAP, IMAPS,
LDAP, LDAPS, POP3, POP3S, RTMP, RTSP, SCP, SFTP, SMB, SMBS, SMTP,
SMTPS, TELNET and TFTP). The command is designed to work without user
interaction.<br>
‘curl link’ - gives information about the website and outputs the html code.<br>
‘curl -O link/file.html’ - copies the html code of the website to file.html<br><br>

<li>ssh<br>
<li>ssh<br>
ssh (SSH client) is a program for logging into a remote machine and for executing
commands on a remote machine. It is intended to replace rlogin and rsh, and
provide secure encrypted communications between two untrusted hosts over an
insecure network. X11 connections and arbitrary TCP/IP ports can also be
forwarded over the secure channel.
<br>
ssh connects and logs into the specified hostname (with optional user name).
The user must prove his/her identity to the remote machine using one of several
methods depending on the protocol version used.
<br>
If command is specifieded, command is executed on the remote host instead of
a login shell.
<br>
<u>BASIC COMMAND</u>
<br>
$ ssh remote_host
<br>
The remote host in this example is the IP address or domain name that
you are trying to connect to. If your username is different on the remote system,
you can specify it by using this syntax:
<br>
$ ssh remote_username@remote_host
<br>
<u>TO COPY FILES</u>
</br>
$ scp source destination
<br>
<u>COPY A FILE FROM HOST TO LOCAL</u>
<br>
$ scp localhostfile.txt jsmith@remotehost.example.com:/home/jsmith/localhostfile.txt
<br>
<u>COPY A FILE FROM LOCAL TO HOST</u>
</br>
$ scp localhostfile.txt jsmith@remotehost.example.com:/home/jsmith/localhostfile.txt
12<br>
<u>TO SHUTDOWN CONNECTED COMPUTER</u>
</br>
$ ssh user@remote\_computer
<br>
$ sudo poweroff
<br>
$ sudo reboot
<li>wget
<br>
GNU wget is a free utility for non-interactive download of fies from the Web.
It supports HTTP , HTTPS , and FTP protocols, as well as retrieval through
HTTP proxies.
<br>
Wget is non-interactive, meaning that it can work in the background, while
the user is not logged on. This allows you to start a retrieval and disconnect
from the system, letting Wget fnish the work. By contrast, most of the Web
browsers require constant user's presence, which can be a great hindrance when
transferring a lot of data.
</br>
Wget can follow links in HTML , XHTML , and CSS pages, to create lo-
cal versions of remote web sites, fully recreating the directory structure of the
original site. This is sometimes referred to as "recursive downloading." While
doing that, Wget respects the Robot Exclusion Standard (/robots.txt). Wget
can be instructed to convert the links in downloaded Files to point at the local Files, for online viewing.
Wget has been designed for robustness over slow or unstable network con-
nections; if a download fails due to a network problem, it will keep retrying
until the whole File has been retrieved. If the server supports regetting, it will
instruct the server to continue the download from where it left off.
<br>
wget http://www.openss7.org/repos/tarballs/strx25-0.9.2.1.tar.bz2 this
command will download a single file and store it in the current repository.
<br>
wget -O wget.zip http://ftp.gnu.org/gnu/wget/wget-1.5.3.tar.gz Us-
ing -O (uppercase) option, downloads file with differenterent file name. Here we have
given wget.zip file name as show below.
<br>
wget -c http://www.openss7.org/repos/tarballs/strx25-0.9.2.1.tar.bz2
Restart a download which got stopped in the middle using wget -c option.
<br>
wget -mirror [WebsiteName] If you wish to retain a copy of any
website that you may like to refer to/read locally, or maybe save a copy of your
blog to the hard disk as back up, you may execute the wget command with
mirror option.
<br>
wget -i download file-list.txt allows you to download multiple files
stored in download-file-list.txt simultaneously.
<br>
<li>ftp
<br>
The FTP (File Transfer Protocol) utility program is commonly used for copying
file to and from other computers. These computers may be at the same site
or at different sites thousands of miles apart. FTP is a general protocol that
works on UNIX systems as well as a variety of other (non-UNIX) systems.
<br>
To connect your local machine to the remote machine, type
ftp machinename
<br>

where machinename is the full machine name of the remote machine, e.g.,
some-url.com. If the name of the machine is unknown, you may type
ftp IP-Address
<br>
where machinennumber is the net address of the remote machine, e.g.,
129.82.45.181. In either case, this command is similar to logging onto the remote
machine. If the remote machine has been reached successfully, FTP responds
by asking for a loginname and password.
<br>
When you enter your own loginname and password for the remote machine,
it returns the prompt
<br>
ftp >
<br>
and permits you access to your own home directory on the remote machine.
You should be able to move around in your own directory and to copy files to
and from your local machine using the FTP interface commands.
<br>
<table>
<tr colspan= "2">
<tr>
<td>?</td><td>request help or info about FTP Commands</td></tr>
<tr></td><td>cd</td><td>change directory in remote machine</td></tr>
<tr><td>close</td><td>terminate a connection with remote computer</td></tr>
<tr><td>delete</td><td>delete a file in remote computer</td></tr>
<tr><td>get</td><td>get a copy of a file in the remote machine to local machine</td></tr>
<td><tr>ls</tr><tr>list the names of files in the current directory in the remote machine</td>
<tr><td>mkdir</td><td>make a new directory in the remote machine</td></tr>
<tr><td>pwd</td><td>print the working directory in remote machine></td></tr>
<tr><td>quit</td><td>exit ftp environment</td></tr>
</table>
<li>grep
<br>
GREP : Global Regular Expression Print
<br>
Searches for text in a file
<br>
Can search for simple words.
<br>
Can look for regular expression - more complex charecter strings(
words followed by any no of spaces, followed by a digit or lowercase letter).
Searching the given string
<br>
&npsb '$ grep <literal string> ' filename To search a specific string in a
specified file<br>

Case insensitive search
<br>
$ grep -i ?string? filename
<br>
$ grep -i ?string? FILE PATTERN
<br>
-This searches for given string/pattern case insensitively.
<br>
Simple regular expressions
<br>
?[0-9]? look for any digit
<br>
?[a-zA-Z]? look for one upper or lower case letter
<br>
?.? look for one charector
<br>
?.*? any number of charectors
<br>
?n.? a literal decimal point
<br>
?n.161:? dot, then 161, then colon
<br>
?n.161[: ]? dot, then 161, then colon or space
<br>
Advanced regular expressions
<br>
Look for lines that hold either string1 or string2
<br>
$ grep -E ?(string1|string2)? flename
<br>
Lines that have string1 followed by string2 on the same line, but
<br>
possibly with other charectors in between.
<br>
$ grep ?string1.*string2? flename
<br>
String1 has to be at the beginning of the line.
<br>
$ grep ?^string1? flename
<br>
Look for it at the end of the line.
<br>
$ grep ?string1$? flename

<br>Output

<br>Result
<br>The advanced linux commands ftp, ssh, wget, grep and curl were studied. 
<br>
References
[1] Basic FTP Commands. url: https://www.cs.colostate.edu/helpdocs/
ftp.html.
[2] curl. url: https://curl.haxx.se.
[3] File Transfer Protocol. url: https://en.wikipedia.org/wiki/File_
Transfer_Protocol.
[4] GNU Wget. url: https://www.gnu.org/software/wget/.



