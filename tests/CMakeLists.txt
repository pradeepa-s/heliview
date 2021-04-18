cmake_minimum_required(VERSION 3.10)

# set the project name
project(heliview_test)

# add the executable
add_subdirectory("${PROJECT_SOURCE_DIR}/../submodules/googletest" gtest)

add_executable(heliview_test sample_test.cpp)

target_link_libraries(heliview_test PUBLIC gtest_main)
