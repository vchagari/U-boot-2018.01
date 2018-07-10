#################################################################################
#                              UBOOT SUNXI 	                                  	#
#																			  	#
#	                 Supports booting from SPI Nor Flash					  	#
#																				#
#################################################################################

Compilation steps: 

	1. cd u-boot-sunxi
	2. make clean
	3. make distclean
	4. make "target defconfig" CROSS_COMPILE="toolchain" 
		(ex: make orangepi_zero_defconfig CROSS_COMPILE=arm-none-eabi-)

Note: 
1. If you get this error at step 4: "In file included from ./tools/../common/env_embedded.c:16:0, from tools/common/env_embedded.c:1:". please do the following to fix it.
2. open tools/common/env_embedded.c file and delete the first line in the file, save and then do the step 4 again. 



