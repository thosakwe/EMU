cmake_minimum_required(VERSION 2.8)
set(CMAKE_CXX_STANDARD 11)
add_subdirectory(asm)
add_subdirectory(vm)
add_executable(emu main.cpp)
target_link_libraries(emu asm vm)