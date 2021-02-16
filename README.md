# Description

`baseconv` is a simple multi-base converter.
It supports base conversions from base 1 to base 36.
Numbers contain characters from 1 to 9, and from A to Z.
Note that `baseconv` is case-insensitive.

# Usage

```
>>> import baseconv
>>> baseconv.license()  -->  displays license
baseconv.baseXtoY(num, **X, **Y)  -->  converts num from base X to base Y
# X and Y are keywords arguments

# example:
>>> baseconv.baseXtoY('FF', X=16, Y=10)  # will work
255
>>> baseconv.baseXtoY('FF', 16, 10)  # will not work since X and Y are not positional.
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: baseXtoY() takes 1 positional argument but 3 were given
```
