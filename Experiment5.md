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
i="y"<br>
echo "enter the first number"<br>
read n1<br>
echo "enter the second number"<br>
read n2<br>
while [ $i = "y" ]<br>
	do<br>
	echo "1-addition"<br>
	echo "2-subtraction"<br>
	echo "3-multiplication"<br>
	echo "4-division"<br>
	echo "5-modulo division"<br>
	read c<br>
	case $c in<br>
1)sum=`expr $n1 + $n2`<br>
	echo "result="$sum;;<br>
2)sum=`expr $n1 - $n2`<br>
	echo "result="$sum;;<br>
3)sum=`expr $n1 \* $n2`<br>
	echo "result="$sum;;<br>
4)sum=`expr $n1 / $n2`<br>
	echo "result="$sum;;<br>
5)sum=`expr $n1 % $n2`<br>
	echo "result="$sum;;<br>
esac<br>
	echo "do you want to continue(y/n)"<br>
read i<br>
if [ $i != "y" ]<br>
	then<br>
	exit<br>
fi<br>
done<br>
<br>
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/calculator.png)
