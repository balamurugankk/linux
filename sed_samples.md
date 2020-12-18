### sed examples

```
# sed '/one/p' 1.txt
one is my dream
one is my dream
two is my thought
one is my favourite
one is my favourite
three is my fate`
```
*** will print again the line contains `two` : ***
```
# sed '/two/p' 1.txt
one is my dream
two is my thought
two is my thought
one is my favourite
three is my fate
```
*** will print the line contains `two` of file : ***
```
# sed -n '/two/p' 1.txt
two is my thought
```
*** will print the 2nd line of file : ***
```
# sed -n '2p' 1.txt
two is my thought
```
** will print the 1-3 line of file : ***
```
# sed -n '1,3p' 1.txt
one is my dream
two is my thought
one is my favourite
```
*** will print the 1st line of file : ***
```
# sed -n '1p' 1.txt
one is my dream
```
*** will print section of file from a line containing “GREEN” to end of file : ***
```
# sed -n '/through/,$p' 2.txt
The car went through the tunnel.
I got a package from a friend.
I have liked that song since 1999.
She put the flowers by the window.
The food was placed on the table.
#
```
*** will print  3p prints third line of input file ***
```
# sed -n '4'p 2.txt
3p prints third line of input file
#
```
***  will print 4~3p prints every 3nd line starting from 4th line as shown below. ***
```
# sed -n '4~3'p 2.txt
The cat jumped off the counter.
The book belongs to Anthony.
The sun is above the clouds.
He swam at the lake.
The car went through the tunnel.
She put the flowers by the window.
#
```
***  will print ***
```
```
***  will print ***
```
```
***  will print ***
```
```
***  will print ***
```
```
*** will print ***
```
```
:::
*statement*
:::
