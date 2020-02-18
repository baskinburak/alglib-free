project(alglibfree)
cmake_minimum_required(VERSION 3.0.0 FATAL_ERROR)

file(GLOB alglib_files "src/*.cpp")

add_library(
  alglib-free
  ${alglib_files}
)

target_include_directories(
  alglib-free
  PUBLIC
  src
)