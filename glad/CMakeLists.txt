#
# project: fips-glad\
#  
fips_begin_lib(glad)
	 fips_files(
		include/glad/gl.h 
		include/glad/wgl.h
		include/KHR/khrplatform.h
		src/gl.c 
		src/wgl.c
	) 
fips_end_lib(glad)
if (FIPS_CLANG)
    set_target_properties(glad PROPERTIES COMPILE_FLAGS "-Wno-shift-negative-value")
endif()
