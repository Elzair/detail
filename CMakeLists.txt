cmake_minimum_required(VERSION 3.3)

project(boost_detail)

add_library(boost_detail INTERFACE)

target_include_directories(boost_detail BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_detail DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
