# <center>Experiment 4 </center>
## <center>Shell Programming</center>
### Aim:
Write shell script to show various system configuration like<br>
<li>Currently logged user and his login name
<li>Your current shell
<li>Your home directory
<li>Your operating system type
<li>Your current path setting
<li>Your current working directory
<li>Number of users currently logged inAdvanced linux commands curl, wget, ftp, ssh and grep.<br>


clear<br>
log=`who|wc -l`<br>
echo "the currently logged in user is $USER"<br>
echo "the current shell is $SHELL"<br>
echo "the home drectory is $HOME"<br>
echo "the os type is $OSTYPE"<br>
echo "the current path setting is $PATH"<br>
echo "the working directory is $PWD"<br>
echo "there are $log users logged in"<br>

### Output

![](https://raw.githubusercontent.com/sreejiths1979/foss/master/exp4.png)

### Result
The shell script for displaying various system configurations were made and the
output was verified. The script was run on Ubuntu 18.1. 




