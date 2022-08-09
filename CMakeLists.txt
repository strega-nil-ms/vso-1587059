cmake_minimum_required(VERSION 3.22)

include("${CMAKE_CURRENT_SOURCE_DIR}/vcpkg/scripts/buildsystems/vcpkg.cmake")
project(testproj CXX)

set(CMAKE_CXX_STANDARD 23)

find_package(fmt REQUIRED)

add_executable(main main.cxx)
target_link_libraries(main fmt::fmt)
