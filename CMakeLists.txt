cmake_minimum_required(VERSION 3.0.0)

# Change project name to the desired executable name!
project(cpp-vs-proj-template VERSION 0.1.0)

aux_source_directory(src SOURCES)
set(CMAKE_CXX_STANDARD 17)
include(CTest)
enable_testing()

add_executable(${PROJECT_NAME} ${SOURCES})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
