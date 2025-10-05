cmake_minimum_required(VERSION 3.20)
project(concertc LANGUAGES C)

if (MSVC)
    add_compile_options(/W4 /Ox)
else()
    add_compile_options(-Wall -Wextra -Wpedantic -O2)
endif()

add_executable(concertc concertc.c)

install(TARGETS concertc
 RUNTIME DESTINATION bin)
