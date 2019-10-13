---
layout: post
title: Boolean Returning String Methods in Base Python vs. Pandas Series
---

When dealing with strings in Python, there are several [methods](https://docs.python.org/3/library/stdtypes.html#string-methods) 
that will take in the string and return a boolean value. <br> These include:
* str.isalnum()
* str.isalpha()
* str.isdecimal()
* str.isdigit()
* str.islower()
* str.isnumeric()
* str.isspace()
* str.istitle()
* str.isupper()

All of these methods will apply a different conditional on the string in question and output a boolean value (True/False).<br>

When using any of the methods that are listed above, there are no parameters that need to be listed inside the rounded brackets.

If a pandas series has strings in it, you can also use [string handling methods](https://pandas.pydata.org/pandas-docs/stable/reference/series.html#string-handling) 
to deal with the individual strings. <br> These include:

* Series.str.isalnum()
* Series.str.isalpha()
* Series.str.isdecimal()
* Series.str.isdigit()
* Series.str.islower()
* Series.str.isnumeric()
* Series.str.isspace()
* Series.str.istitle()
* Series.str.isupper()

When using these methods, note that null values `NaN` will also output null values. The way to prevent this is to specify the parameter 
`na` to equal either `True` or `False`. It would look something like this.

`Series.str.isalpha(na=False)`


**Coming up:** Code examples of how this works!
