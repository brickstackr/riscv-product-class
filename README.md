# riscv-product-class
 Exercises from the Risc-V product class taught by Kunal Ghosh
 # Exercise 1. 
 ### Counter
 Comparing the counter code in RISC-V to ARM and x86
the ARM output shows way more overhead at the very top of the output. there is a whole extra block like this 
```
        ;ARM64

        %       4
        IMPORT  |__acrt_iob_func|
        IMPORT  |__stdio_common_vfprintf|
        IMPORT  |clock|

|unsigned __int64 `__local_stdio_printf_options'::`2'::_OptionsStorage| % 0x8 ; `__local_stdio_printf_options'::`2'::_OptionsStorage

        ;Flags[SingleProEpi] functionLength[72] RegF[0] RegI[0] H[0] frameChainReturn[Chained] frameSize[48]

        ;Flags[SingleProEpi] functionLength[88] RegF[0] RegI[0] H[0] frameChainReturn[Chained] frameSize[32]
        ;Flags[SingleProEpi] functionLength[36] RegF[0] RegI[0] H[0] frameChainReturn[Chained] frameSize[32]
        ;Flags[SingleProEpi] functionLength[100] RegF[0] RegI[0] H[0] frameChainReturn[Chained] frameSize[32]

        ;Code Words[3], Epilog Start Index[8], E[1], X[0], Function Length[24]=96 bytes
        ;set_fp
        ;save_fplr_x
        ;nop
        ;nop
        ;nop
        ;nop
        ;alloc_s
        ;end
        ;save_fplr_x
        ;alloc_s
        ;end
        ;nop
```
the x86 and RISC-V output are the most similar but there are still some key differences. 
with fewer instructions available, it takes the RISC-V processor more instructions to do each operation

RISC-V operations for the count code: 59
x86 operations for the count code: 50 
