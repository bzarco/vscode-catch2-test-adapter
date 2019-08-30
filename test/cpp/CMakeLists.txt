cmake_minimum_required(VERSION 3.10)

set(CMAKE_BUILD_TYPE Debug)

project(Tests)

#

include("GoogleTest.cmake")
add_gtest_with_main(gtest1 "gtest1.cpp")

#

include("Catch2Test.cmake")

add_catch2test_with_main(suite1 "suite1.cpp")
add_catch2test_with_main(suite2 "suite2.cpp")
add_catch2test_with_main(suite3 "suite3.cpp")