PRINT PATTERN  1 4*5*6 2*3
For any input number N Print the following code – For below code N=4

1
4*5*6
2*3
7*8*9*10
PREREQUISITE:
Basic knowledge in Java programming, usage of loops.

ALGORITHM:
Take input from user i.e number of lines required (N value).
Take two loops one for each line (say ‘i’) and other for each digit in a particular line (say ‘j’). i starts from N and j starts from 1.
Take a result variable (say ‘a’) and initialize it with 1, t with 4, k with 3.
Divide the pattern into two i.e, parts even and odd lines.
Here ‘i’ loop is used to access each line from n to 1 and ‘j’ loop is used to print values in each line. j loop is executed until it reaches i-1 value in odd lines and k value in even lines.
Print ‘a’,’t’ value along with * and post increment.
Print the final value ‘a’ and ‘t’ of each line and go to next line.
Repeat the ‘i’ loop until it reaches n.
CODE IN JAVA:
[code language=”java”]
import java.lang.*;
import java.io.*;
class Pattern
{
public static void main(String[] args)throws IOException
{
BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
int n,i,j,a=1,t=4,k=3;
System.out.print("Enter N value:");
n=Integer.parseInt(br.readLine());
for(i=1;i&lt;=n;i++)
{
if(i%2!=0)
{
for(j=1;j&lt;(i-1);j++)
{
System.out.print((a++)+"*");
}
System.out.println(a++);
}
else
{
for(j=1;j&lt;k;j++)
{
System.out.print((t++)+"*");
}
System.out.println(t++);
k++;
}
}
}
}
[/code]

 

TAKING INPUT:


DISPLAYING OUTPUT:
