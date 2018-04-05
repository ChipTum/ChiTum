# Define target name
set(TARGET_NAME 01_HelloWorld)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

add_compile_options(-std=c++17)

add_executable(${TARGET_NAME} HelloWorld.cpp)
target_link_libraries(${TARGET_NAME} ${SDL2_LIBRARIES})