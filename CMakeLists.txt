cmake_minimum_required(VERSION 3.12)
project(SR-1)

set(CMAKE_CXX_STANDARD 11)

find_package(SDL2 REQUIRED)

# Incluye manualmente la ubicación del directorio raíz de GLM
include_directories(/opt/homebrew/Cellar/glm/0.9.9.8/include)

add_executable(SR1 src/main.cpp)

target_link_libraries(SR1 ${SDL2_LIBRARIES})
