# cmake version
cmake_minimum_required(VERSION 3.8)

# --> Set your project name here <--
project(Wizard)                                      

# includes CUTE library
include_directories(cute)                       

# include BOOST (can be commented out if not needed)
set(Boost_INCLUDE_DIR C:/MinGW/include) # --> Change according to your installation <--
set(Boost_LIBRARY_DIR C:/MinGW/lib) # --> Change according to your installation <--
find_package(Boost 1.71.0)
include_directories(${Boost_INCLUDE_DIR})
if(NOT Boost_FOUND)
    message(FATAL_ERROR "Could not find boost!")
endif()

# set C++ Version to 17
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++17") # enable C++17 standard

# set path to all source (.cpp) files. needed for SOURCE_FILES variable
file(GLOB_RECURSE SOURCE_FILES "src/*.cpp")

# creates the executable from the project name and the SOURCE_FILES variable
add_executable(${PROJECT_NAME} ${SOURCE_FILES})            