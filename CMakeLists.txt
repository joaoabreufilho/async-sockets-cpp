cmake_minimum_required(VERSION 3.16)

add_library(async_sockets STATIC easysocket/include/basesocket.h
        easysocket/include/DllHelper.h
        easysocket/include/tcpserver.h
        easysocket/include/tcpsocket.h
        easysocket/include/udpserver.h
        easysocket/include/udpsocket.h
        easysocket/src/basesocket.cpp
        easysocket/src/tcpserver.cpp
        easysocket/src/tcpsocket.cpp
        easysocket/src/udpserver.cpp
        easysocket/src/udpsocket.cpp)
        
target_include_directories(async_sockets PUBLIC easysocket/include)
