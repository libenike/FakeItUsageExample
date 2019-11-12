cmake_minimum_required(VERSION 3.15.1)

project(FakeItUsageExample)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

find_package(FakeIt REQUIRED)

add_executable(FakeItUsageExample
    FakeItUsageExample.cpp
)
target_link_libraries(FakeItUsageExample
    PRIVATE
        FakeIt::FakeIt
)
