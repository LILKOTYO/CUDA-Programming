cmake_minimum_required(VERSION 3.20)
project(02_threadOrganization LANGUAGES CXX CUDA)

enable_language(CUDA)

add_executable(${PROJECT_NAME} hello3.cu)

find_package(CUDA  REQUIRED)
include_directories("${CUDA_INCLUDE_DIRS}")