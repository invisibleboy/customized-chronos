004001f0 addiu $29 $29 -24
004001f8 sw $31 20 $29 
00400200 sw $30 16 $29 
00400208 addu $30 $0 $29
00400210 jal 00400278
00400218 lui $4 4096
00400220 addiu $4 $4 4160
00400228 lui $5 4096
00400230 addiu $5 $5 2560
00400238 lui $6 4096
00400240 addiu $6 $6 960
00400248 jal 004002b8
00400250 addu $29 $0 $30
00400258 lw $31 20 $29 
00400260 lw $30 16 $29 
00400268 addiu $29 $29 24
00400270 jr $31
00400278 addiu $29 $29 -8
00400280 sw $30 0 $29 
00400288 addu $30 $0 $29
00400290 sw $0 -32624 $28 
00400298 addu $29 $0 $30
004002a0 lw $30 0 $29 
004002a8 addiu $29 $29 8
004002b0 jr $31
004002b8 addiu $29 $29 -24
004002c0 sw $31 20 $29 
004002c8 sw $30 16 $29 
004002d0 addu $30 $0 $29
004002d8 sw $4 24 $30 
004002e0 sw $5 28 $30 
004002e8 sw $6 32 $30 
004002f0 lw $4 24 $30 
004002f8 jal 00400358
00400300 lw $4 28 $30 
00400308 jal 00400358
00400310 lw $4 24 $30 
00400318 lw $5 28 $30 
00400320 lw $6 32 $30 
00400328 jal 004005c8
00400330 addu $29 $0 $30
00400338 lw $31 20 $29 
00400340 lw $30 16 $29 
00400348 addiu $29 $29 24
00400350 jr $31
00400358 addiu $29 $29 -32
00400360 sw $31 28 $29 
00400368 sw $30 24 $29 
00400370 addu $30 $0 $29
00400378 sw $4 32 $30 
00400380 sw $0 16 $30 
00400388 lw $2 16 $30 
00400390 slti $3 $2 20
00400398 bne $3 $0 004003a8
004003a0 j 00400488
004003a8 sw $0 20 $30 
004003b0 lw $2 20 $30 
004003b8 slti $3 $2 20
004003c0 bne $3 $0 004003d0
004003c8 j 00400460
004003d0 jal 004004b0
004003d8 lw $4 16 $30 
004003e0 lw $3 20 $30 
004003e8 addu $5 $0 $3
004003f0 sll $3 $5 0x2
004003f8 addu $6 $0 $4
00400400 sll $5 $6 0x2
00400408 addu $5 $5 $4
00400410 sll $4 $5 0x4
00400418 lw $5 32 $30 
00400420 addu $4 $4 $5
00400428 addu $3 $3 $4
00400430 sw $2 0 $3 
00400438 lw $3 20 $30 
00400440 addiu $2 $3 1
00400448 addu $3 $0 $2
00400450 sw $3 20 $30 
00400458 j 004003b0
00400460 lw $3 16 $30 
00400468 addiu $2 $3 1
00400470 addu $3 $0 $2
00400478 sw $3 16 $30 
00400480 j 00400388
00400488 addu $29 $0 $30
00400490 lw $31 28 $29 
00400498 lw $30 24 $29 
004004a0 addiu $29 $29 32
004004a8 jr $31
004004b0 addiu $29 $29 -8
004004b8 sw $30 0 $29 
004004c0 addu $30 $0 $29
004004c8 lw $2 -32624 $28 
004004d0 addu $4 $0 $2
004004d8 sll $3 $4 0x5
004004e0 addu $3 $3 $2
004004e8 sll $4 $3 0x2
004004f0 addu $4 $4 $2
004004f8 addiu $2 $4 81
00400500 lui $6 4145
00400508 ori $6 $6 5319
00400510 mult $2 $6
00400518 mfhi $5
00400520 mflo $4
00400528 srl $6 $5 0x0
00400530 addu $7 $0 $0
00400538 sra $3 $6 0x9
00400540 sra $4 $2 0x1f
00400548 subu $3 $3 $4
00400550 addu $5 $0 $3
00400558 sll $4 $5 0x6
00400560 subu $4 $4 $3
00400568 sll $5 $4 0x2
00400570 addu $5 $5 $3
00400578 sll $4 $5 0x5
00400580 subu $4 $4 $3
00400588 subu $2 $2 $4
00400590 sw $2 -32624 $28 
00400598 lw $2 -32624 $28 
004005a0 j 004005a8
004005a8 addu $29 $0 $30
004005b0 lw $30 0 $29 
004005b8 addiu $29 $29 8
004005c0 jr $31
004005c8 addiu $29 $29 -8
004005d0 sw $30 0 $29 
004005d8 addu $30 $0 $29
004005e0 sw $4 8 $30 
004005e8 sw $5 12 $30 
004005f0 sw $6 16 $30 
004005f8 addu $2 $0 $0
00400600 slti $5 $2 20
00400608 bne $5 $0 00400618
00400610 j 00400830
00400618 addu $3 $0 $0
00400620 slti $5 $3 20
00400628 bne $5 $0 00400638
00400630 j 00400820
00400638 addu $6 $0 $3
00400640 sll $5 $6 0x2
00400648 addu $7 $0 $2
00400650 sll $6 $7 0x2
00400658 addu $6 $6 $2
00400660 sll $7 $6 0x4
00400668 lw $8 16 $30 
00400670 addu $6 $7 $8
00400678 addu $5 $5 $6
00400680 sw $0 0 $5 
00400688 addu $4 $0 $0
00400690 slti $5 $4 20
00400698 bne $5 $0 004006a8
004006a0 j 00400810
004006a8 addu $6 $0 $3
004006b0 sll $5 $6 0x2
004006b8 addu $7 $0 $2
004006c0 sll $6 $7 0x2
004006c8 addu $6 $6 $2
004006d0 sll $7 $6 0x4
004006d8 lw $8 16 $30 
004006e0 addu $6 $7 $8
004006e8 addu $5 $5 $6
004006f0 addu $7 $0 $3
004006f8 sll $6 $7 0x2
00400700 addu $8 $0 $2
00400708 sll $7 $8 0x2
00400710 addu $7 $7 $2
00400718 sll $8 $7 0x4
00400720 lw $9 16 $30 
00400728 addu $7 $8 $9
00400730 addu $6 $6 $7
00400738 addu $8 $0 $4
00400740 sll $7 $8 0x2
00400748 addu $9 $0 $2
00400750 sll $8 $9 0x2
00400758 addu $8 $8 $2
00400760 sll $9 $8 0x4
00400768 lw $10 8 $30 
00400770 addu $8 $9 $10
00400778 addu $7 $7 $8
00400780 addu $9 $0 $3
00400788 sll $8 $9 0x2
00400790 addu $10 $0 $4
00400798 sll $9 $10 0x2
004007a0 addu $9 $9 $4
004007a8 sll $10 $9 0x4
004007b0 lw $11 12 $30 
004007b8 addu $9 $10 $11
004007c0 addu $8 $8 $9
004007c8 lw $7 0 $7 
004007d0 lw $8 0 $8 
004007d8 mult $7 $8
004007e0 mflo $7
004007e8 lw $6 0 $6 
004007f0 addu $7 $6 $7
004007f8 sw $7 0 $5 
00400800 addiu $4 $4 1
00400808 j 00400690
00400810 addiu $3 $3 1
00400818 j 00400620
00400820 addiu $2 $2 1
00400828 j 00400600
00400830 addu $29 $0 $30
00400838 lw $30 0 $29 
00400840 addiu $29 $29 8
00400848 jr $31