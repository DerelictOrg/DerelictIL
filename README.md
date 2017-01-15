DerelictIL
==========

A dynamic binding to version 1.8.0 of the [DevIL][1] library for the D Programming Language.

Please see the [Derelict documentation][2], for information on how to build DerelictIL and load DevIL at run time. In the meantime, here's some sample code.

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
[2]: https://derelictorg.github.io/

