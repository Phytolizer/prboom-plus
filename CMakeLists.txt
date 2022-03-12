cmake_minimum_required(VERSION 3.20)
project(
    "PrBoom+"
    LANGUAGES CXX
    VERSION 0.1.0
    HOMEPAGE_URL "https://github.com/Phytolizer/prboom-plus.git"
)

set(SRC main.cpp)
list(TRANSFORM SRC PREPEND "prboom2/source/")

add_executable(prboom-plus ${SRC})
