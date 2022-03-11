cmake_minimum_required(VERSION 3.12...3.15)
project(test-cmake-findpython)

cmake_policy(GET CMP0094 _CMP0094)
message(STATUS "CMP0094: ${_CMP0094}")
message(STATUS "Python_FIND_STRATEGY: ${Python_FIND_STRATEGY}")
message(STATUS "Python_ROOT_DIR: ${Python_ROOT_DIR}")

find_package(Python 3.6 COMPONENTS Interpreter Development REQUIRED)
