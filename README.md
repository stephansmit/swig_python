compile commands
~~~~
swig -tcl example.i
gcc -fpic -c example.c example_wrap.c -I/usr/include/tcl8.6
~~~~

requirements:
~~~~
sudo apt-get install tcl8.6-dev
sudo apt-get install swig
sudo apt-get install python3-dev
~~~~
