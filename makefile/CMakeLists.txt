cmake_minimum_required(VERSION 3.16)

project(
    TEST
    LANGUAGES CXX
)
add_executable(program main.cc bar.cc foo.cc)

target_compile_options(program PUBLIC -Wall -Werror)