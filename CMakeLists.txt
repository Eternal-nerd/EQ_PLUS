cmake_minimum_required(VERSION 3.5)
project(EQ_PLUS)

# set standard:
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# add source files:
set(SOURCES
	src/main.cpp
)

# add headers
set(HEADERS
)

# add executable:
add_executable(EQ_PLUS ${SOURCES} ${HEADERS})

# add libs
#target_link_libraries(EQ_PLUS PRIVATE Vulkan::Vulkan SDL3::SDL3)

# Specify the output directory for the binary
set_target_properties(EQ_PLUS PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/bin)