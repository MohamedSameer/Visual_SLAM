cmake_minimum_required(VERSION 2.8)
project(useEigen)

#set(CMAKE_BUILD_TYPE "Release")
#set(CMAKE_CXX_FLAGS "-O3")

# 添加Eigen头文件

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

include_directories("/usr/include/eigen3")


# or
# find_package(Eigen3 REQUIRED)
# target_link_libraries(your_target PRIVATE Eigen3::Eigen)

add_executable(eigenMatrix eigenMatrix.cpp)


