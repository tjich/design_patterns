cmake_minimum_required(VERSION 3.0)
project(patterns LANGUAGES CXX C)
set(CMAKE_CXX_STANDARD 17)
set(SRC_DIR ${CMAKE_SOURCE_DIR}/patterns)

function(add_patterns filename)
add_executable(${filename} ${SRC_DIR}/${filename}.cpp)
endfunction()

add_patterns(singleton)
add_patterns(factory)
add_patterns(pimpl)
add_patterns(facade)
add_patterns(templ)
add_patterns(strategy)
add_patterns(table_driven)
add_patterns(chain_of_responsibility)
add_patterns(crtp)
add_patterns(adl)

