# Beecrypt 

The following is a stripped down version of Beecrypt-4.2.1, it contains the C interfaces only, Java, Python, and C++ interfaces have been removed. 

## License

The original Beecrypt library is available under the terms of the Lesser GNU Public License, in accordance with that license, the modified library contained in this directory is _also_ released under the Lesser GNU Public License 2.1.

### Notes on modification

One header was modified to prevent redefining assert() macro. This modification occurred on 4/3/2015.

The library's organization was modified to support building with CMake rather than autotools. This reorganization occurred on 3/29/2015. 
