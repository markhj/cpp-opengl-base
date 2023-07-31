This is a "starter pack" for getting into OpenGL with C++. It utilizes the vcpkg package manager which is required to install dependencies.

# Prerequisites

* vcpkg (and basic knowledge of how it works). It is used in **manifest mode**.
* C++ environment, for example CLion or Visual Studio

# Libraries

There are plenty of library choices out there for OpenGL. In this particular application we use:

- GLFW
- GLEW
- GLM
- Assimp
- stb_image

Replacing them with alternatives shouldn't be too complicated, if you wish to go with other libraries.

# Getting started

Clone the project and open it in your favorite IDE.

From console/command line run:

````bash
vcpkg install
````

The build is tested on Windows 64-bit with MinGW/GCC compiler.
You may need to tweak vcpkg to get it to work with other compilers.

It should now be possible to compile the project and see a window with a colored triangle.

## Alternatives to vcpkg
You can of course ignore the vcpkg approach and use another method to include the libraries, such as MSYS2.

The libraries you will need are listed above.

