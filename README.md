# cmake_apollo_hdmap
Apollo HDMap SDK compiled with cmake.

# how to build
```
sudo bash build.sh
```

# how to test map
<<<<<<< HEAD
```
build/test_api testdata/base_map.bin
```
=======
build/test_api testdata/base_map.bin
>>>>>>> 2a3d05661cbe1250cbf92afce7b3a30bf47af841

## dep
```
sudo apt-get install autoconf automake libtool curl make g++ unzip
```
+ protobuf-3.3.0: compile with source
```
sudo apt-get install libprotobuf-dev protobuf-compiler
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
https://github.com/leethomason/tinyxml2

The package tinyxml2 provides CMake targets:
    find_package(tinyxml2 CONFIG REQUIRED)
    target_link_libraries(main PRIVATE tinyxml2::tinyxml2)

```

+ eigen3

```
sudo apt-get install libeigen3-dev 
```

+ OpenCV <br/>
[安装方法](https://docs.opencv.org/4.x/d7/d9f/tutorial_linux_install.html)

+ Boost <br/>
[安装方法](https://www.aiuai.cn/aifarm1186.html#:~:text=Ubuntu%20-%20Boost%20%E5%BA%93%E7%BC%96%E8%AF%91%E5%AE%89%E8%A3%85.%20Boost%E5%BA%93%E6%98%AF%E4%B8%BAC%2B%2B%E8%AF%AD%E8%A8%80%E6%A0%87%E5%87%86%E5%BA%93%E6%8F%90%E4%BE%9B%E6%89%A9%E5%B1%95%E7%9A%84%E4%B8%80%E4%BA%9BC%2B%2B%E7%A8%8B%E5%BA%8F%E5%BA%93%E7%9A%84%E6%80%BB%E7%A7%B0%EF%BC%8C%E7%94%B1Boost%E7%A4%BE%E5%8C%BA%E7%BB%84%E7%BB%87%E5%BC%80%E5%8F%91%E3%80%81%E7%BB%B4%E6%8A%A4.%20Boost%E5%90%91%E6%9D%A5%E6%9C%89%E5%87%86%E6%A0%87%E5%87%86%E5%BA%93%E4%B9%8B%E7%A7%B0%EF%BC%8C%E5%BE%88%E5%A4%9A%E6%96%B0%E7%89%B9%E6%80%A7%E4%BE%8B%E5%A6%82%E6%99%BA%E8%83%BD%E6%8C%87%E9%92%88%E7%AD%89%E9%83%BD%E6%98%AF%E5%85%88%E5%9C%A8boost%E4%B8%AD%E5%AE%9E%E7%8E%B0%EF%BC%8C%E5%90%8E%E6%9D%A5%E8%A2%AB%E5%90%B8%E6%94%B6%E5%88%B0%E6%A0%87%E5%87%86%E5%BA%93%E4%B9%8B%E4%B8%AD.%20Boost%E5%AE%9E%E7%8E%B0%E4%BA%86%E6%97%A5%E5%BF%97%E3%80%81%E7%AE%97%E6%B3%95%E3%80%81%E6%97%A5%E6%9C%9F%E3%80%81%E5%9C%B0%E7%90%86%E3%80%81%E6%95%B0%E5%AD%A6%E3%80%81%E7%BA%BF%E7%A8%8B%E5%8D%8F%E7%A8%8B%E7%AD%89%E5%90%84%E7%A7%8D%E5%AE%9E%E7%94%A8%E5%B7%A5%E5%85%B7.%20Boost,Boost%20%E5%BA%93%20apt%20%E5%AE%89%E8%A3%85.%20Ubuntu%20%E6%8F%90%E4%BE%9B%E4%BA%86%20apt%20%E5%AE%89%E8%A3%85%E6%96%B9%E5%BC%8F%EF%BC%8C%E5%A6%82%EF%BC%9A).

+ glog <br/>
[安装方法](https://blog.csdn.net/liuxiaodong400/article/details/82951402)

+ gflags <br/>
[安装方法](https://blog.csdn.net/qq_21597761/article/details/102544703)