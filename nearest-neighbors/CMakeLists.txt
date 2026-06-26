add_library(nearest_neighbors STATIC)

target_sources(nearest_neighbors
    PUBLIC FILE_SET nearest_neighbors_interface
    TYPE CXX_MODULES FILES
    # Full API
        nearest_neighbors.cppm
    # Individual APIs
        point.cppm
)
