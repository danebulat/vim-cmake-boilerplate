# lib/interp/CMakeLists.txt
# Compile shared library from source files
add_library(interp interpolate.cpp)

# State that any target linking to this library can see 
# the passed source directories
target_include_directories(interp
    INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
