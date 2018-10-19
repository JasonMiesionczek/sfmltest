cmake_minimum_required(VERSION 3.0.0)
project(sfml VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(sfml main.cpp)
target_link_libraries(sfml sfml-graphics sfml-window sfml-system)
set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
