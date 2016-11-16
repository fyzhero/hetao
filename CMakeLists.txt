project (hetao)

set (cmake_build_type Debug)

set (src_path ./src)
set (src_list ${src_path}/main.cpp)
set (boost_path /Users/fanyizhong/software/boost_1_60_0/)

include_directories(${boost_path})

add_executable(./bin/hetaod ${src_list})
target_link_libraries(./bin/hetaod pthread stdc++)
