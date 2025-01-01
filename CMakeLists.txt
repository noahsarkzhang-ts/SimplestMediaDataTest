cmake_minimum_required(VERSION 3.28)
project(SimplestMediadataTest)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

set(CMAKE_CXX_STANDARD 17)

file(GLOB rgbs *.rgb)
file(COPY ${rgbs} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB pngs *.png)
file(COPY ${pngs} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB flvs *.flv)
file(COPY ${flvs} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB pcms *.pcm)
file(COPY ${pcms} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB yuvs *yuv)
file(COPY ${yuvs} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB accs *acc)
file(COPY ${accs} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB pks *pk)
file(COPY ${pks} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB h264s *h264)
file(COPY ${h264s} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB tss *ts)
file(COPY ${tss} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})
file(GLOB jpgs *jpg)
file(COPY ${jpgs} DESTINATION ${CMAKE_RUNTIME_OUTPUT_DIRECTORY})

set(udp_src ${CMAKE_CURRENT_SOURCE_DIR}/simplest_mediadata_udp.cpp)

link_libraries(ws2_32)

file(GLOB srcs *.cpp)
# list(REMOVE_ITEM srcs ${udp_src})

foreach(src  ${srcs})
    message(STATUS "${src} added")
endforeach()

add_executable(SimplestMediadataTest ${srcs})
