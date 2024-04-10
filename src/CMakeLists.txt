
set(IOP_HEADER_FILES
        mpi_io_trace.h
        )

set(IOP_SOURCE_FILES
        mpi_io_trace.c
        )


# set binary path and lib storage path for compiling process.
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib)

add_library(iop_hook STATIC ${IOP_SOURCE_FILES} ${IOP_HEADER_FILES})
target_link_libraries(iop_hook PUBLIC ${EXTRA_LIBS})
