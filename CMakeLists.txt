cmake_minimum_required(VERSION 3.0.0)
project(flappybird VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(flappybird main.cpp)
target_link_libraries(flappybird SDL2main SDL2 SDL2_image)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
