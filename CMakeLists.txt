cmake_minimum_required(VERSION  3.25.2)

project(app) 
find_package(
    ZLIB REQUIRED 
)


add_executable(${PROJECT_NAME} src/main.cpp)
target_link_libraries(${PROJECT_NAME} 
    ZLIB::ZLIB 
)