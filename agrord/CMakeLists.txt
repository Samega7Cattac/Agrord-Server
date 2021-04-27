SET(Boost_USE_MULTITHREAD ON)

find_package(Boost REQUIRED COMPONENTS thread system)

IF(Boost_FOUND)
    include_directories(${Boost_INCLUDE_DIRS})
    link_directories(${Boost_LIBRARY_DIRS})
ENDIF(Boost_FOUND)



target_sources(Agrord PRIVATE
        Agrord.cpp Agrord.hpp
        Server.cpp Server.hpp
        Room.cpp Room.hpp)