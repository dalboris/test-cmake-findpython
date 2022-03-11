cmake_minimum_required(VERSION 3.12)
cmake_policy(GET CMP0094 _CMP0094)
message(STATUS "Python_FIND_STRATEGY_POLICY: ${_CMP0094}")
message(STATUS "Python_FIND_STRATEGY: ${Python_FIND_STRATEGY}")

project(test-cmake-findpython)

find_package(Python 3.6 COMPONENTS Interpreter Development REQUIRED)
