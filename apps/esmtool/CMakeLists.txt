set(ESMTOOL
  esmtool.cpp
)
source_group(apps\\esmtool FILES ${ESMTOOL})

# Main executable
add_executable(esmtool
  ${ESMTOOL}
)

target_link_libraries(esmtool
  ${Boost_LIBRARIES}
  components
)

#if (APPLE)
#    find_library(CARBON_FRAMEWORK Carbon)
#    target_link_libraries(openmw ${CARBON_FRAMEWORK})
#endif (APPLE)
