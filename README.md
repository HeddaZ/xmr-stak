## Windows 编译

> * Visual Studio 2019
> * CMake

```
"C:\Program Files (x86)\Microsoft Visual Studio\2019\Enterprise\Common7\Tools\VsMSBuildCmd.bat"

set CMAKE_PREFIX_PATH=.\libs\hwloc;.\libs\libmicrohttpd;.\libs\openssl

cmake .

cmake --build . --config Release --target install

cd bin\Release

copy ..\..\libs\openssl\bin\* .
```


## Ubuntu 编译

```
sudo apt install libmicrohttpd-dev libssl-dev cmake build-essential libhwloc-dev ocl-icd-opencl-dev

unzip xmr-stak-xmr-stak-rx.zip
mkdir xmr-stak-xmr-stak-rx/build
cd xmr-stak-xmr-stak-rx/build

cmake ..
make install
```
