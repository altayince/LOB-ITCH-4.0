cmake_minimum_required(VERSION 3.12)
project(itch_order_book_master)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)

add_executable(prog
        bufferedreader.cpp
        bufferedreader.h
        itch.h
        main.cpp
        order_book.h
        types.h)
