
# CMakeLists.txt 的语法比较简单,由命令、注释和空格组成,其中命令是不区分大小写的,符号"#"后面的内容被认为是注释。
# 命令由命令名称、小括号和参数组成,参数之间使用空格进行间隔

# 项目的名称是 main
PROJECT(main)

# 限定了 CMake 的版本
CMAKE_MINIMUM_REQUIRED(VERSION 3.4.1)

# AUX_SOURCE_DIRECTORY 将当前目录中的源文件名称赋值给变量 DIR_SRCS
AUX_SOURCE_DIRECTORY(. DIR_SRCS)

# 指示变量 DIR_SRCS 中的源文件需要编译 成一个名称为 main 的可执行文件
ADD_EXECUTABLE(main ${DIR_SRCS})
