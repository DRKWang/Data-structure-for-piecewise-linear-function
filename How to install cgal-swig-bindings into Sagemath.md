How to install cgal-swig-bindings on Mac OS X with homebrew for Python

Replace the python paths below with the correct version for your system and follow the following instructions in the terminal.

```
brew install cgal 

brew install swig

git clone https://github.com/CGAL/cgal-swig-bindings.git 

cd cgal-swig-bindings
```

#setting the configuration of the python version of cgal

```
cmake -DCGAL_DIR=/usr/local/lib/cmake/CGAL \ 
-DBUILD_PYTHON=ON \
-DBUILD_JAVA=OFF \
-DPYTHON_LIBRARIES=/usr/local/lib/python3.9 \
-DPYTHON_LIBRARY=/usr/local/Cellar/python@3.9/3.9.1/Frameworks/Python.framework/Versions/3.9/lib/libpython3.9.dylib\
-DPython_FRAMEWORKS=/usr/local/Cellar/python@3.9/3.9.1/Frameworks/Python.framework \
-DPYTHON_INCLUDE_DIR=/usr/local/Cellar/python@3.9/3.9.1/Frameworks/Python.framework/Headers

make

cd build-python 
```

#move the generated CGAL folder to location under the site-packages of sage

```
sudo mv CGAL/ /Users/binshuaiwang/Sage/sage-9.2/local/lib/python3.8/site-packages 

```
