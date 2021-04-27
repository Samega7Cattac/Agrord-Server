include(CheckIncludeFileCXX)
CHECK_INCLUDE_FILE_CXX(asio.hpp asio_FOUND)

target_sources(Agrord PRIVATE
        Agrord.cpp Agrord.hpp
        Server.cpp Server.hpp
        Room.cpp Room.hpp)
