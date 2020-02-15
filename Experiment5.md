# <Text align="center">Experiment 5</Textext>
## <center>Shell script to show various system configurations</center>
### Aim:
Write shell script to show various system configurations like
<li>your OS and version, release number, kernel version</li>
<li>all available shells</li>
<li>computer CPU information like processor type, speed etc</li>
<li>memory information</li>
<li>hard disk information like size of hard-disk, cache memory, model etc</li>
<li>File system (Mounted)</li>
</br>

### Programme
\#!/bin/bash<br>
echo -e "`cat /etc/os-release`"<br>
echo -e "`cat /etc/shells`"<br>
echo -e "`xset q`"<br>
echo -e "`cat /proc/meminfo`"<br>
echo -e "Driver: `sudo hdparm -I /dev/sda`"<br>
echo -e "`cat /proc/mounts`"<br>

### Output
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/Exp5_1.png)
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/Exp5_2.png)
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/Exp5_3.png)

### Result
A Shell script programme to show various system configurations has been made and executed successfully.
