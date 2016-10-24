# quantlib-conan-example
Usage example of QuantLib with Conan.io package manager

Just follow these steps (see [Getting started guide](http://docs.conan.io/en/latest/getting_started.html)):

 #. Clone the repository

  ```
  git clone https://github.com/jgsogo/quantlib-conan-example.git quantlib-conan-example
  ```

 #. Create a directory to build the example out-of-source

  ```
  cd quantlib-conan-example
  mkdir build && cd build
  ```

 #. Install all dependencies using [conan.io](https://conan.io). This will grab already existing packages from conan server or build them if missing.

  ```
  conan install .. --build=missing
  ```

 #. Build and run the example as usual with CMake

  ```
  # (Linux, mac)
  $ cmake .. -G "Unix Makefiles" -DCMAKE_BUILD_TYPE=Release
  $ cmake --build .
  ```


