# Define target name
set(TARGET_NAME 01_HelloWorld)

add_compile_options(-std=c++17)

add_executable(${TARGET_NAME} HelloWorld.cpp)