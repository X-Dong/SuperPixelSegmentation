INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR})

add_library(libSLIC SLIC.cpp)

ADD_EXECUTABLE(SLICSegmentationExample SLICSegmentationExample.cpp ../Helpers.cpp)
TARGET_LINK_LIBRARIES(SLICSegmentationExample ${ITK_LIBRARIES} libSLIC)
