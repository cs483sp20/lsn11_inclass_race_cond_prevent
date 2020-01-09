cmake_minimum_required(VERSION 3.3)
project(Lsn12_Example_race_cond_prevent)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Werror")

set(SOURCE_FILES main.c)
add_executable(race_cond_prevent ${SOURCE_FILES})
target_link_libraries(race_cond_prevent pthread)
