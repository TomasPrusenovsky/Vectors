cmake_minimum_required(VERSION 3.26)
project(Vectors)
set(CMAKE_CXX_STANDARD 23)

add_subdirectory(dependencies/GLFW)
add_subdirectory(dependencies/glad)
add_subdirectory(dependencies/ImGui)


include_directories(
        dependencies/GLFW/include
        dependencies/glad/include
        dependencies/ImGui
        dependencies/ImGui/backends
)

add_executable(Vectors main.cpp)

target_link_libraries(Vectors PRIVATE glfw)
target_link_libraries(Vectors PRIVATE glad)
target_link_libraries(Vectors PRIVATE ImGui)


