compile commands
~~~~
swig -python example.i
gcc -fPIC -c example.c example_wrap.c -I/usr/include/python3.5
ld -shared example.o example_wrap.o -o _example.so
~~~~

requirements:
~~~~
sudo apt-get install tcl8.6-dev
sudo apt-get install swig
sudo apt-get install python3-dev
~~~~
