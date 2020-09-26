cmake_minimum_required (VERSION 3.7.0) 
project(problem_95)

if (UNIX)
else()
  add_definitions(-D_SILENCE_ALL_CXX17_DEPRECATION_WARNINGS -D_WIN32_WINNT=0x0601)
endif()

include_directories("/home/yusuke/source/cpp/src/The-Modern-Cpp-Challenge/libs/asio/include")

add_executable(problem_95 main.cpp)

set_target_properties (problem_95 PROPERTIES FOLDER "12.NetworkingCloud")
set(CMAKE_CXX_FLAGS "-std=c++17 -Wall -pthread")
