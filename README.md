# CI-CD
CS 478: Independent Study

The first project is contained in the extras/cmake/helloworld directory of the GitHub repository. 
In this example a simple “Hello World” C++ program is built (HelloWorld.cpp)

The Hello World C++ Example
provided in /src/

 CMakeLists.txt, which contains the contents of CMakeLists.txt file 
 -----------------------------
 
 The CMakeLists.txt file in Listing 2 consists of only three lines:
The first line sets the minimum version of CMake for this project, which is major version 2, minor version 8, and patch version 9 in this example. 
This version is somewhat arbitrary in this example, but providing a version number allows for future support for your build environment. 
Therefore, you should use the current version of CMake on your system, which for this example is determined just below.
The second line is the project() command that sets the project name.
The third line is the add_executable() command, which requests that an executable is to be built using the helloworld.cpp source file. 
The first argument to the add_executable() function is the name of the executable to be built, and the second argument is the source file from which to build the executable.
To build the project, first test that you have CMake installed, and if not, install it using the package manager that is used by your  Linux OS. 

This command installs cmake library in Linux
:~/$ sudo apt-get install cmake
-----------------------------------
This command it shows the version of cmake
:~/$ cmake -version
---------------------------------------
The project code is in the GitHub repository directory or in your root directory if you using local, for example
erald@erald:~/CI-CD/CI-CD$
Now you are ready to build the Hello World project using CMake — execute the cmake command and pass it the directory that contains the source code and the CMakeLists.txt file — in this case “.” refers to the current directory:
erald@erald:~/CI-CD/CI-CD$ cmake .
-----------------------------------------
CMake identified the environment settings for the Linux device and created the Makefile for this project, which can be viewed.

Once the Makefile has been created, the make command can be used to build the project:
erald@erald:~/CI-CD/CI-CD$ make
------------------------------
Scanning dependencies of target hello
 [100%] Building CXX object CMakeFiles/Hello.dir/Helloworld.cpp.o
 Linking CXX executable Hello
 [100%] Built target Hello
Now we can run our program by doing the following.
erald@erald:~/CI-CD/CI-CD$ ./Hello
---------------------------------------------


