add_library(imgui)
target_include_directories(imgui PUBLIC . backends)
target_sources(imgui PUBLIC
  imgui.cpp
  imgui_demo.cpp
  imgui_draw.cpp
  imgui_tables.cpp
  imgui_widgets.cpp
  backends/imgui_impl_glfw.cpp
  backends/imgui_impl_opengl3.cpp
)
target_link_libraries(imgui PUBLIC glfw)