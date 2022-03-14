# SomePython

### Scn #1
1. Print a-n: a b c d e f g h i j k l m n
2. Every second in a-n: a c e g i k m
3. Append a-n to index of urls{hello.com/, hej.com/, ..., hallo.com/}: hello.com/a hej.com/b ... hallo.com/n

##### Soln:

>>> import string
>>> string.ascii_lowercase[:14]
'abcdefghijklmn'
>>> string.ascii_lowercase[:14:2]
'acegikm'

[i + j for i, j in zip(list_of_urls, string.ascii_lowercase[:14])]

<<<-OR->>>
for i in range(ord('a'), ord('n')+1):
    print chr(i),





Split a string into N equal parts? [duplicate]
parts = [your_string[i:i+n] for i in range(0, len(your_string), n)]
