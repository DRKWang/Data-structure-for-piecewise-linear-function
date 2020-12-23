How to install cgal-swig-bindings on Mac OS X with homebrew for Python

Follow the following instructions in the terminal.

```
brew install cgal

brew install swig

git clone https://github.com/CGAL/cgal-swig-bindings.git

cd cgal-swig-bindings

cmake -DCGAL_DIR=/usr/local/lib/cmake/CGAL \
-DBUILD_PYTHON=ON \
-DBUILD_JAVA=OFF \
-DPYTHON_LIBRARIES=/usr/local/lib/python3.9 \
-DPYTHON_OUTDIR_PREFIX=/Users/binshuaiwang/Sage/sage-9.2/local/lib/python3.8/site-packages

make
```
