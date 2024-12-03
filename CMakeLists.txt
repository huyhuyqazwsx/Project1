cmake_minimum_required(VERSION 3.15)
project(project-1)

set(CMAKE_CXX_STANDARD 20)

# Tìm thư viện ZLIB
find_package(ZLIB REQUIRED)

# Thêm file nguồn
add_executable(project-1 main.cpp)

# Liên kết thư viện ZLIB
target_link_libraries(project-1 ZLIB::ZLIB)


