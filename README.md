# CH32V003fun MounRiverStudio

Instructions on how to compile and debug code written using the alternative HAL ch32v003fun or for PlatformIO. 
The process is simple: in MRS, delete all files in the USER directory, then delete the files in INC and SRC under Peripheral. 
Next, completely delete the Debug directory. After that, upload ch32v003fun.h to INC and upload ch32v003fun.c to SRC. 
Upload funconfig.h to USER, and in main, include only the code itself. 
Of course, if the code uses other peripherals, the respective files need to be added to INC and SRC. 
This way, you can compile anything in the MRS environment without any issues. 
As an example, I am providing a sample MRS project.
