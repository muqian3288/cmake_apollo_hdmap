# cmake_apollo_hdmap
Apollo HDMap SDK compiled with cmake.


## dep
```
sudo apt-get install autoconf automake libtool curl make g++ unzip
```
+ protobuf-3.3.0: compile with source
```
git clone -b v3.3.0 https://github.com/protocolbuffers/protobuf
cd protobuf
./autogen.sh
./configure --prefix=/shared_dir/opt
make -j8 -l8
sudo make install 
sudo ldconfig
cd ..
rm -rf protobuf
```
+ proj.4-4.9.3: compile with source
https://download.osgeo.org/proj/proj-4.9.1.tar.gz
```
./autogen.sh
./configure --prefix=/shared_dir/opt
make -j8 -l8
sudo make install 
sudo ldconfig
```
+ tinyxml2-5.0.1: compile with source
```
git clone -b 5.0.1 https://github.com/leethomason/tinyxml2.git
cd tinyxml2
mkdir build && cd build
cmake -DCMAKE_INSTALL_PREFIX=/shared_dir/opt  ..
make 
make install
cd ..
rm -rf tinyxml2
```