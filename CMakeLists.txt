cmake_minimum_required(VERSION 3.0)

project(FakeItUsageExample)

find_package(FakeIt REQUIRED)

add_executable(FakeItUsageExample
    FakeItUsageExample.cpp
)
target_link_libraries(FakeItUsageExample
    PRIVATE
        FakeIt::FakeIt
)
