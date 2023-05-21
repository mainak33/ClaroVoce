cmake_minimum_required(VERSION 3.16)

# Project name and a few useful settings. Other commands can pick up the results
project(
  CppwPy
  VERSION 0.0.1)

add_executable(CppwPy main.cpp)

set(CMAKE_PREFIX_PATH "${CMAKE_SOURCE_DIR}/../install")
find_package(PythonLibs REQUIRED)
include_directories(${PYTHON_INCLUDE_DIRS})
target_link_libraries(CppwPy ${PYTHON_LIBRARIES})
