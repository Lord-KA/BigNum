cmake_minimum_required(VERSION 3.14)
project(ULInt)


add_executable(ulint test-ulint.cpp ../ulint.cpp ../ulint.hpp)

target_link_libraries(
    ulint
    gtest_main
)


include(GoogleTest)
gtest_discover_tests(ulint)
