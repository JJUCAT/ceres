cmake_minimum_required(VERSION 2.8)
project(ceres)

find_package(Ceres REQUIRED)
include_directories(${CERES_INCLUDE_DIRS})

add_executable(main src/main.cc)
target_link_libraries(main ${CERES_LIBRARIES})
