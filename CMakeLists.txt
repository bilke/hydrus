cmake_minimum_required(VERSION 2.8.8)
set(CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR})
project(mhm)
enable_language (Fortran)

add_definitions(-DGFORTRAN)

add_executable(h1d_calc
	HYDRUS.FOR
	HYSTER.FOR
	INPUT.FOR
	MATERIAL.FOR
	OUTPUT.FOR
	SINK.FOR
	SOLUTE.FOR
	TEMPER.FOR
	TIME.FOR
	WATFLOW.FOR
)
