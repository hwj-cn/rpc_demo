cmake_minimum_required(VERSION 3.20)
project(rpc_demo LANGUAGES CXX)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 包含目录
include_directories(
    ${CMAKE_CURRENT_SOURCE_DIR}/include
    ${CMAKE_CURRENT_SOURCE_DIR}/third_party
)

# 添加主库
# add_library(rpc_lib STATIC
    # src/rpc_server.cpp
    # src/rpc_client.cpp
    # src/rpc_common.cpp
# )

# 添加可执行文件
# add_executable(rpc_demo src/main.cpp)
# target_link_libraries(rpc_demo rpc_lib)

# 启用测试
# enable_testing()

# 添加子目录
add_subdirectory(test/spdlog)
