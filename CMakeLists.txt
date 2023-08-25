cmake_minimum_required(VERSION 3.27 FATAL_ERROR)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

project(
  esms
  VERSION
    2.7.3
  LANGUAGES
    CXX
)

add_subdirectory(src)
