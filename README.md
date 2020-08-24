# GoogleTest-Demo

## 概述
本工程引用的是编译好的gtest静态库，其中包括linux-X86版本和linux-arm版本

## 使用说明
### 编译命令
- x86-linux
    - ***mkdir build ; cd build;***
    - ***cmake .. -DCMAKE_TOOLCHAIN_FILE=../cmake/wxh_x86.cmake***
    - ***make***
- arm-linux
    - ***mkdir build_arm ; cd build_arm;***
    - ***cmake .. -DCMAKE_TOOLCHAIN_FILE=../cmake/wxh_arm.cmake***
    ***make -j2***