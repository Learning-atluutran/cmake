add_subdirectory(lib1)
add_executable(myTest main.cpp)
target_link_libraries(myTest PUBLIC lib1)
target_include_directories(myTest PUBLIC
				"${PROJECT_BINARY_DIR}"
				"${PROJECT_SOURCE_DIR}/lib1"
)
