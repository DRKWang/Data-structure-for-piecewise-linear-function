# Target
- install the cgal_swig_bindings into sage

# So far
- has installed the cgal_swig_bindings successfully.
- But in some cases, we may encounter the error that the code was deprecated by the newer python version, which comes from
```Found Python: (found version "3.8.2") found components: Interpreter Development Development.Module Development.Embed``` 
  To solve this error, we can 
  - set the ```-DPython_EXECUTABLE=$SAGE_ROOT/build/bin/sage-python23```, which will git the direction to the python Compiler. 
  - set the root, ```-DPython_ROOT_DIR```.
  - Set the version of python, ```find_package(PythonInterp 3.5 REQUIRED)```.



# Reference
- [cmake template](https://mjmorse.com/blog/cmake-template/)
- [cmake wiki](https://gitlab.kitware.com/cmake/community/-/wikis/home)
- [cmake find package grammary](https://cmake.org/cmake/help/latest/command/find_package.html#search-procedure)
