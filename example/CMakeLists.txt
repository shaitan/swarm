if(BUILD_URLFETCHER)
#	add_executable(crawler crawler.cpp)
#	target_link_libraries(crawler swarm ev)
	add_executable(download download.cpp)
	target_link_libraries(download swarm swarm_urlfetcher ev)
	add_executable(url_test url_test.cpp)
	target_link_libraries(url_test swarm)
endif()

add_subdirectory(elliptics)
