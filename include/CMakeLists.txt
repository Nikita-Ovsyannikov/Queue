set(target ${QUEUE_CUSTOM_PROJECT})
project(${target})

file(GLOB QUEUE_HEADERS "*.h*")

add_custom_target(${target} SOURCES ${QUEUE_HEADERS})