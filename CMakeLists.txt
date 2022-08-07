cmake_minimum_required(VERSION 3.21)

set(CMAKE_CXX_STANDARD 20)

project(ModelViewer)

add_executable(model-viewer
    main.cpp
)

include_directories(include)

target_link_libraries(model-viewer
PUBLIC
    opengl32
    ${CMAKE_SOURCE_DIR}/libs/glfw3.lib
    ${CMAKE_SOURCE_DIR}/libs/assimp-vc142-mtd.lib
    ${CMAKE_SOURCE_DIR}/libs/imgui.lib     
)
