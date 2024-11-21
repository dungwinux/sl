cmake_minimum_required(VERSION 3.23)

project(sl)
set(CMAKE_C_STANDARD 11)

find_package(unofficial-pdcurses CONFIG REQUIRED)

add_executable(sl sl.c)

target_link_libraries(sl PRIVATE unofficial::pdcurses::pdcurses)