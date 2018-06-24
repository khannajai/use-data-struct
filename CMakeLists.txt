cmake_minimum_required(VERSION 3.5.1)

find_package(PkgConfig REQUIRED)
pkg_check_modules(DATASTRUCTURES REQUIRED data-structures-cpp)
include_directories(${DATASTRUCTURES_INCLUDE_DIRS})
add_executable(mytest test-data-struct.cpp)
target_link_libraries(mytest ${DATASTRUCTURES_LIBRARIES})

