project(implot3d)

add_library(implot3d STATIC 
	"implot3d.cpp"	
	"implot3d.h"
	"implot3d_demo.cpp"
	"implot3d_internal.h"
	"implot3d_items.cpp"
	"implot3d_meshes.cpp"
)

target_include_directories(implot3d PUBLIC ${CMAKE_CURRENT_LIST_DIR})
target_link_libraries(implot3d PUBLIC imgui)
