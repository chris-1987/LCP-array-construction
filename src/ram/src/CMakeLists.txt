INCLUDE_DIRECTORIES("${CMAKE_CURRENT_BINARY_DIR}")

# add STXXL includes path
INCLUDE_DIRECTORIES("${STXXL_INCLUDE_DIRS}")

#build a executable program
ADD_EXECUTABLE(lcpa_ram lcpa_ram.cpp)
TARGET_LINK_LIBRARIES(lcpa_ram ${STXXL_LIBRARIES})
