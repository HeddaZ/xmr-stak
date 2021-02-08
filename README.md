### CMake

```
"C:\Program Files (x86)\Microsoft Visual Studio\2019\Enterprise\Common7\Tools\VsMSBuildCmd.bat"

set CMAKE_PREFIX_PATH=.\libs\hwloc;.\libs\libmicrohttpd;.\libs\openssl

cmake .

cmake --build . --config Release --target install

cd bin\Release

copy ..\..\libs\openssl\bin\* .
```