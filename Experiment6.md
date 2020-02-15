# <Text align="center">Experiment 6 </Text>
## <centre>Menu driven calculator</centre>
### Aim:
Write a shell script to implement a menu driven calculator with following functions
<li>Addition</li>
<li>Subtraction</li>
<li>Multiplication</li>
<li>Division</li>
<li>Modulus</li>
<br>

### Programme
<br>
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
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/exp6_1.png)
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/exp6_2.png)
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/exp6_1.png)<br>
![](https://raw.githubusercontent.com/sreejiths1979/foss/master/exp6_2.png)<br>
