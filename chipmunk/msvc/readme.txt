This subdirectory contains project and solution files for building
the Chipmunk Physics library and its demo suite with Microsoft Visual C++.

There are separate directories for each compiler version.  The Developer
Studio program likes to refer to itself with a year but it also has a version
number. Here are the correspondences:

    MSVC 2008: vc9
    MSVC 2010: vc10

The demo suite uses the external GLUT (OpenGL Utility Toolkit) library for
rendering.  A copy is included in the glut subdirectory.  The demo program
will look for glut.dll at load time, so you'll need to ensure it is findable.
One way to do this is to set the working directory (found under Debugging
configuration properties in Developer Studio) to "../../glut/runtime". This
will launch the demo in that directory, enabling Windows to find the required
DLL.
