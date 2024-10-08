cmake_minimum_required(VERSION 3.25)
project(30dayMakeCppServer)

set(CMAKE_CXX_STANDARD 14)

include_directories(code/day02)
include_directories(code/day03)
include_directories(code/day04)
include_directories(code/day05)
include_directories(code/day06/src)
include_directories(code/day07/src)
include_directories(code/day08/src)
include_directories(code/day09/src)
include_directories(code/day10/src)
include_directories(code/day11/src)
include_directories(code/day12/src)
include_directories(code/day13/src/include)
include_directories(code/day14/src/include)
include_directories(code/day15/src/include)
include_directories(code/day16/src/include)

add_executable(30dayMakeCppServer_day01_client
        code/day01/client.cpp
)
add_executable(30dayMakeCppServer_day01_server
        code/day01/server.cpp
)
add_executable(30dayMakeCppServer_day02_client
        code/day02/client.cpp
        code/day02/util.cpp
)
add_executable(30dayMakeCppServer_day02_server
        code/day02/server.cpp
        code/day02/util.cpp
)
#        code/day03/client.cpp
#        code/day03/server.cpp
#        code/day03/util.cpp
#        code/day03/util.h
#        code/day04/client.cpp
#        code/day04/Epoll.cpp
#        code/day04/Epoll.h
#        code/day04/InetAddress.cpp
#        code/day04/InetAddress.h
#        code/day04/server.cpp
#        code/day04/Socket.cpp
#        code/day04/Socket.h
#        code/day04/util.cpp
#        code/day04/util.h
#        code/day05/Channel.cpp
#        code/day05/Channel.h
#        code/day05/client.cpp
#        code/day05/Epoll.cpp
#        code/day05/Epoll.h
#        code/day05/InetAddress.cpp
#        code/day05/InetAddress.h
#        code/day05/server.cpp
#        code/day05/Socket.cpp
#        code/day05/Socket.h
#        code/day05/util.cpp
#        code/day05/util.h
#        code/day06/src/Channel.cpp
#        code/day06/src/Channel.h
#        code/day06/src/Epoll.cpp
#        code/day06/src/Epoll.h
#        code/day06/src/EventLoop.cpp
#        code/day06/src/EventLoop.h
#        code/day06/src/InetAddress.cpp
#        code/day06/src/InetAddress.h
#        code/day06/src/Server.cpp
#        code/day06/src/Server.h
#        code/day06/src/Socket.cpp
#        code/day06/src/Socket.h
#        code/day06/src/util.cpp
#        code/day06/src/util.h
#        code/day06/client.cpp
#        code/day06/server.cpp
#        code/day07/src/Acceptor.cpp
#        code/day07/src/Acceptor.h
#        code/day07/src/Channel.cpp
#        code/day07/src/Channel.h
#        code/day07/src/Epoll.cpp
#        code/day07/src/Epoll.h
#        code/day07/src/EventLoop.cpp
#        code/day07/src/EventLoop.h
#        code/day07/src/InetAddress.cpp
#        code/day07/src/InetAddress.h
#        code/day07/src/Server.cpp
#        code/day07/src/Server.h
#        code/day07/src/Socket.cpp
#        code/day07/src/Socket.h
#        code/day07/src/util.cpp
#        code/day07/src/util.h
#        code/day07/client.cpp
#        code/day07/server.cpp
#        code/day08/src/Acceptor.cpp
#        code/day08/src/Acceptor.h
#        code/day08/src/Channel.cpp
#        code/day08/src/Channel.h
#        code/day08/src/Connection.cpp
#        code/day08/src/Connection.h
#        code/day08/src/Epoll.cpp
#        code/day08/src/Epoll.h
#        code/day08/src/EventLoop.cpp
#        code/day08/src/EventLoop.h
#        code/day08/src/InetAddress.cpp
#        code/day08/src/InetAddress.h
#        code/day08/src/Server.cpp
#        code/day08/src/Server.h
#        code/day08/src/Socket.cpp
#        code/day08/src/Socket.h
#        code/day08/src/util.cpp
#        code/day08/src/util.h
#        code/day08/client.cpp
#        code/day08/server.cpp
#        code/day09/src/Acceptor.cpp
#        code/day09/src/Acceptor.h
#        code/day09/src/Buffer.cpp
#        code/day09/src/Buffer.h
#        code/day09/src/Channel.cpp
#        code/day09/src/Channel.h
#        code/day09/src/Connection.cpp
#        code/day09/src/Connection.h
#        code/day09/src/Epoll.cpp
#        code/day09/src/Epoll.h
#        code/day09/src/EventLoop.cpp
#        code/day09/src/EventLoop.h
#        code/day09/src/InetAddress.cpp
#        code/day09/src/InetAddress.h
#        code/day09/src/Server.cpp
#        code/day09/src/Server.h
#        code/day09/src/Socket.cpp
#        code/day09/src/Socket.h
#        code/day09/src/util.cpp
#        code/day09/src/util.h
#        code/day09/client.cpp
#        code/day09/server.cpp
#        code/day10/src/Acceptor.cpp
#        code/day10/src/Acceptor.h
#        code/day10/src/Buffer.cpp
#        code/day10/src/Buffer.h
#        code/day10/src/Channel.cpp
#        code/day10/src/Channel.h
#        code/day10/src/Connection.cpp
#        code/day10/src/Connection.h
#        code/day10/src/Epoll.cpp
#        code/day10/src/Epoll.h
#        code/day10/src/EventLoop.cpp
#        code/day10/src/EventLoop.h
#        code/day10/src/InetAddress.cpp
#        code/day10/src/InetAddress.h
#        code/day10/src/Server.cpp
#        code/day10/src/Server.h
#        code/day10/src/Socket.cpp
#        code/day10/src/Socket.h
#        code/day10/src/ThreadPool.cpp
#        code/day10/src/ThreadPool.h
#        code/day10/src/util.cpp
#        code/day10/src/util.h
#        code/day10/client.cpp
#        code/day10/server.cpp
#        code/day10/ThreadPoolTest.cpp
#        code/day11/src/Acceptor.cpp
#        code/day11/src/Acceptor.h
#        code/day11/src/Buffer.cpp
#        code/day11/src/Buffer.h
#        code/day11/src/Channel.cpp
#        code/day11/src/Channel.h
#        code/day11/src/Connection.cpp
#        code/day11/src/Connection.h
#        code/day11/src/Epoll.cpp
#        code/day11/src/Epoll.h
#        code/day11/src/EventLoop.cpp
#        code/day11/src/EventLoop.h
#        code/day11/src/InetAddress.cpp
#        code/day11/src/InetAddress.h
#        code/day11/src/Server.cpp
#        code/day11/src/Server.h
#        code/day11/src/Socket.cpp
#        code/day11/src/Socket.h
#        code/day11/src/ThreadPool.cpp
#        code/day11/src/ThreadPool.h
#        code/day11/src/util.cpp
#        code/day11/src/util.h
#        code/day11/client.cpp
#        code/day11/server.cpp
#        code/day11/test.cpp
#        code/day11/ThreadPoolTest.cpp
#        code/day12/src/Acceptor.cpp
#        code/day12/src/Acceptor.h
#        code/day12/src/Buffer.cpp
#        code/day12/src/Buffer.h
#        code/day12/src/Channel.cpp
#        code/day12/src/Channel.h
#        code/day12/src/Connection.cpp
#        code/day12/src/Connection.h
#        code/day12/src/Epoll.cpp
#        code/day12/src/Epoll.h
#        code/day12/src/EventLoop.cpp
#        code/day12/src/EventLoop.h
#        code/day12/src/Server.cpp
#        code/day12/src/Server.h
#        code/day12/src/Socket.cpp
#        code/day12/src/Socket.h
#        code/day12/src/ThreadPool.cpp
#        code/day12/src/ThreadPool.h
#        code/day12/src/util.cpp
#        code/day12/src/util.h
#        code/day12/client.cpp
#        code/day12/server.cpp
#        code/day12/test.cpp
#        code/day12/ThreadPoolTest.cpp
#        code/day13/src/include/Acceptor.h
#        code/day13/src/include/Buffer.h
#        code/day13/src/include/Channel.h
#        code/day13/src/include/Connection.h
#        code/day13/src/include/Epoll.h
#        code/day13/src/include/EventLoop.h
#        code/day13/src/include/Macros.h
#        code/day13/src/include/Server.h
#        code/day13/src/include/Socket.h
#        code/day13/src/include/ThreadPool.h
#        code/day13/src/include/util.h
#        code/day13/src/Acceptor.cpp
#        code/day13/src/Buffer.cpp
#        code/day13/src/Channel.cpp
#        code/day13/src/Connection.cpp
#        code/day13/src/Epoll.cpp
#        code/day13/src/EventLoop.cpp
#        code/day13/src/Server.cpp
#        code/day13/src/Socket.cpp
#        code/day13/src/ThreadPool.cpp
#        code/day13/src/util.cpp
#        code/day13/test/multiple_client.cpp
#        code/day13/test/server.cpp
#        code/day13/test/single_client.cpp
#        code/day13/test/thread_test.cpp
#        code/day14/src/include/Acceptor.h
#        code/day14/src/include/Buffer.h
#        code/day14/src/include/Channel.h
#        code/day14/src/include/Connection.h
#        code/day14/src/include/Epoll.h
#        code/day14/src/include/EventLoop.h
#        code/day14/src/include/Macros.h
#        code/day14/src/include/Server.h
#        code/day14/src/include/Socket.h
#        code/day14/src/include/ThreadPool.h
#        code/day14/src/include/util.h
#        code/day14/src/Acceptor.cpp
#        code/day14/src/Buffer.cpp
#        code/day14/src/Channel.cpp
#        code/day14/src/Connection.cpp
#        code/day14/src/Epoll.cpp
#        code/day14/src/EventLoop.cpp
#        code/day14/src/Server.cpp
#        code/day14/src/Socket.cpp
#        code/day14/src/ThreadPool.cpp
#        code/day14/src/util.cpp
#        code/day14/test/multiple_client.cpp
#        code/day14/test/server.cpp
#        code/day14/test/single_client.cpp
#        code/day14/test/thread_test.cpp
#        code/day15/src/include/Acceptor.h
#        code/day15/src/include/Buffer.h
#        code/day15/src/include/Channel.h
#        code/day15/src/include/Connection.h
#        code/day15/src/include/EventLoop.h
#        code/day15/src/include/Exception.h
#        code/day15/src/include/Log.h
#        code/day15/src/include/Macros.h
#        code/day15/src/include/pine.h
#        code/day15/src/include/Poller.h
#        code/day15/src/include/Server.h
#        code/day15/src/include/SignalHandler.h
#        code/day15/src/include/Socket.h
#        code/day15/src/include/ThreadPool.h
#        code/day15/src/include/util.h
#        code/day15/src/Acceptor.cpp
#        code/day15/src/Buffer.cpp
#        code/day15/src/Channel.cpp
#        code/day15/src/Connection.cpp
#        code/day15/src/EventLoop.cpp
#        code/day15/src/Poller.cpp
#        code/day15/src/Server.cpp
#        code/day15/src/Socket.cpp
#        code/day15/src/ThreadPool.cpp
#        code/day15/src/util.cpp
#        code/day15/test/chat_client.cpp
#        code/day15/test/chat_server.cpp
#        code/day15/test/echo_client.cpp
#        code/day15/test/echo_clients.cpp
#        code/day15/test/echo_server.cpp
#        code/day15/test/http_server.cpp
#        code/day16/src/include/Acceptor.h
#        code/day16/src/include/Buffer.h
#        code/day16/src/include/Channel.h
#        code/day16/src/include/common.h
#        code/day16/src/include/Connection.h
#        code/day16/src/include/EventLoop.h
#        code/day16/src/include/Exception.h
#        code/day16/src/include/Log.h
#        code/day16/src/include/pine.h
#        code/day16/src/include/Poller.h
#        code/day16/src/include/SignalHandler.h
#        code/day16/src/include/Socket.h
#        code/day16/src/include/TcpServer.h
#        code/day16/src/include/ThreadPool.h
#        code/day16/src/Acceptor.cpp
#        code/day16/src/Buffer.cpp
#        code/day16/src/Channel.cpp
#        code/day16/src/Connection.cpp
#        code/day16/src/EventLoop.cpp
#        code/day16/src/Poller.cpp
#        code/day16/src/Socket.cpp
#        code/day16/src/TcpServer.cpp
#        code/day16/src/ThreadPool.cpp
#        code/day16/test/chat_client.cpp
#        code/day16/test/chat_server.cpp
#        code/day16/test/echo_client.cpp
#        code/day16/test/echo_clients.cpp
#        code/day16/test/echo_server.cpp
#        code/day16/test/http_server.cpp)
