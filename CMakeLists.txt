#
# project: fips-glad
# 
fips_begin_lib(glad)
    fips_files(
		include/glad/gl.h 
		include/glad/wgl.h
		include/glad/KHR/khrplatform.h
		src/gl.c 
		src/wgl.c
    ) 
fips_end_lib(glad)
