# Vermillion-Parser

Android ELF file parser test sample for frida-vermillion-Engine.

## Preview

```shell
ELF File: /REDACTED/lib/arm64-v8a/libREDACTED.so
=== ELF File Analysis ===
Architecture: 64-bit

=== ELF64 Header ===
Entry point: 0x0000000000000000
Program header offset: 64
Section header offset: 28584976
Number of program headers: 10
Number of section headers: 28
String table index: 27

=== Section Headers ===
Idx  Name                 Type         Address            Offset     Size      
----------------------------------------------------------------------------
[ 0] <no name>            NULL         0x0000000000000000 0x00000000          0
[ 1] .note.android.ident  NOTE         0x0000000000000270 0x00000270        152
[ 2] .dynsym              DYNSYM       0x0000000000000308 0x00000308      49080
[ 3] .gnu.version         UNKNOWN      0x000000000000c2c0 0x0000c2c0       4090
[ 4] .gnu.version_r       UNKNOWN      0x000000000000d2bc 0x0000d2bc         96
[ 5] .gnu.hash            UNKNOWN      0x000000000000d320 0x0000d320      10984
[ 6] .hash                HASH         0x000000000000fe08 0x0000fe08      16368
[ 7] .dynstr              STRTAB       0x0000000000013df8 0x00013df8     176520
[ 8] .rela.dyn            RELA         0x000000000003ef80 0x0003ef80    2329320
[ 9] .rela.plt            RELA         0x0000000000277a68 0x00277a68      12264
[10] .gcc_except_table    PROGBITS     0x000000000027aa50 0x0027aa50     978448
[11] .rodata              PROGBITS     0x000000000036a000 0x0036a000    4451840
[12] protodesc_cold       PROGBITS     0x00000000007a8e00 0x007a8e00      47744
[13] .eh_frame_hdr        PROGBITS     0x00000000007b4880 0x007b4880     625172
[14] .eh_frame            PROGBITS     0x000000000084d298 0x0084d298    3382260
[15] .text                PROGBITS     0x0000000000b8aec0 0x00b86ec0   15573224
[16] .plt                 PROGBITS     0x0000000001a64fb0 0x01a60fb0       8208
[17] .data.rel.ro         PROGBITS     0x0000000001a6afc0 0x01a62fc0     866696
[18] .fini_array          UNKNOWN      0x0000000001b3e948 0x01b36948         16
[19] .init_array          UNKNOWN      0x0000000001b3e958 0x01b36958       4240
[20] .dynamic             DYNAMIC      0x0000000001b3f9e8 0x01b379e8        560
[21] .got                 PROGBITS     0x0000000001b3fc18 0x01b37c18      24712
[22] .got.plt             PROGBITS     0x0000000001b45ca0 0x01b3dca0       4112
[23] .relro_padding       NOBITS       0x0000000001b46cb0 0x01b3ecb0        848
[24] .data                PROGBITS     0x0000000001b4acb0 0x01b3ecb0      15744
[25] .bss                 NOBITS       0x0000000001b4ea30 0x01b42a30     143064
[26] .comment             PROGBITS     0x0000000000000000 0x01b42a30        204
[27] .shstrtab            STRTAB       0x0000000000000000 0x01b42afc        271

=== Program Headers ===
Idx  Type         Offset     VirtAddr           PhysAddr           FileSiz    MemSiz    
------------------------------------------------------------------------------
[ 0] PHDR         0x00000040 0x0000000000000040 0x0000000000000040        560        560
[ 1] LOAD         0x00000000 0x0000000000000000 0x0000000000000000   12086924   12086924
[ 2] LOAD         0x00b86ec0 0x0000000000b8aec0 0x0000000000b8aec0   15581440   15581440
[ 3] LOAD         0x01a62fc0 0x0000000001a6afc0 0x0000000001a6afc0     900336     901184
[ 4] LOAD         0x01b3ecb0 0x0000000001b4acb0 0x0000000001b4acb0      15744     158808
[ 5] DYNAMIC      0x01b379e8 0x0000000001b3f9e8 0x0000000001b3f9e8        560        560
[ 6] UNKNOWN      0x01a62fc0 0x0000000001a6afc0 0x0000000001a6afc0     900336     901184
[ 7] UNKNOWN      0x007b4880 0x00000000007b4880 0x00000000007b4880     625172     625172
[ 8] UNKNOWN      0x00000000 0x0000000000000000 0x0000000000000000          0          0
[ 9] NOTE         0x00000270 0x0000000000000270 0x0000000000000270        152        152

=== Symbol Table ===

--- DYNSYM (Section 2) ---
Symbol count: 2045, String table: dynstr (section 7)
Idx  Name                           Value              Size       Type     Bind     Shndx 
-------------------------------------------------------------------------------------------
[ 0] <no name>                      0x0000000000000000          0 NOTYPE   LOCAL    UND   
[ 1] __cxa_finalize                 0x0000000000000000          0 FUNC     GLOBAL   UND   
[ 2] __cxa_atexit                   0x0000000000000000          0 FUNC     GLOBAL   UND   
[ 3] _ZdlPv                         0x0000000000000000          0 FUNC     GLOBAL   UND   
[ 4] _ZNSt6__ndk119__shared_weak_count14__release_weakEv 0x0000000000000000          0 FUNC     GLOBAL   UND   
[ 5] __stack_chk_fail               0x0000000000000000          0 FUNC     GLOBAL   UND   
[ 6] strlen                         0x0000000000000000          0 FUNC     GLOBAL   UND   
[ 7] _Znwm                          0x0000000000000000          0 FUNC     GLOBAL   UND   
[ 8] memmove                        0x0000000000000000          0 FUNC     GLOBAL   UND   
[ 9] __cxa_allocate_exception       0x0000000000000000          0 FUNC     GLOBAL   UND   
[10] _ZTISt12length_error           0x0000000000000000          0 OBJECT   GLOBAL   UND   
[11] _ZNSt12length_errorD1Ev        0x0000000000000000          0 FUNC     GLOBAL   UND   
[12] __cxa_throw                    0x0000000000000000          0 FUNC     GLOBAL   UND   
[13] __cxa_free_exception           0x0000000000000000          0 FUNC     GLOBAL   UND   
[14] _ZNSt11logic_errorC2EPKc       0x0000000000000000          0 FUNC     GLOBAL   UND   
[15] _ZTVSt12length_error           0x0000000000000000          0 OBJECT   GLOBAL   UND   
[16] __gxx_personality_v0           0x0000000000000000          0 FUNC     GLOBAL   UND   
[17] _ZTVSt12out_of_range           0x0000000000000000          0 OBJECT   GLOBAL   UND   
[18] _ZTISt12out_of_range           0x0000000000000000          0 OBJECT   GLOBAL   UND   
[19] _ZNSt12out_of_rangeD1Ev        0x0000000000000000          0 FUNC     GLOBAL   UND   
[20] __cxa_begin_catch              0x0000000000000000          0 FUNC     GLOBAL   UND   
[21] __cxa_end_catch                0x0000000000000000          0 FUNC     GLOBAL   UND   
[22] _ZSt9terminatev                0x0000000000000000          0 FUNC     GLOBAL   UND   

{ . . . }

```

## Troubleshooting & Community

This is private project for internal member group, If you encounter any issues, please check the existing issues first.  
- Report new bugs or unexpected behavior by opening a detailed issue.  
- For questions, suggestions, or discussions, feel free to start a thread in the discussions tab.  
- Pull requests to improve documentation, fix bugs, or add features are always welcome.  

Thank you for contributing to the project!
