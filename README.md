# cmake-cygwin

## How to compile cmake 3.10.3
* Install cygwin on Windows
  * During setup make sure to include the following packages
    * curl
    * gcc-g++
    * libcurl-devel
    * libncurses++w10
    * libncurses-devel
    * make
    * wget
    * zlib
    * zlib-devel
* Open a cygwin terminal and type the following commands
   <pre><code>
    wget https://cmake.org/files/v3.10/cmake-3.10.3.tar.gz
    tar -xzf cmake-3.10.3.tar.gz
    cd cmake-3.10.3
    ./configure --no-system-libs
    make all
    make install
   </code></pre>

Source: https://egoboo.org/build-from-source/windows-10-cygwin/how-to-install-a-more-recent-cmake-version-on-cygwin/

The only issue with this build is that it is creating unexpected folders with emoji in the name. Those folders will appears where the cmake.exe file is located as well as in the temporary folder cmake creates during builds
