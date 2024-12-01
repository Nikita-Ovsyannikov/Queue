set(target ${QUEUE_TESTS})

file(GLOB QUEUE_HEADERS "*.h*")
file(GLOB QUEUE_SOURCES "*.cpp")

add_executable(${target} ${QUEUE_SOURCES} ${QUEUE_HEADERS})
target_link_libraries(${target} gtest)
target_include_directories(${target} PUBLIC ${CMAKE_SOURCE_DIR}/gtest ${QUEUE_INCLUDE})
add_test(${target} ${target})