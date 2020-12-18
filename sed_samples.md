## sed examples

```
# sed '/one/p' 1.txt
one is my dream
one is my dream
two is my thought
one is my favourite
one is my favourite
three is my fate`
```
```
# sed '/two/p' 1.txt
one is my dream
two is my thought
two is my thought
one is my favourite
three is my fate
```
```
# sed -n '/two/p' 1.txt
two is my thought
```
```
# sed -n '2p' 1.txt
two is my thought
```
```
# sed -n '1,3p' 1.txt
one is my dream
two is my thought
one is my favourite
```
```
# sed -n '1p' 1.txt
one is my dream
```
```
# sed -n '/through/,$p' 2.txt
The car went through the tunnel.
I got a package from a friend.
I have liked that song since 1999.
She put the flowers by the window.
The food was placed on the table.
# 
```

:::
*statement*
:::
