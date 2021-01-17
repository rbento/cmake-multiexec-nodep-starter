cmake_minimum_required (VERSION 3.18)

project ("project-name")

add_definitions(-D_CRT_SECURE_NO_WARNINGS)

file(GLOB SOURCE_FILES *.c)

foreach(SOURCE_PATH ${SOURCE_FILES})

    get_filename_component(EXECUTABLE_NAME ${SOURCE_PATH} NAME_WE)

    add_executable(${EXECUTABLE_NAME} ${SOURCE_PATH})

endforeach(SOURCE_PATH ${SOURCE_FILES})
