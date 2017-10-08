cmake_minimum_required(VERSION 2.6)
#myapp:main.o 
PROJECT(myapp)
#导入头文件
INCLUDE_DIRECTORIES(
include
)
#指定源文件的目录
AUX_SOURCE_DIRECTORY(src DIR_SRCS)
#把可执行的文件放大哪个目录下  SET  方法设置变量
SET(TEST_MATH ${DIR_SRCS})
ADD_EXECUTABLE(${PROJECT_NAME} ${TEST_MATH})

