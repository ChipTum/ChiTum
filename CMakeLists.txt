cmake_minimum_required(VERSION 3.5)

project(ChipTum VERSION 0.0.1)

# Samples
add_subdirectory(samples)

# Testing
enable_testing()
add_subdirectory(test)

# Benchmarks
add_subdirectory(bench)