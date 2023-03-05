# CMakeList.txt : CMake project for SDL_Learning, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

find_package(SDL2 REQUIRED)
find_package(SDL2_image REQUIRED)

# Add source to this project's executable.
add_executable (SDL_Learning "SDL_Learning.cpp" "SDL_Learning.h")

target_link_libraries(SDL_Learning SDL2::SDL2 SDL2::SDL2main SDL2_image::SDL2_image)

# TODO: Add tests and install targets if needed.
