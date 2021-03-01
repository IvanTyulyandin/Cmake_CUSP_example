cmake_minimum_required(VERSION 3.18)
project(Cusp_test)

set(CMAKE_CXX_STANDARD 20)
add_compile_options(-Wall -Wextra -Wpedantic -Werror -Wno-unused-function -Wno-unused-variable)

add_executable(Cusp_test main.cpp)

find_package(OpenMP REQUIRED)
target_link_libraries(Cusp_test OpenMP::OpenMP_CXX)

file(GLOB MTX_FILES ${CMAKE_CURRENT_SOURCE_DIR}/*.mtx)
file(COPY ${MTX_FILES} DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
