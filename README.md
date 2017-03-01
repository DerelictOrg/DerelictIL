DerelictIL
==========

A dynamic binding to version 1.8.0 of the [DevIL][1] library for the D Programming Language.

Please see the sections on [Compiling and Linking][2] and [The Derelict Loader][3], in the Derelict documentation, for information on how to build DerelictIL and load DevIL at run time. In the meantime, here's some sample code.

```D
import derelict.devil.il;
import derelict.devil.ilu;
import derelict.devil.ilut;

void main() {
    // Load the DevIL/ILU/ILUT libraries, .
    DerelictIL.load();
    DerelictILU.load();
    DerelictILUT.load();

    // Now DevIL functions can be called.
    ...
}
```

[1]: https://github.com/DentonW/DevIL
[2]: http://derelictorg.github.io/building/overview/
[3]: http://derelictorg.github.io/loading/loader/

