cmake_minimum_required(VERSION 3.7.0)
project(opencv VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

find_package(OpenCV REQUIRED)
message("OpenCV = ${OpenCV_INCLUDE_DIRS}")


add_executable(opencv main.cpp)
target_include_directories(opencv PRIVATE ${OpenCV_INCLUDE_DIRS})
target_link_libraries(opencv ${OpenCV_LIBS})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
