# NOTE: this CMakeLists does not exist in the upstream repository and therefore only contains what's strictly necessary
#       to compile for usage with InSimo projects.
cmake_minimum_required(VERSION 3.14)

add_library(imoguizmo INTERFACE
    imoguizmo.hpp
)

target_include_directories(imoguizmo INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(imoguizmo INTERFACE imgui)
