# RPC 核心功能测试配置
add_executable(rpc_test rpc_test.cpp)

# 链接主库和可能的序列化库
target_link_libraries(rpc_test
    rpc_lib
)

# 添加测试
add_test(NAME rpc_test COMMAND rpc_test)
