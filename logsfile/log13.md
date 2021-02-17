# So far
- Update a test example to check whether the cgal has been installed successfully.

# Understanding

The difference between C and python is that C has many data types whereas python only has one object.

swig is a thing that helps the programmer to automatically generate binding codes. Originally, we have a library in C and we hope to make it accessible via python. We can not explicitly use it and thus, we add a wrapper function, or say file, for it to form a python module to be used. This wrapper function will make the double transformation between python and C, especially in terms of data type. However, this process is tedious.

In turn, we use swig to generate automatically. We still have to write SWIG interface file to list all the function that are used to be interfaced. 

According to [this slides](https://en.opensuse.org/images/e/eb/Kkaempf_KnowledgeSharing_Swig.pdf), the process would look like this: lib.h + lib.i -(swig)-> lib_wrapper.c -(gcc)-> lib_wrap.so. And lib_wrap.so can be used by python.
  


# Points
src := system resource controller

library := A library is a collection of implementations of behavior, written in terms of a language, \
that has a well-defined interface by which behavior is invoked. 

Static libraries are incorporated into a program executable before the program is run.

Shared libraries(.so/.dylib) are loaded at program start-up and may be shared by different programs.

Dynamically loaded libraries are loaded while the executable is running.

# Reference
- header/source file in C https://cs.brynmawr.edu/Courses/cs246/spring2013/slides/04FunctionsAndHeaderFiles.pdf
- generate bindings for C from swig https://en.opensuse.org/images/e/eb/Kkaempf_KnowledgeSharing_Swig.pdf
- tutorial videos for swig https://www.youtube.com/watch?v=J-iVTLp6M9I&t=12s
- library classification https://www.massey.ac.nz/~dpplayne/159732/Lecture05-Libraries.ppt
- Gomory's method http://eventos.cmm.uchile.cl/discretas2016/wp-content/uploads/sites/26/2016/01/L2.pdf
