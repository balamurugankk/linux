

== sed examples ==

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

  # sed -n '2p' 1.txt 
  two is my thought
  # sed -n '1,3p' 1.txt 
  one is my dream
  two is my thought
  one is my favourite
  # sed -n '1p' 1.txt 
  one is my dream
::: 
*statement* 
:::
