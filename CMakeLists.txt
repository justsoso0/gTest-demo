project(IO)

SET( CMAKE_CXX_FLAGS "-std=c++11")


include_directories(${CMAKE_HOME_DIRECTORY}/depend/libgtest/include)

if(${CMAKE_USR_OS} EQUAL 0)
    link_directories(${CMAKE_HOME_DIRECTORY}/depend/libgtest/linux_os_x86)
    message(STATUS "IN <OS-LINUX X86>")
elseif(${CMAKE_USR_OS} EQUAL 1)
    link_directories(${CMAKE_HOME_DIRECTORY}/depend/libgtest/linux_os_arm)
    message(STATUS "IN <OS-ARM-LINUX>")
endif()


add_executable(main main.cpp)
target_link_libraries(main gtest pthread)











