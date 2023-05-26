cmake_minimum_required(VERSION 3.1)

set(PROJECT_NAME "test_ddmo")
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR})


include_directories(${PROJECT_SOURCE_DIR}/include)

link_directories(${PROJECT_SOURCE_DIR}/lib)

add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME}  libprintX.so)