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
<br>
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/op_exp3.png)

<br>Result
<br>The advanced linux commands ftp, ssh, wget, grep and curl were studied. 
<br>
References<br>
[1] Basic FTP Commands. url: https://www.cs.colostate.edu/helpdocs/
ftp.html.<br>
[2] curl. url: https://curl.haxx.se.<br>
[3] File Transfer Protocol. url: https://en.wikipedia.org/wiki/File_
Transfer_Protocol.<br>
[4] GNU Wget. url: https://www.gnu.org/software/wget/.



