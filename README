# cppscript
## Hopefully, a handy tool to run C++ code as shell scripts.

Some times I find my self trying out some C++ code so I always do the same thing

    $ vi test.cpp
    ...write...
    $ g++ -Wall -Wextra -Werror --std=c++11 -o test test.cpp -lxyz
    $ ./test

Ok, yes. I can write a `Makefile` to do that:
    $ vi test.cpp
    ...write..
    $ make
    ...compiles and run...
    
But I thought in proper scripting languages you just write and run. So I want to do the same thing in C++.
I could've installed an existing C++ interpreter like CINT or Cling but I wanted to have my own bit of fun. So there we go.

    $ vi test.cpp
    #!/usr/bin/cppscript

    #include <iostream>

    void main() { std::cout << "Hello world" << std::endl; }

    $ ./test.cpp
    
What `cppscript` should then do is use temporary files to call gcc and run the fnal executable.
