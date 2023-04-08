cmake_minimum_required(VERSION 3.20)
project(03_basicFramework LANGUAGES CXX CUDA)

enable_language(CUDA)

add_executable(${PROJECT_NAME} add1.cu)

find_package(CUDA  REQUIRED)
include_directories("${CUDA_INCLUDE_DIRS}")