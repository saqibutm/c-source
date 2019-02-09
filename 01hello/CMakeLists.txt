cmake_minimum_required(VERSION 3.13)
project(01hello C)

set(CMAKE_C_STANDARD 11)

# add extra include directories
include_directories(/usr/local/include)


# add extra lib directories
link_directories(/usr/local/lib)


# specify the executable (no libraries here)
add_executable(01hello main.c)


# specify the dependency on an extra library
target_link_libraries(01hello libcs50.a)