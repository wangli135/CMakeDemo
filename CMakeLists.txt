cmake_minimum_required (VERSION 2.8)
project (Demo3)

# 查找当前目录下的所有源文件
aux_source_directory (. DIR_SRCS)

# 添加子目录
add_subdirectory(math)

# 指定生成目标
add_executable(Demo main.cpp)

# 添加链接库  
target_link_libraries(Demo MathFunctions)
