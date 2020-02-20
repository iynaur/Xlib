cmake_minimum_required(VERSION 3.1.0)
project(HelicopterGame)

set(CMAKE_CXX_STANDARD 14)

file(GLOB_RECURSE SRC_LIST  "${PROJECT_SOURCE_DIR}/*.cpp")

set(EXECUTABLE_OUTPUT_PATH "${PROJECT_SOURCE_DIR}")
add_executable(HelicopterGame ${SRC_LIST})
target_link_libraries(HelicopterGame
-lX11 -lpthread
                                    )
