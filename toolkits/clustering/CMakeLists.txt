project(GraphProcessing)

add_graphlab_executable(kmeans kmeans.cpp)
add_graphlab_executable(generate_synthetic generate_synthetic.cpp)
add_graphlab_executable(spectral_clustering spectral_clustering.cpp)
add_graphlab_executable(graph_laplacian_for_sc graph_laplacian_for_sc.cpp)

install(TARGETS 
        kmeans 
        generate_synthetic 
        spectral_clustering 
        graph_laplacian_for_sc
        RUNTIME DESTINATION bin)
