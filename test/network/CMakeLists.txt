# 网络测试配置
add_executable(network_test network_test.cpp)

# 链接主库和网络相关依赖
target_link_libraries(network_test
    rpc_lib
    pthread
)

# 添加测试
add_test(NAME network_test COMMAND network_test)
