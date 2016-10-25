project(QuantLibExample)
cmake_minimum_required(VERSION 2.8.12)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

find_package(QuantLib)

include_directories(${QuantLib_INCLUDE_DIRS})
add_executable(ex-quantlib main.cpp)
target_link_libraries(ex-quantlib ${QuantLib_LIBS})

