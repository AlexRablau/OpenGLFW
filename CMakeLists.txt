cmake_minimum_required (VERSION 3.0)

project(MirageEngine)

add_subdirectory(deps/glfw-3.1.1)

include_directories(include)

add_executable(Main src/main.cpp)

target_link_libraries(Main glfw ${GLFW_LIBRARIES})