add_executable(genre "genre.cpp")
add_executable(measures "measures.cpp")
add_executable(octree_base "octree_base.cpp")

target_link_libraries(genre PRIVATE CGAL)
target_link_libraries(measures PRIVATE CGAL)
target_link_libraries(octree_base PRIVATE CGAL)