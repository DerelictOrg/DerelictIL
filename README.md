DerelictIL
==========

A dynamic binding to version 1.7.8 of the [DevIL][1] library for the D Programming Language.

For information on how to build DerelictIL and link it with your programs, please see the post [Using Derelict][2] at The One With D.

For information on how to load the DevIL library via DerelictIL, see the page [DerelictUtil for Users][3] at the DerelictUtil Wiki. In the meantime, here's some sample code.

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

NOTE: In the Windows binary packages downloadable from the [DevIL homepage][1], DevIL.dll does not properly export the function ilFlipSurfaceDxtcData. Therefore, I have currently disabled it in the binding.

[1]: http://openil.sourceforge.net/
[2]: http://dblog.aldacron.net/derelict-help/using-derelict/
[3]: https://github.com/DerelictOrg/DerelictUtil/wiki/DerelictUtil-for-Users

