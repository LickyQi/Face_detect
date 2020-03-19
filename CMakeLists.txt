cmake_minimum_required(VERSION 3.14)
project(facedetecte)

set(CMAKE_CXX_STANDARD 11)

#添加头文件搜索路径
include_directories(/usr/local/include)

#添加库文件搜索路径
link_directories(/usr/local/lib)

add_executable(facedetecte main.cpp)

#添加Opencv库
target_link_libraries(facedetecte opencv_world)