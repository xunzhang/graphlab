project(GraphLab)

# Primary executable
add_graphlab_executable(lda_sequential_cgs lda_sequential_cgs.cpp)
add_graphlab_executable(cgs_lda cgs_lda.cpp)
add_graphlab_executable(cgs_lda_mimno_experimental cgs_lda_mimno_experimental.cpp)

install(TARGETS
        lda_sequential_cgs
        cgs_lda
        cgs_lda_mimno_experimental
        RUNTIME DESTINATION bin/graphlab)
