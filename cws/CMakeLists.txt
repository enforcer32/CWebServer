file(GLOB_RECURSE CWSSources
	"${CMAKE_CURRENT_SOURCE_DIR}/cws.C"
)

add_definitions(-DCWS_DEBUG)

add_executable(${CWS_TARGET_NAME} ${CWSSources})
target_include_directories(${CWS_TARGET_NAME} PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}/../")
