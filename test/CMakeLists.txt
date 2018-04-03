set(TARGET_NAME test_sample)

# Configure google test
enable_testing()
find_package(GTest REQUIRED)
include_directories(${GTEST_INCLUDE_DIRS})

GTEST_ADD_TESTS("${TARGET_NAME}" "" test.cpp)

add_compile_options(-std=c++17)
add_executable(${TARGET_NAME} test.cpp)
target_link_libraries(${TARGET_NAME} ${GTEST_BOTH_LIBRARIES} pthread)