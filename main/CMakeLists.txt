cmake_minimum_required(VERSION 3.14)
project(main)

set(CMAKE_CXX_STANDARD 17)

include_directories(${CMAKE_SOURCE_DIR}/osm/)

add_executable(compare_vector ${UTILITY_SOURCE_FILES} compare_vector.cpp)
target_link_libraries(compare_vector osm module pthread z)

add_executable(compute_contraction_hierarchy ${UTILITY_SOURCE_FILES} compute_contraction_hierarchy.cpp)
target_link_libraries(compute_contraction_hierarchy osm module pthread z)

add_executable(compute_geographic_distance_weights ${UTILITY_SOURCE_FILES} compute_geographic_distance_weights.cpp)
target_link_libraries(compute_geographic_distance_weights osm module pthread z)

add_executable(compute_nested_dissection_order ${UTILITY_SOURCE_FILES} compute_nested_dissection_order.cpp)
target_link_libraries(compute_nested_dissection_order osm module pthread z)

add_executable(convert_road_dimacs_coordinates ${UTILITY_SOURCE_FILES} convert_road_dimacs_coordinates.cpp)
target_link_libraries(convert_road_dimacs_coordinates osm module pthread z)

add_executable(convert_road_dimacs_graph ${UTILITY_SOURCE_FILES} convert_road_dimacs_graph.cpp)
target_link_libraries(convert_road_dimacs_graph osm module pthread z)

add_executable(decode_vector ${UTILITY_SOURCE_FILES} decode_vector.cpp)
target_link_libraries(decode_vector osm module pthread z)

add_executable(encode_vector ${UTILITY_SOURCE_FILES} encode_vector.cpp)
target_link_libraries(encode_vector osm module pthread z)

add_executable(examine_ch ${UTILITY_SOURCE_FILES} examine_ch.cpp)
target_link_libraries(examine_ch osm module pthread z)

add_executable(export_road_dimacs_graph ${UTILITY_SOURCE_FILES} export_road_dimacs_graph.cpp)
target_link_libraries(export_road_dimacs_graph osm module pthread z)

add_executable(generate_constant_vector ${UTILITY_SOURCE_FILES} generate_constant_vector.cpp)
target_link_libraries(generate_constant_vector osm module pthread z)

add_executable(generate_dijkstra_rank_test_queries ${UTILITY_SOURCE_FILES} generate_dijkstra_rank_test_queries.cpp)
target_link_libraries(generate_dijkstra_rank_test_queries osm module pthread z)

add_executable(generate_random_node_list ${UTILITY_SOURCE_FILES} generate_random_node_list.cpp)
target_link_libraries(generate_random_node_list osm module pthread z)

add_executable(generate_random_source_times ${UTILITY_SOURCE_FILES} generate_random_source_times.cpp)
target_link_libraries(generate_random_source_times osm module pthread z)

add_executable(generate_test_queries ${UTILITY_SOURCE_FILES} generate_test_queries.cpp)
target_link_libraries(generate_test_queries osm module pthread z)

add_executable(graph_to_dot ${UTILITY_SOURCE_FILES} graph_to_dot.cpp)
target_link_libraries(graph_to_dot osm module pthread z)

add_executable(graph_to_svg ${UTILITY_SOURCE_FILES} graph_to_svg.cpp)
target_link_libraries(graph_to_svg osm module pthread z)

add_executable(osm_extract ${UTILITY_SOURCE_FILES} osm_extract.cpp)
target_link_libraries(osm_extract osm module pthread z)

add_executable(randomly_permute_nodes ${UTILITY_SOURCE_FILES} randomly_permute_nodes.cpp)
target_link_libraries(randomly_permute_nodes osm module pthread z)

add_executable(run_contraction_hierarchy_query ${UTILITY_SOURCE_FILES} run_contraction_hierarchy_query.cpp)
target_link_libraries(run_contraction_hierarchy_query osm module pthread z)

add_executable(run_dijkstra ${UTILITY_SOURCE_FILES} run_dijkstra.cpp)
target_link_libraries(run_dijkstra osm module pthread z)

add_executable(show_path ${UTILITY_SOURCE_FILES} show_path.cpp)
target_link_libraries(show_path osm module pthread z)
