FIND_PACKAGE(Boost)

include_directories(
	include/
	${Boost_INCLUDE_DIR}
)



set(SOURCES
	src/HevcParser.cpp
	src/Hevc.cpp
	src/HevcParserImpl.cpp
	src/BitstreamReader.cpp
	src/HevcUtils.cpp
)

add_library(hevcparser ${SOURCES})


