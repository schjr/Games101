# Games101 Homework 3
By schjr

In homework 3, the incorrect solution to HW2 
caused chaos from the very beginning. Hence I
use sympy to calculate the Projection Matrix
from first principles, yet the cow is still 
upside down. Hence I added a z-axis rotation of 
degree $\pi$ to mitigate it.

A problem that requires attention is that using
auto to automatically deduce the type of variables
may fail. For example, a variable which must be float
is deduced to be an integer, and such problem is hard
to find. This teachs us that modern C++ is recondite:
```C++
//auto someVariable = (a->x).b().c();
float someVariable = (a->x).b().c();
```



Another thing that should be noticed is that
a cow which consists of absolute white and black can
be caused by incorrectly assign intensity of point
light source to that of the ambient.

The out-of-bound texture coordinate problem is
solved by Clamping.
