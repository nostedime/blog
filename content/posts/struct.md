+++
date = '2025-09-17T14:41:55+02:00'
title = 'Struct'
+++



## Global or not

```
struct
{
	int x;
	int y;
};
```


declares a structure of type struct { int x, int y }. And yes, the type contains the members in brackets.


If you add a tag like this :

struct point
{
	int x;
	int y:
};
You refer to "{ int x, int y }" by the new tag point.



Now if you would need to initialize a variable named "my_point" of type "struct point".
How would you do ? 

- you could do it directly at declaration step :
struct { int x; int y } my_point;

or with declaration and then initialization.
- struct point { int x; int y} my_point;



Deep dive into declaration of structs.

To understand better structs declaration. I have tried some silly things such as 
