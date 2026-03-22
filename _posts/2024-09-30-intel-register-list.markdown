---
title: 어셈블리어 개요
date: 2024-09-08 00:00:00 +09:00
categories: [개발 관련, GNU Assembler]
tags: Assembler
---

## 개요

GNU Assembler

General register

* EAX,EBX,ECX,EDX
Segment register
* CS DS ES FS GS SS
Index and Pointer
* ESI EDI EBP EIP ESP
Indicator
EFLAGS

64 bits : RAX RBX RCX RDX
32 bits :  EAX EBX ECX EDX
16 bits : AX BX CX DX
 8 bits : AH AL BH BL CH CL DH DL

범용 레지스터와
 EAX,AX,AH,AL : 누산기 Accumulator 레지스터.
               I/O 포트 접근, 산술, 인터럽트 호출이나 그 외의 경우 사용

EBX,BX,BH,BL : Base register
                메모리 접근을 위한 Base pointer 로 사용한다.
                인터럽트 호출 결과 값을 받기도 한다.

ECX,CX,CH,CL : Counter register
                루프 카운터와 시프트 작업에 사용된다.
                인터럽트 호출 결과값을 받기도 한다.

EDX,DX,DH,DL : Data register
                I/O 포트 접근, 산술, 인터럽트 호출이나 그 외의 경우 사용