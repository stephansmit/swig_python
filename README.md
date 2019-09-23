# Swig with Python

Example how to create a python interface to a c code.

## Requirements
~~~~
sudo apt-get install swig
sudo apt-get install python3-dev
~~~~

## Compilation
~~~~
swig -python example.i
gcc -fPIC -c example.c example_wrap.c -I/usr/include/python3.5
ld -shared example.o example_wrap.o -o _example.so
~~~~

