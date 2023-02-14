project(CuckoFilter)

cmake_minimum_required(VERSION 2.4)

set(CMAKE_BUILD_TYPE Release)

add_library(CuckooFiltSupport
            bitsutil.h
            cuckoofilter.h
            debug.h
            hashutil.h
            hashutil.cc     
            packedtable.h
            permencoding.h
            printutil.h
            simd-block.h
            singletable.h
        )


target_include_directories(CuckooFiltSupport PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

# target_link_libraries(
#     CuckoFilter
#     CuckoFiltSupport
# )
