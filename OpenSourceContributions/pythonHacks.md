#Python LAMBDA Hacks

**you master lambda, you master shortcuts**

    data=[(lambda x:x.text)(x.extract())  for x in soup.findAll('p') ]
                      ^1           ^2         ^3           ^4

here we can see 4 parts of the list comprehension:

 - 1: i finally want this
 - 2: x.extract will perform some operation on x, here it pop the element from soup
 - 3: x is the list iterable which is passed to the input of lambda at 2 along with extract operation
 - 4: some arbitary list


