cmake_minimum_required(VERSION 3.10)
project(chat_server_client)

set(CMAKE_CXX_STANDARD 14)

# 添加可执行文件
add_executable(chat_server chat_server.cpp)
target_link_libraries(chat_server -lpthread -lboost_system -lboost_thread -lboost_chrono -lboost_date_time)

add_executable(chat_client chat_client.cpp)
target_link_libraries(chat_client -lpthread -lboost_system -lboost_thread -lboost_chrono -lboost_date_time)

