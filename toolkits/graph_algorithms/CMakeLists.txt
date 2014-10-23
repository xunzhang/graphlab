project(Djikstra)
add_graphlab_executable(djikstra djikstra.cpp)
add_graphlab_executable(prestige prestige.cpp)
add_graphlab_executable(betweeness betweeness.cpp)
add_graphlab_executable(closeness closeness.cpp)

install(TARGETS
        djikstra
        prestige
        betweeness
        closeness
        RUNTIME DESTINATION bin/graphlab)
