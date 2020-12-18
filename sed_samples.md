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
*** will print section of file from a line containing `through` to end of file : ***
```
# sed -n '/through/,$p' 2.txt
The car went through the tunnel.
I got a package from a friend.
I have liked that song since 1999.
She put the flowers by the window.
The food was placed on the table.
#
```
*** 3p prints third line of input file ***
```
# sed -n '4'p 2.txt
3p prints third line of input file
#
```
*** 4~3p prints every 3nd line starting from 4th line as shown below. ***
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
*** print a block of data that starts with a line containing `belongs`, and ending with a line that contains `down`: ***
```
# sed -n -e '/belongs/,/down/p' 2.txt
The book belongs to Anthony.
They were sitting by the tree.
We are running in the gym today.
The sun is above the clouds.
She lives near her workplace.
She drew the picture with a crayon.
He swam at the lake.
I walked down the street.
#
```
*** print 5 consecutive lines after a pattern : ***
```
# sed -n '/lake/{n;p;n;p;n;p;n;p;n;p}' 2.txt
I walked down the street.
We located the key for the lock.
The car went through the tunnel.
I got a package from a friend.
I have liked that song since 1999.
#
#
# sed -n '/lake/{p;n;p;n;p;n;p;n;p;n;p}' 2.txt
He swam at the lake.
I walked down the street.
We located the key for the lock.
The car went through the tunnel.
I got a package from a friend.
I have liked that song since 1999.
#

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
