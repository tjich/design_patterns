cmake_minimum_required(VERSION 3.0)
project(design_patterns LANGUAGES CXX C)
set(CMAKE_CXX_STANDARD 17)
set(SRC_DIR ${CMAKE_SOURCE_DIR}/cpp_lang)

function(add_langs filename)
add_executable(${filename} ${SRC_DIR}/${filename}.cpp)
endfunction()

add_langs(cpp_lang01)
add_langs(cpp_lang02)
add_langs(cpp_lang03)
add_langs(cpp_lang04)
add_langs(cpp_lang05)