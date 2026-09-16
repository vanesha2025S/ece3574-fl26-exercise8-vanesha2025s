cmake_minimum_required(VERSION 3.16)
project(Exercise8 CXX)

set(CMAKE_AUTOMOC ON)
set(CMAKE_INCLUDE_CURRENT_DIR ON)

# Find Qt6 Widgets module automatically
find_package(Qt6Widgets REQUIRED)

# Add your executable and sources
add_executable(hello_static hello_static.cpp)

# Link Qt6 Widgets
target_link_libraries(hello_static Qt6::Widgets)
