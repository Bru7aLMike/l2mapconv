cmake_minimum_required(VERSION 3.22)
project(app)

add_executable(${PROJECT_NAME} src/main.cpp)

target_link_libraries(${PROJECT_NAME}
    PRIVATE config

    PRIVATE doctest
    PRIVATE cxxopts
)

set_target_properties(${PROJECT_NAME} PROPERTIES OUTPUT_NAME "vanity")
