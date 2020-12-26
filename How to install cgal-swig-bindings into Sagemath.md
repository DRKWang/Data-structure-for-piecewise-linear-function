How to install cgal-swig-bindings on Mac OS X with homebrew for Python

Replace the python paths below with the correct version for your system and follow the following instructions in the terminal.

```
alias python=python3

brew install cgal 

brew install swig

git clone https://github.com/CGAL/cgal-swig-bindings.git 

cd cgal-swig-bindings
```

#setting the configuration of the python version of cgal.

```
cmake -DCGAL_DIR=/usr/local/lib/cmake/CGAL \
-DBUILD_PYTHON=ON \
-DBUILD_JAVA=OFF \
-DPYTHON_OUTDIR_PREFIX=/Users/binshuaiwang/Sage/sage-9.2/local/lib/python3.8/site-packages

make

```

