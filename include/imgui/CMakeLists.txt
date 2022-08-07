cmake_minimum_required(VERSION 3.21)

add_library(imgui
STATIC
    imgui_demo.cpp
    imgui_draw.cpp
    imgui_tables.cpp
    imgui_widgets.cpp
    imgui.cpp
    imgui_impl_glfw.cpp
    imgui_impl_opengl3.cpp
)

target_link_libraries(imgui
opengl32
)

target_include_directories(imgui
PUBLIC
    .
)