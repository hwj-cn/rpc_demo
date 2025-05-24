cmake_minimum_required(VERSION 3.20)

# spdlog 测试配置
add_executable(spdlog_test spdlog_test.cpp)

include(FetchContent)
FetchContent_Declare(
      spdlog
      GIT_REPOSITORY https://github.com/gabime/spdlog.git
      GIT_TAG v1.11.0
)
# Download spdlog
FetchContent_MakeAvailable(spdlog)

target_link_libraries(spdlog_test PUBLIC spdlog::spdlog)