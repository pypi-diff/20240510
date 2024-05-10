# Comparing `tmp/openmm_cuda-8.1.1.11.8-py3-none-win_amd64.whl.zip` & `tmp/openmm_cuda-8.1.1.12-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 921916 bytes, number of entries: 12
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-30 00:23 OpenMM.libs/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-30 00:23 openmm_cuda-8.1.1.11.8.dist-info/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-30 00:23 OpenMM.libs/lib/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-30 00:23 OpenMM.libs/lib/plugins/
--rw-rw-rw-  2.0 fat  1075712 b- defN 24-Apr-30 00:22 OpenMM.libs/lib/plugins/OpenMMAmoebaCUDA.dll
--rw-rw-rw-  2.0 fat  1737216 b- defN 24-Apr-30 00:22 OpenMM.libs/lib/plugins/OpenMMCUDA.dll
--rw-rw-rw-  2.0 fat   108032 b- defN 24-Apr-30 00:23 OpenMM.libs/lib/plugins/OpenMMDrudeCUDA.dll
--rw-rw-rw-  2.0 fat   124416 b- defN 24-Apr-30 00:22 OpenMM.libs/lib/plugins/OpenMMRPMDCUDA.dll
--rw-rw-rw-  2.0 fat       96 b- defN 24-Apr-30 00:23 openmm_cuda-8.1.1.11.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      744 b- defN 24-Apr-30 00:23 openmm_cuda-8.1.1.11.8.dist-info/RECORD
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-30 00:23 openmm_cuda-8.1.1.11.8.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-30 00:23 openmm_cuda-8.1.1.11.8.dist-info/WHEEL
-12 files, 3046309 bytes uncompressed, 920150 bytes compressed:  69.8%
+Zip file size: 921884 bytes, number of entries: 12
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-30 00:14 OpenMM.libs/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-30 00:14 openmm_cuda-8.1.1.12.dist-info/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-30 00:14 OpenMM.libs/lib/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-30 00:14 OpenMM.libs/lib/plugins/
+-rw-rw-rw-  2.0 fat  1075712 b- defN 24-Apr-30 00:13 OpenMM.libs/lib/plugins/OpenMMAmoebaCUDA.dll
+-rw-rw-rw-  2.0 fat  1737216 b- defN 24-Apr-30 00:12 OpenMM.libs/lib/plugins/OpenMMCUDA.dll
+-rw-rw-rw-  2.0 fat   108032 b- defN 24-Apr-30 00:13 OpenMM.libs/lib/plugins/OpenMMDrudeCUDA.dll
+-rw-rw-rw-  2.0 fat   124416 b- defN 24-Apr-30 00:12 OpenMM.libs/lib/plugins/OpenMMRPMDCUDA.dll
+-rw-rw-rw-  2.0 fat       94 b- defN 24-Apr-30 00:14 openmm_cuda-8.1.1.12.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      736 b- defN 24-Apr-30 00:14 openmm_cuda-8.1.1.12.dist-info/RECORD
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-30 00:14 openmm_cuda-8.1.1.12.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-30 00:14 openmm_cuda-8.1.1.12.dist-info/WHEEL
+12 files, 3046299 bytes uncompressed, 920138 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: OpenMM.libs/
 Comment: 
 
-Filename: openmm_cuda-8.1.1.11.8.dist-info/
+Filename: openmm_cuda-8.1.1.12.dist-info/
 Comment: 
 
 Filename: OpenMM.libs/lib/
 Comment: 
 
 Filename: OpenMM.libs/lib/plugins/
 Comment: 
@@ -18,20 +18,20 @@
 
 Filename: OpenMM.libs/lib/plugins/OpenMMDrudeCUDA.dll
 Comment: 
 
 Filename: OpenMM.libs/lib/plugins/OpenMMRPMDCUDA.dll
 Comment: 
 
-Filename: openmm_cuda-8.1.1.11.8.dist-info/METADATA
+Filename: openmm_cuda-8.1.1.12.dist-info/METADATA
 Comment: 
 
-Filename: openmm_cuda-8.1.1.11.8.dist-info/RECORD
+Filename: openmm_cuda-8.1.1.12.dist-info/RECORD
 Comment: 
 
-Filename: openmm_cuda-8.1.1.11.8.dist-info/top_level.txt
+Filename: openmm_cuda-8.1.1.12.dist-info/top_level.txt
 Comment: 
 
-Filename: openmm_cuda-8.1.1.11.8.dist-info/WHEEL
+Filename: openmm_cuda-8.1.1.12.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## OpenMM.libs/lib/plugins/OpenMMAmoebaCUDA.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800452e0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 00:22:53 2024
+Time/Date		Tue Apr 30 00:13:06 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000004a000
 SizeOfInitializedData	00000000000bce00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000452e0
@@ -166,15 +166,15 @@
 	fd8fa	  159  ?getExtrapolationCoefficients@AmoebaMultipoleForce@OpenMM@@QEBAAEBV?$vector@NV?$allocator@N@std@@@std@@XZ
 	fd8b4	  177  ?getMutualInducedTargetEpsilon@AmoebaMultipoleForce@OpenMM@@QEBANXZ
 	fd86e	  176  ?getMutualInducedMaxIterations@AmoebaMultipoleForce@OpenMM@@QEBAHXZ
 	fd7fc	  136  ?getCovalentMap@AmoebaMultipoleForce@OpenMM@@QEBAXHW4CovalentType@12@AEAV?$vector@HV?$allocator@H@std@@@std@@@Z
 
  000fbc18	000fc7a0 00000000 00000000 000fe6d2 0004bac0
 
-	DLL Name: cufft64_10.dll
+	DLL Name: cufft64_11.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	fe654	   32  cufftPlan3d
 	fe662	    9  cufftExecC2C
 	fe672	   12  cufftExecR2C
 	fe682	   10  cufftExecC2R
 	fe692	   14  cufftExecZ2Z
 	fe6a2	   11  cufftExecD2Z
@@ -11874,15 +11874,15 @@
 	  b030: 6c 61 6e 33 64 00 09 00 63 75 66 66 74 45 78 65
 	  b040: 63 43 32 43 00 00 0c 00 63 75 66 66 74 45 78 65
 	  b050: 63 52 32 43 00 00 0a 00 63 75 66 66 74 45 78 65
 	  b060: 63 43 32 52 00 00 0e 00 63 75 66 66 74 45 78 65
 	  b070: 63 5a 32 5a 00 00 0b 00 63 75 66 66 74 45 78 65
 	  b080: 63 44 32 5a 00 00 0d 00 63 75 66 66 74 45 78 65
 	  b090: 63 5a 32 44 00 00 03 00 63 75 66 66 74 44 65 73
-	  b0a0: 74 72 6f 79 00 00 63 75 66 66 74 36 34 5f 31 30
+	  b0a0: 74 72 6f 79 00 00 63 75 66 66 74 36 34 5f 31 31
 	  b0b0: 2e 64 6c 6c 00 00 d3 02 3f 3f 31 50 6c 61 74 66
 	  b0c0: 6f 72 6d 40 4f 70 65 6e 4d 4d 40 40 55 45 41 41
 	  b0d0: 40 58 5a 00 e9 09 3f 67 65 74 50 72 6f 70 65 72
 	  b0e0: 74 79 56 61 6c 75 65 40 50 6c 61 74 66 6f 72 6d
 	  b0f0: 40 4f 70 65 6e 4d 4d 40 40 55 45 42 41 41 45 42
 	  b100: 56 3f 24 62 61 73 69 63 5f 73 74 72 69 6e 67 40
 	  b110: 44 55 3f 24 63 68 61 72 5f 74 72 61 69 74 73 40
@@ -375244,19 +375244,17 @@
    1800e9eb8:	movsxd 0x74(%rcx),%esp
    1800e9ebb:	imul   $0x4be00000,0x6e(%rdi),%ebp
    1800e9ec2:	adc    %al,0x1(%rax)
    1800e9ec8:	orb    $0x1,-0x80(%rax,%rdx,1)
    1800e9ecd:	add    %al,(%rax)
    1800e9ecf:	add    %al,(%rax)
    1800e9ed1:	add    %al,(%rax)
-   1800e9ed3:	add    %bl,%ch
-   1800e9ed5:	cmp    %esi,(%rax)
-   1800e9ed7:	data16 add %al,(%rax)
-   1800e9eda:	add    %al,(%rax)
-   1800e9edc:	or     $0x64000000,%eax
+   1800e9ed3:	add    %dl,0x663037(%rdx)
+   1800e9ed9:	add    %al,(%rax)
+   1800e9edb:	add    %cl,0x64000000(%rip)        # 0x1e40e9ee1
    1800e9ee1:	add    (%rax),%eax
    1800e9ee3:	add    %dh,0xe(%rax,%rdx,8)
    1800e9ee7:	add    %dh,0xe(%rsp,%rax,8)
    1800e9eeb:	add    %al,(%rax)
    1800e9eed:	add    %al,(%rax)
    1800e9eef:	add    %bh,(%rax)
    1800e9ef1:	add    %eax,(%rax)
@@ -412136,15 +412134,15 @@
    1800fe6c7:	data16 je 0x1800fe70e
    1800fe6ca:	gs jae 0x1800fe741
    1800fe6cd:	jb     0x1800fe73e
    1800fe6cf:	jns    0x1800fe6d1
    1800fe6d1:	add    %ah,0x75(%rbx)
    1800fe6d4:	data16 data16 je 0x1800fe70e
    1800fe6d8:	xor    $0x5f,%al
-   1800fe6da:	xor    %esi,(%rax)
+   1800fe6da:	xor    %esi,(%rcx)
    1800fe6dc:	cs fs insb (%dx),%es:(%rdi)
    1800fe6df:	insb   (%dx),%es:(%rdi)
    1800fe6e0:	add    %al,(%rax)
    1800fe6e2:	roll   %cl,(%rdx)
    1800fe6e4:	(bad)
    1800fe6e5:	(bad)
    1800fe6e6:	xor    %edx,0x6c(%rax)
```

## OpenMM.libs/lib/plugins/OpenMMCUDA.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800e1738
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 00:22:19 2024
+Time/Date		Tue Apr 30 00:12:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000000f0a00
 SizeOfInitializedData	00000000000b7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000e1738
@@ -492,84 +492,84 @@
 	197f16	 1973  ?getAngleParameters@HarmonicAngleForce@OpenMM@@QEBAXHAEAH00AEAN1@Z
 	192be8	  644  ??1CustomFunction@Lepton@@UEAA@XZ
 
  001915ec	00192a38 00000000 00000000 0019c3ee 000f3320
 
 	DLL Name: nvcuda.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	19c304	  136  cuEventSynchronize
-	19c31a	  129  cuEventDestroy_v2
-	19c32e	  317  cuMemHostGetDevicePointer_v2
-	19c34e	  140  cuFuncGetAttribute
-	19c364	  106  cuDeviceGetName
-	19c2f4	  132  cuEventRecord
-	19c376	  491  cuStreamCreate
-	19c388	  519  cuStreamWaitEvent
-	19c39c	  494  cuStreamDestroy_v2
-	19c3b2	  144  cuFuncSetCacheConfig
-	19c2e4	  127  cuEventCreate
-	19c3de	  365  cuMemcpyAsync
-	19c0ac	  299  cuMemAlloc_v2
-	19c2d2	  474  cuProfilerStop
+	19c304	  137  cuEventSynchronize
+	19c31a	  130  cuEventDestroy_v2
+	19c32e	  339  cuMemHostGetDevicePointer_v2
+	19c34e	  141  cuFuncGetAttribute
+	19c364	  107  cuDeviceGetName
+	19c2f4	  133  cuEventRecord
+	19c376	  513  cuStreamCreate
+	19c388	  543  cuStreamWaitEvent
+	19c39c	  516  cuStreamDestroy_v2
+	19c3b2	  145  cuFuncSetCacheConfig
+	19c2e4	  128  cuEventCreate
+	19c3de	  387  cuMemcpyAsync
+	19c0ac	  321  cuMemAlloc_v2
+	19c2d2	  496  cuProfilerStop
 	19c2ba	   20  cuCtxEnablePeerAccess
-	19c2a2	   95  cuDeviceCanAccessPeer
-	19c290	  274  cuLaunchKernel
-	19c27a	  515  cuStreamSynchronize
-	19c268	  315  cuMemHostAlloc
-	19c258	  305  cuMemFreeHost
-	19c242	  446  cuModuleGetFunction
-	19c21c	  452  cuModuleLoad
-	19c0bc	  306  cuMemFree_v2
-	19c0cc	  404  cuMemcpyHtoD_v2
-	19c0de	  392  cuMemcpyDtoH_v2
-	19c0f0	  402  cuMemcpyHtoDAsync_v2
-	19c108	  390  cuMemcpyDtoHAsync_v2
-	19c120	  384  cuMemcpyDtoDAsync_v2
-	19c138	  163  cuGetErrorName
-	19c22c	  454  cuModuleLoadDataEx
-	19c14a	  259  cuInit
-	19c154	  126  cuDriverGetVersion
-	19c3ca	   39  cuCtxSynchronize
-	19c206	   35  cuCtxSetCacheConfig
-	19c1f4	   36  cuCtxSetCurrent
-	19c1de	   31  cuCtxPopCurrent_v2
-	19c1c8	   33  cuCtxPushCurrent_v2
+	19c2a2	   96  cuDeviceCanAccessPeer
+	19c290	  288  cuLaunchKernel
+	19c27a	  539  cuStreamSynchronize
+	19c268	  337  cuMemHostAlloc
+	19c258	  327  cuMemFreeHost
+	19c242	  468  cuModuleGetFunction
+	19c21c	  474  cuModuleLoad
+	19c0bc	  328  cuMemFree_v2
+	19c0cc	  426  cuMemcpyHtoD_v2
+	19c0de	  414  cuMemcpyDtoH_v2
+	19c0f0	  424  cuMemcpyHtoDAsync_v2
+	19c108	  412  cuMemcpyDtoHAsync_v2
+	19c120	  406  cuMemcpyDtoDAsync_v2
+	19c138	  164  cuGetErrorName
+	19c22c	  476  cuModuleLoadDataEx
+	19c14a	  269  cuInit
+	19c154	  127  cuDriverGetVersion
+	19c3ca	   40  cuCtxSynchronize
+	19c206	   36  cuCtxSetCacheConfig
+	19c1f4	   37  cuCtxSetCurrent
+	19c1de	   32  cuCtxPopCurrent_v2
+	19c1c8	   34  cuCtxPushCurrent_v2
 	19c1b6	   17  cuCtxDestroy_v2
 	19c1a4	   14  cuCtxCreate_v2
-	19c18c	   98  cuDeviceGetAttribute
-	19c178	  100  cuDeviceGetCount
-	19c16a	   97  cuDeviceGet
+	19c18c	   99  cuDeviceGetAttribute
+	19c178	  101  cuDeviceGetCount
+	19c16a	   98  cuDeviceGet
 
  00191600	001929f0 00000000 00000000 0019c47c 000f32d8
 
-	DLL Name: cufft64_10.dll
+	DLL Name: cufft64_11.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	19c45a	    3  cufftDestroy
 	19c448	   35  cufftSetStream
 	19c438	   13  cufftExecZ2D
 	19c46a	   22  cufftGetVersion
 	19c418	   10  cufftExecC2R
 	19c408	   12  cufftExecR2C
 	19c3fa	   32  cufftPlan3d
 	19c428	   11  cufftExecD2Z
 
  00191614	00192b90 00000000 00000000 0019c56a 000f3478
 
-	DLL Name: nvrtc64_112_0.dll
+	DLL Name: nvrtc64_120_0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	19c52c	   12  nvrtcGetPTX
-	19c51a	   13  nvrtcGetPTXSize
+	19c52c	   16  nvrtcGetPTX
+	19c51a	   17  nvrtcGetPTXSize
 	19c504	    2  nvrtcCompileProgram
 	19c4ee	    4  nvrtcDestroyProgram
 	19c4d8	    3  nvrtcCreateProgram
-	19c4be	   16  nvrtcGetSupportedArchs
-	19c4a2	   11  nvrtcGetNumSupportedArchs
+	19c4be	   20  nvrtcGetSupportedArchs
+	19c4a2	   13  nvrtcGetNumSupportedArchs
 	19c48c	    7  nvrtcGetErrorString
-	19c53a	   15  nvrtcGetProgramLogSize
-	19c554	   14  nvrtcGetProgramLog
+	19c53a	   19  nvrtcGetProgramLogSize
+	19c554	   18  nvrtcGetProgramLog
 
  00191628	00191718 00000000 00000000 0019c738 000f2000
 
 	DLL Name: KERNEL32.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	19ddb0	  906  InitializeSListHead
 	19dd7e	  567  GetCurrentThreadId
@@ -995,17 +995,17 @@
 	[ 181] +base[ 182] ae40 Export RVA
 	[ 182] +base[ 183] af00 Export RVA
 	[ 183] +base[ 184] afc0 Export RVA
 	[ 184] +base[ 185] b070 Export RVA
 	[ 185] +base[ 186] b130 Export RVA
 	[ 186] +base[ 187] b200 Export RVA
 	[ 187] +base[ 188] fe2c0 Export RVA
-	[ 188] +base[ 189] f49bc Export RVA
+	[ 188] +base[ 189] f49cc Export RVA
 	[ 189] +base[ 190] fe2c4 Export RVA
-	[ 190] +base[ 191] f4a20 Export RVA
+	[ 190] +base[ 191] f4a30 Export RVA
 	[ 191] +base[ 192] c130 Export RVA
 	[ 192] +base[ 193] c140 Export RVA
 	[ 193] +base[ 194] fe00 Export RVA
 	[ 194] +base[ 195] ff20 Export RVA
 	[ 195] +base[ 196] 42560 Export RVA
 	[ 196] +base[ 197] 42570 Export RVA
 	[ 197] +base[ 198] 193a0 Export RVA
@@ -19546,16 +19546,16 @@
 	  450: 68 39 0f 00 90 39 0f 00 e0 39 0f 00 80 38 0f 00
 	  460: 18 39 0f 00 70 40 0f 00 80 7f 0f 00 40 3e 0f 00
 	  470: 78 3e 0f 00 68 3f 0f 00 f8 3d 0f 00 78 42 0f 00
 	  480: e0 3d 0f 00 60 42 0f 00 60 3a 0f 00 38 3b 0f 00
 	  490: c8 3d 0f 00 48 42 0f 00 b0 3d 0f 00 30 42 0f 00
 	  4a0: 50 ab 00 00 00 ac 00 00 d0 ac 00 00 90 ad 00 00
 	  4b0: 40 ae 00 00 00 af 00 00 c0 af 00 00 70 b0 00 00
-	  4c0: 30 b1 00 00 00 b2 00 00 c0 e2 0f 00 bc 49 0f 00
-	  4d0: c4 e2 0f 00 20 4a 0f 00 30 c1 00 00 40 c1 00 00
+	  4c0: 30 b1 00 00 00 b2 00 00 c0 e2 0f 00 cc 49 0f 00
+	  4d0: c4 e2 0f 00 30 4a 0f 00 30 c1 00 00 40 c1 00 00
 	  4e0: 00 fe 00 00 20 ff 00 00 60 25 04 00 70 25 04 00
 	  4f0: a0 93 01 00 30 94 01 00 70 ff 00 00 90 94 01 00
 	  500: 30 26 04 00 d0 70 0c 00 90 01 01 00 50 28 04 00
 	  510: b0 32 04 00 10 33 04 00 20 33 04 00 10 71 0c 00
 	  520: 50 71 0c 00 80 02 01 00 90 71 0c 00 d0 71 0c 00
 	  530: 20 e1 19 00 40 e1 19 00 90 ec 0d 00 b0 3e 02 00
 	  540: a0 ec 0d 00 d0 d4 00 00 d0 d4 00 00 60 e1 19 00
@@ -25194,91 +25194,91 @@
 	  16550: 40 40 40 32 40 40 73 74 64 40 40 56 3f 24 61 6c
 	  16560: 6c 6f 63 61 74 6f 72 40 56 3f 24 76 65 63 74 6f
 	  16570: 72 40 55 3f 24 70 61 69 72 40 48 4e 40 73 74 64
 	  16580: 40 40 56 3f 24 61 6c 6c 6f 63 61 74 6f 72 40 55
 	  16590: 3f 24 70 61 69 72 40 48 4e 40 73 74 64 40 40 40
 	  165a0: 32 40 40 73 74 64 40 40 40 32 40 40 73 74 64 40
 	  165b0: 40 58 5a 00 4f 70 65 6e 4d 4d 2e 64 6c 6c 00 00
-	  165c0: 2b 01 63 75 4d 65 6d 41 6c 6c 6f 63 5f 76 32 00
-	  165d0: 32 01 63 75 4d 65 6d 46 72 65 65 5f 76 32 00 00
-	  165e0: 94 01 63 75 4d 65 6d 63 70 79 48 74 6f 44 5f 76
-	  165f0: 32 00 88 01 63 75 4d 65 6d 63 70 79 44 74 6f 48
-	  16600: 5f 76 32 00 92 01 63 75 4d 65 6d 63 70 79 48 74
-	  16610: 6f 44 41 73 79 6e 63 5f 76 32 00 00 86 01 63 75
+	  165c0: 41 01 63 75 4d 65 6d 41 6c 6c 6f 63 5f 76 32 00
+	  165d0: 48 01 63 75 4d 65 6d 46 72 65 65 5f 76 32 00 00
+	  165e0: aa 01 63 75 4d 65 6d 63 70 79 48 74 6f 44 5f 76
+	  165f0: 32 00 9e 01 63 75 4d 65 6d 63 70 79 44 74 6f 48
+	  16600: 5f 76 32 00 a8 01 63 75 4d 65 6d 63 70 79 48 74
+	  16610: 6f 44 41 73 79 6e 63 5f 76 32 00 00 9c 01 63 75
 	  16620: 4d 65 6d 63 70 79 44 74 6f 48 41 73 79 6e 63 5f
-	  16630: 76 32 00 00 80 01 63 75 4d 65 6d 63 70 79 44 74
-	  16640: 6f 44 41 73 79 6e 63 5f 76 32 00 00 a3 00 63 75
-	  16650: 47 65 74 45 72 72 6f 72 4e 61 6d 65 00 00 03 01
-	  16660: 63 75 49 6e 69 74 00 00 7e 00 63 75 44 72 69 76
-	  16670: 65 72 47 65 74 56 65 72 73 69 6f 6e 00 00 61 00
-	  16680: 63 75 44 65 76 69 63 65 47 65 74 00 64 00 63 75
+	  16630: 76 32 00 00 96 01 63 75 4d 65 6d 63 70 79 44 74
+	  16640: 6f 44 41 73 79 6e 63 5f 76 32 00 00 a4 00 63 75
+	  16650: 47 65 74 45 72 72 6f 72 4e 61 6d 65 00 00 0d 01
+	  16660: 63 75 49 6e 69 74 00 00 7f 00 63 75 44 72 69 76
+	  16670: 65 72 47 65 74 56 65 72 73 69 6f 6e 00 00 62 00
+	  16680: 63 75 44 65 76 69 63 65 47 65 74 00 65 00 63 75
 	  16690: 44 65 76 69 63 65 47 65 74 43 6f 75 6e 74 00 00
-	  166a0: 62 00 63 75 44 65 76 69 63 65 47 65 74 41 74 74
+	  166a0: 63 00 63 75 44 65 76 69 63 65 47 65 74 41 74 74
 	  166b0: 72 69 62 75 74 65 00 00 0e 00 63 75 43 74 78 43
 	  166c0: 72 65 61 74 65 5f 76 32 00 00 11 00 63 75 43 74
-	  166d0: 78 44 65 73 74 72 6f 79 5f 76 32 00 21 00 63 75
+	  166d0: 78 44 65 73 74 72 6f 79 5f 76 32 00 22 00 63 75
 	  166e0: 43 74 78 50 75 73 68 43 75 72 72 65 6e 74 5f 76
-	  166f0: 32 00 1f 00 63 75 43 74 78 50 6f 70 43 75 72 72
-	  16700: 65 6e 74 5f 76 32 00 00 24 00 63 75 43 74 78 53
-	  16710: 65 74 43 75 72 72 65 6e 74 00 23 00 63 75 43 74
+	  166f0: 32 00 20 00 63 75 43 74 78 50 6f 70 43 75 72 72
+	  16700: 65 6e 74 5f 76 32 00 00 25 00 63 75 43 74 78 53
+	  16710: 65 74 43 75 72 72 65 6e 74 00 24 00 63 75 43 74
 	  16720: 78 53 65 74 43 61 63 68 65 43 6f 6e 66 69 67 00
-	  16730: c4 01 63 75 4d 6f 64 75 6c 65 4c 6f 61 64 00 00
-	  16740: c6 01 63 75 4d 6f 64 75 6c 65 4c 6f 61 64 44 61
-	  16750: 74 61 45 78 00 00 be 01 63 75 4d 6f 64 75 6c 65
-	  16760: 47 65 74 46 75 6e 63 74 69 6f 6e 00 31 01 63 75
-	  16770: 4d 65 6d 46 72 65 65 48 6f 73 74 00 3b 01 63 75
-	  16780: 4d 65 6d 48 6f 73 74 41 6c 6c 6f 63 00 00 03 02
+	  16730: da 01 63 75 4d 6f 64 75 6c 65 4c 6f 61 64 00 00
+	  16740: dc 01 63 75 4d 6f 64 75 6c 65 4c 6f 61 64 44 61
+	  16750: 74 61 45 78 00 00 d4 01 63 75 4d 6f 64 75 6c 65
+	  16760: 47 65 74 46 75 6e 63 74 69 6f 6e 00 47 01 63 75
+	  16770: 4d 65 6d 46 72 65 65 48 6f 73 74 00 51 01 63 75
+	  16780: 4d 65 6d 48 6f 73 74 41 6c 6c 6f 63 00 00 1b 02
 	  16790: 63 75 53 74 72 65 61 6d 53 79 6e 63 68 72 6f 6e
-	  167a0: 69 7a 65 00 12 01 63 75 4c 61 75 6e 63 68 4b 65
-	  167b0: 72 6e 65 6c 00 00 5f 00 63 75 44 65 76 69 63 65
+	  167a0: 69 7a 65 00 20 01 63 75 4c 61 75 6e 63 68 4b 65
+	  167b0: 72 6e 65 6c 00 00 60 00 63 75 44 65 76 69 63 65
 	  167c0: 43 61 6e 41 63 63 65 73 73 50 65 65 72 00 14 00
 	  167d0: 63 75 43 74 78 45 6e 61 62 6c 65 50 65 65 72 41
-	  167e0: 63 63 65 73 73 00 da 01 63 75 50 72 6f 66 69 6c
-	  167f0: 65 72 53 74 6f 70 00 00 7f 00 63 75 45 76 65 6e
-	  16800: 74 43 72 65 61 74 65 00 84 00 63 75 45 76 65 6e
-	  16810: 74 52 65 63 6f 72 64 00 88 00 63 75 45 76 65 6e
-	  16820: 74 53 79 6e 63 68 72 6f 6e 69 7a 65 00 00 81 00
+	  167e0: 63 63 65 73 73 00 f0 01 63 75 50 72 6f 66 69 6c
+	  167f0: 65 72 53 74 6f 70 00 00 80 00 63 75 45 76 65 6e
+	  16800: 74 43 72 65 61 74 65 00 85 00 63 75 45 76 65 6e
+	  16810: 74 52 65 63 6f 72 64 00 89 00 63 75 45 76 65 6e
+	  16820: 74 53 79 6e 63 68 72 6f 6e 69 7a 65 00 00 82 00
 	  16830: 63 75 45 76 65 6e 74 44 65 73 74 72 6f 79 5f 76
-	  16840: 32 00 3d 01 63 75 4d 65 6d 48 6f 73 74 47 65 74
+	  16840: 32 00 53 01 63 75 4d 65 6d 48 6f 73 74 47 65 74
 	  16850: 44 65 76 69 63 65 50 6f 69 6e 74 65 72 5f 76 32
-	  16860: 00 00 8c 00 63 75 46 75 6e 63 47 65 74 41 74 74
-	  16870: 72 69 62 75 74 65 00 00 6a 00 63 75 44 65 76 69
-	  16880: 63 65 47 65 74 4e 61 6d 65 00 eb 01 63 75 53 74
-	  16890: 72 65 61 6d 43 72 65 61 74 65 00 00 07 02 63 75
+	  16860: 00 00 8d 00 63 75 46 75 6e 63 47 65 74 41 74 74
+	  16870: 72 69 62 75 74 65 00 00 6b 00 63 75 44 65 76 69
+	  16880: 63 65 47 65 74 4e 61 6d 65 00 01 02 63 75 53 74
+	  16890: 72 65 61 6d 43 72 65 61 74 65 00 00 1f 02 63 75
 	  168a0: 53 74 72 65 61 6d 57 61 69 74 45 76 65 6e 74 00
-	  168b0: ee 01 63 75 53 74 72 65 61 6d 44 65 73 74 72 6f
-	  168c0: 79 5f 76 32 00 00 90 00 63 75 46 75 6e 63 53 65
-	  168d0: 74 43 61 63 68 65 43 6f 6e 66 69 67 00 00 27 00
+	  168b0: 04 02 63 75 53 74 72 65 61 6d 44 65 73 74 72 6f
+	  168c0: 79 5f 76 32 00 00 91 00 63 75 46 75 6e 63 53 65
+	  168d0: 74 43 61 63 68 65 43 6f 6e 66 69 67 00 00 28 00
 	  168e0: 63 75 43 74 78 53 79 6e 63 68 72 6f 6e 69 7a 65
-	  168f0: 00 00 6d 01 63 75 4d 65 6d 63 70 79 41 73 79 6e
+	  168f0: 00 00 83 01 63 75 4d 65 6d 63 70 79 41 73 79 6e
 	  16900: 63 00 6e 76 63 75 64 61 2e 64 6c 6c 00 00 20 00
 	  16910: 63 75 66 66 74 50 6c 61 6e 33 64 00 0c 00 63 75
 	  16920: 66 66 74 45 78 65 63 52 32 43 00 00 0a 00 63 75
 	  16930: 66 66 74 45 78 65 63 43 32 52 00 00 0b 00 63 75
 	  16940: 66 66 74 45 78 65 63 44 32 5a 00 00 0d 00 63 75
 	  16950: 66 66 74 45 78 65 63 5a 32 44 00 00 23 00 63 75
 	  16960: 66 66 74 53 65 74 53 74 72 65 61 6d 00 00 03 00
 	  16970: 63 75 66 66 74 44 65 73 74 72 6f 79 00 00 16 00
 	  16980: 63 75 66 66 74 47 65 74 56 65 72 73 69 6f 6e 00
-	  16990: 63 75 66 66 74 36 34 5f 31 30 2e 64 6c 6c 00 00
+	  16990: 63 75 66 66 74 36 34 5f 31 31 2e 64 6c 6c 00 00
 	  169a0: 07 00 6e 76 72 74 63 47 65 74 45 72 72 6f 72 53
-	  169b0: 74 72 69 6e 67 00 0b 00 6e 76 72 74 63 47 65 74
+	  169b0: 74 72 69 6e 67 00 0d 00 6e 76 72 74 63 47 65 74
 	  169c0: 4e 75 6d 53 75 70 70 6f 72 74 65 64 41 72 63 68
-	  169d0: 73 00 10 00 6e 76 72 74 63 47 65 74 53 75 70 70
+	  169d0: 73 00 14 00 6e 76 72 74 63 47 65 74 53 75 70 70
 	  169e0: 6f 72 74 65 64 41 72 63 68 73 00 00 03 00 6e 76
 	  169f0: 72 74 63 43 72 65 61 74 65 50 72 6f 67 72 61 6d
 	  16a00: 00 00 04 00 6e 76 72 74 63 44 65 73 74 72 6f 79
 	  16a10: 50 72 6f 67 72 61 6d 00 02 00 6e 76 72 74 63 43
-	  16a20: 6f 6d 70 69 6c 65 50 72 6f 67 72 61 6d 00 0d 00
+	  16a20: 6f 6d 70 69 6c 65 50 72 6f 67 72 61 6d 00 11 00
 	  16a30: 6e 76 72 74 63 47 65 74 50 54 58 53 69 7a 65 00
-	  16a40: 0c 00 6e 76 72 74 63 47 65 74 50 54 58 00 0f 00
+	  16a40: 10 00 6e 76 72 74 63 47 65 74 50 54 58 00 13 00
 	  16a50: 6e 76 72 74 63 47 65 74 50 72 6f 67 72 61 6d 4c
-	  16a60: 6f 67 53 69 7a 65 00 00 0e 00 6e 76 72 74 63 47
+	  16a60: 6f 67 53 69 7a 65 00 00 12 00 6e 76 72 74 63 47
 	  16a70: 65 74 50 72 6f 67 72 61 6d 4c 6f 67 00 00 6e 76
-	  16a80: 72 74 63 36 34 5f 31 31 32 5f 30 2e 64 6c 6c 00
+	  16a80: 72 74 63 36 34 5f 31 32 30 5f 30 2e 64 6c 6c 00
 	  16a90: 33 02 47 65 74 43 75 72 72 65 6e 74 50 72 6f 63
 	  16aa0: 65 73 73 49 64 00 0a 03 47 65 74 53 79 73 74 65
 	  16ab0: 6d 54 69 6d 65 41 73 46 69 6c 65 54 69 6d 65 00
 	  16ac0: 04 03 47 65 74 53 79 73 74 65 6d 49 6e 66 6f 00
 	  16ad0: 94 00 43 6c 6f 73 65 48 61 6e 64 6c 65 00 d8 04
 	  16ae0: 52 65 6c 65 61 73 65 53 52 57 4c 6f 63 6b 45 78
 	  16af0: 63 6c 75 73 69 76 65 00 d9 04 52 65 6c 65 61 73
@@ -26699,19 +26699,19 @@
 	reloc   54 offset  250 [f4250] DIR64
 	reloc   55 offset  258 [f4258] DIR64
 	reloc   56 offset  260 [f4260] DIR64
 	reloc   57 offset  268 [f4268] DIR64
 	reloc   58 offset  270 [f4270] DIR64
 	reloc   59 offset  278 [f4278] DIR64
 	reloc   60 offset  280 [f4280] DIR64
-	reloc   61 offset  a40 [f4a40] DIR64
-	reloc   62 offset  a48 [f4a48] DIR64
-	reloc   63 offset  a50 [f4a50] DIR64
-	reloc   64 offset  a68 [f4a68] DIR64
-	reloc   65 offset  a70 [f4a70] DIR64
+	reloc   61 offset  a38 [f4a38] DIR64
+	reloc   62 offset  a40 [f4a40] DIR64
+	reloc   63 offset  a48 [f4a48] DIR64
+	reloc   64 offset  a60 [f4a60] DIR64
+	reloc   65 offset  a68 [f4a68] DIR64
 
 Virtual Address: 000f5000 Chunk size 72 (0x48) Number of fixups 32
 	reloc    0 offset  7c0 [f57c0] DIR64
 	reloc    1 offset  7c8 [f57c8] DIR64
 	reloc    2 offset  7d0 [f57d0] DIR64
 	reloc    3 offset  7d8 [f57d8] DIR64
 	reloc    4 offset  7e0 [f57e0] DIR64
@@ -51131,15 +51131,15 @@
    180014a1f:	int3
    180014a20:	mov    %rbx,0x10(%rsp)
    180014a25:	mov    %rcx,0x8(%rsp)
    180014a2a:	push   %rdi
    180014a2b:	sub    $0x20,%rsp
    180014a2f:	mov    %rdx,%rbx
    180014a32:	mov    %rcx,%rdi
-   180014a35:	lea    0xe0034(%rip),%rax        # 0x1800f4a70
+   180014a35:	lea    0xe002c(%rip),%rax        # 0x1800f4a68
    180014a3c:	mov    %rax,(%rcx)
    180014a3f:	mov    0x8(%rdx),%rax
    180014a43:	mov    %rax,0x8(%rcx)
    180014a47:	add    $0x10,%rdx
    180014a4b:	add    $0x10,%rcx
    180014a4f:	call   0x180004eb0
    180014a54:	nop
@@ -51281,15 +51281,15 @@
    180014c37:	mov    %rax,0x10(%rsi)
    180014c3b:	mov    %rsi,0x88(%rsp)
    180014c43:	mov    (%rsi),%rbx
    180014c46:	mov    %rbx,0x20(%rsp)
    180014c4b:	mov    %rbx,0x28(%rsp)
    180014c50:	mov    %rsi,0x30(%rsp)
    180014c55:	lea    0x10(%r13),%rdi
-   180014c59:	lea    0xdfe10(%rip),%r15        # 0x1800f4a70
+   180014c59:	lea    0xdfe08(%rip),%r15        # 0x1800f4a68
    180014c60:	mov    %rbx,0x90(%rsp)
    180014c68:	mov    %r15,(%rbx)
    180014c6b:	mov    -0x8(%rdi),%rax
    180014c6f:	mov    %rax,0x8(%rbx)
    180014c73:	lea    0x10(%rbx),%rcx
    180014c77:	mov    %rdi,%rdx
    180014c7a:	call   0x180004eb0
@@ -52103,15 +52103,15 @@
    180015a65:	lea    0xa0(%rbp),%rcx
    180015a6c:	call   0x18000c600
    180015a71:	nop
    180015a72:	lea    0xa0(%rbp),%rdx
    180015a79:	mov    %rdi,%rcx
    180015a7c:	call   0x18000f7f0
    180015a81:	xor    %r8d,%r8d
-   180015a84:	lea    0xdefad(%rip),%rdx        # 0x1800f4a38
+   180015a84:	lea    0xdefa9(%rip),%rdx        # 0x1800f4a34
    180015a8b:	mov    %rax,%rcx
    180015a8e:	call   0x18000c600
    180015a93:	nop
    180015a94:	mov    0xb8(%rbp),%rdx
    180015a9b:	cmp    $0x10,%rdx
    180015a9f:	jb     0x180015ad8
    180015aa1:	inc    %rdx
@@ -53701,15 +53701,15 @@
    180017832:	mov    %rax,%rcx
    180017835:	lea    0xdd288(%rip),%rdx        # 0x1800f4ac4
    18001783c:	call   0x1800033f0
    180017841:	mov    %rax,%rcx
    180017844:	lea    0xdd235(%rip),%rdx        # 0x1800f4a80
    18001784b:	call   0x1800033f0
    180017850:	mov    %rax,%rcx
-   180017853:	lea    0xdd21e(%rip),%rdx        # 0x1800f4a78
+   180017853:	lea    0xdd216(%rip),%rdx        # 0x1800f4a70
    18001785a:	call   0x1800033f0
    18001785f:	mov    %rax,%rcx
    180017862:	mov    $0x5b,%edx
    180017867:	call   *0xdaa63(%rip)        # 0x1800f22d0
    18001786d:	nop
    18001786e:	lea    0xc0(%rbp),%rcx
    180017875:	call   0x180008870
@@ -53758,15 +53758,15 @@
    180017937:	mov    %rax,%rcx
    18001793a:	lea    0xdd183(%rip),%rdx        # 0x1800f4ac4
    180017941:	call   0x1800033f0
    180017946:	mov    %rax,%rcx
    180017949:	lea    0xdd130(%rip),%rdx        # 0x1800f4a80
    180017950:	call   0x1800033f0
    180017955:	mov    %rax,%rcx
-   180017958:	lea    0xdd119(%rip),%rdx        # 0x1800f4a78
+   180017958:	lea    0xdd111(%rip),%rdx        # 0x1800f4a70
    18001795f:	call   0x1800033f0
    180017964:	mov    %rax,%rcx
    180017967:	mov    $0x7a,%edx
    18001796c:	call   *0xda95e(%rip)        # 0x1800f22d0
    180017972:	nop
    180017973:	lea    0xc0(%rbp),%rcx
    18001797a:	call   0x180008870
@@ -53827,15 +53827,15 @@
    180017a7a:	mov    %rax,%rcx
    180017a7d:	lea    0xdd040(%rip),%rdx        # 0x1800f4ac4
    180017a84:	call   0x1800033f0
    180017a89:	mov    %rax,%rcx
    180017a8c:	lea    0xdcfed(%rip),%rdx        # 0x1800f4a80
    180017a93:	call   0x1800033f0
    180017a98:	mov    %rax,%rcx
-   180017a9b:	lea    0xdcfd6(%rip),%rdx        # 0x1800f4a78
+   180017a9b:	lea    0xdcfce(%rip),%rdx        # 0x1800f4a70
    180017aa2:	call   0x1800033f0
    180017aa7:	mov    %rax,%rcx
    180017aaa:	mov    $0x88,%edx
    180017aaf:	call   *0xda81b(%rip)        # 0x1800f22d0
    180017ab5:	nop
    180017ab6:	lea    0xc0(%rbp),%rcx
    180017abd:	call   0x180008870
@@ -53905,15 +53905,15 @@
    180017be4:	mov    %rax,%rcx
    180017be7:	lea    0xdced6(%rip),%rdx        # 0x1800f4ac4
    180017bee:	call   0x1800033f0
    180017bf3:	mov    %rax,%rcx
    180017bf6:	lea    0xdce83(%rip),%rdx        # 0x1800f4a80
    180017bfd:	call   0x1800033f0
    180017c02:	mov    %rax,%rcx
-   180017c05:	lea    0xdce6c(%rip),%rdx        # 0x1800f4a78
+   180017c05:	lea    0xdce64(%rip),%rdx        # 0x1800f4a70
    180017c0c:	call   0x1800033f0
    180017c11:	mov    %rax,%rcx
    180017c14:	mov    $0xa6,%edx
    180017c19:	call   *0xda6b1(%rip)        # 0x1800f22d0
    180017c1f:	nop
    180017c20:	lea    0xc0(%rbp),%rcx
    180017c27:	call   0x180008870
@@ -53966,15 +53966,15 @@
    180017d01:	mov    %rax,%rcx
    180017d04:	lea    0xdcdb9(%rip),%rdx        # 0x1800f4ac4
    180017d0b:	call   0x1800033f0
    180017d10:	mov    %rax,%rcx
    180017d13:	lea    0xdcd66(%rip),%rdx        # 0x1800f4a80
    180017d1a:	call   0x1800033f0
    180017d1f:	mov    %rax,%rcx
-   180017d22:	lea    0xdcd4f(%rip),%rdx        # 0x1800f4a78
+   180017d22:	lea    0xdcd47(%rip),%rdx        # 0x1800f4a70
    180017d29:	call   0x1800033f0
    180017d2e:	mov    %rax,%rcx
    180017d31:	mov    $0xa7,%edx
    180017d36:	call   *0xda594(%rip)        # 0x1800f22d0
    180017d3c:	nop
    180017d3d:	lea    0xc0(%rbp),%rcx
    180017d44:	call   0x180008870
@@ -54023,15 +54023,15 @@
    180017e06:	mov    %rax,%rcx
    180017e09:	lea    0xdccb4(%rip),%rdx        # 0x1800f4ac4
    180017e10:	call   0x1800033f0
    180017e15:	mov    %rax,%rcx
    180017e18:	lea    0xdcc61(%rip),%rdx        # 0x1800f4a80
    180017e1f:	call   0x1800033f0
    180017e24:	mov    %rax,%rcx
-   180017e27:	lea    0xdcc4a(%rip),%rdx        # 0x1800f4a78
+   180017e27:	lea    0xdcc42(%rip),%rdx        # 0x1800f4a70
    180017e2e:	call   0x1800033f0
    180017e33:	mov    %rax,%rcx
    180017e36:	mov    $0xbe,%edx
    180017e3b:	call   *0xda48f(%rip)        # 0x1800f22d0
    180017e41:	nop
    180017e42:	lea    0xc0(%rbp),%rcx
    180017e49:	call   0x180008870
@@ -54086,15 +54086,15 @@
    180017f1b:	mov    %rax,%rcx
    180017f1e:	lea    0xdcb9f(%rip),%rdx        # 0x1800f4ac4
    180017f25:	call   0x1800033f0
    180017f2a:	mov    %rax,%rcx
    180017f2d:	lea    0xdcb4c(%rip),%rdx        # 0x1800f4a80
    180017f34:	call   0x1800033f0
    180017f39:	mov    %rax,%rcx
-   180017f3c:	lea    0xdcb35(%rip),%rdx        # 0x1800f4a78
+   180017f3c:	lea    0xdcb2d(%rip),%rdx        # 0x1800f4a70
    180017f43:	call   0x1800033f0
    180017f48:	mov    %rax,%rcx
    180017f4b:	mov    $0xc5,%edx
    180017f50:	call   *0xda37a(%rip)        # 0x1800f22d0
    180017f56:	nop
    180017f57:	lea    0xc0(%rbp),%rcx
    180017f5e:	call   0x180008870
@@ -54155,15 +54155,15 @@
    180018044:	mov    %rax,%rcx
    180018047:	lea    0xdca76(%rip),%rdx        # 0x1800f4ac4
    18001804e:	call   0x1800033f0
    180018053:	mov    %rax,%rcx
    180018056:	lea    0xdca23(%rip),%rdx        # 0x1800f4a80
    18001805d:	call   0x1800033f0
    180018062:	mov    %rax,%rcx
-   180018065:	lea    0xdca0c(%rip),%rdx        # 0x1800f4a78
+   180018065:	lea    0xdca04(%rip),%rdx        # 0x1800f4a70
    18001806c:	call   0x1800033f0
    180018071:	mov    %rax,%rcx
    180018074:	mov    $0xc7,%edx
    180018079:	call   *0xda251(%rip)        # 0x1800f22d0
    18001807f:	nop
    180018080:	lea    0xc0(%rbp),%rcx
    180018087:	call   0x180008870
@@ -54216,15 +54216,15 @@
    180018161:	mov    %rax,%rcx
    180018164:	lea    0xdc959(%rip),%rdx        # 0x1800f4ac4
    18001816b:	call   0x1800033f0
    180018170:	mov    %rax,%rcx
    180018173:	lea    0xdc906(%rip),%rdx        # 0x1800f4a80
    18001817a:	call   0x1800033f0
    18001817f:	mov    %rax,%rcx
-   180018182:	lea    0xdc8ef(%rip),%rdx        # 0x1800f4a78
+   180018182:	lea    0xdc8e7(%rip),%rdx        # 0x1800f4a70
    180018189:	call   0x1800033f0
    18001818e:	mov    %rax,%rcx
    180018191:	mov    $0xce,%edx
    180018196:	call   *0xda134(%rip)        # 0x1800f22d0
    18001819c:	nop
    18001819d:	lea    0xc0(%rbp),%rcx
    1800181a4:	call   0x180008870
@@ -54404,28 +54404,28 @@
    18001847c:	lea    0xdb2ed(%rip),%rcx        # 0x1800f3770
    180018483:	xorps  %xmm0,%xmm0
    180018486:	lea    0x8(%rbx),%rdx
    18001848a:	mov    %rcx,(%rbx)
    18001848d:	lea    0x8(%rax),%rcx
    180018491:	movups %xmm0,(%rdx)
    180018494:	call   0x1800e1dec
-   180018499:	lea    0xdc5a8(%rip),%rax        # 0x1800f4a48
+   180018499:	lea    0xdc5a0(%rip),%rax        # 0x1800f4a40
    1800184a0:	mov    %rax,(%rbx)
    1800184a3:	mov    %rbx,%rax
    1800184a6:	add    $0x20,%rsp
    1800184aa:	pop    %rbx
    1800184ab:	ret
    1800184ac:	int3
    1800184ad:	int3
    1800184ae:	int3
    1800184af:	int3
-   1800184b0:	lea    0xdc5a1(%rip),%rax        # 0x1800f4a58
+   1800184b0:	lea    0xdc599(%rip),%rax        # 0x1800f4a50
    1800184b7:	movq   $0x0,0x10(%rcx)
    1800184bf:	mov    %rax,0x8(%rcx)
-   1800184c3:	lea    0xdc57e(%rip),%rax        # 0x1800f4a48
+   1800184c3:	lea    0xdc576(%rip),%rax        # 0x1800f4a40
    1800184ca:	mov    %rax,(%rcx)
    1800184cd:	mov    %rcx,%rax
    1800184d0:	ret
    1800184d1:	int3
    1800184d2:	int3
    1800184d3:	int3
    1800184d4:	int3
@@ -54634,15 +54634,15 @@
    1800186cb:	int3
    1800186cc:	int3
    1800186cd:	int3
    1800186ce:	int3
    1800186cf:	int3
    1800186d0:	rex push %rbx
    1800186d2:	sub    $0x20,%rsp
-   1800186d6:	lea    0xdc393(%rip),%rax        # 0x1800f4a70
+   1800186d6:	lea    0xdc38b(%rip),%rax        # 0x1800f4a68
    1800186dd:	mov    %rcx,%rbx
    1800186e0:	mov    %rax,(%rcx)
    1800186e3:	mov    0x68(%rcx),%rdx
    1800186e7:	cmp    $0x10,%rdx
    1800186eb:	jb     0x18001871e
    1800186ed:	mov    0x50(%rcx),%rcx
    1800186f1:	inc    %rdx
@@ -55200,15 +55200,15 @@
    180018ecc:	int3
    180018ecd:	int3
    180018ece:	int3
    180018ecf:	int3
    180018ed0:	mov    %rbx,0x8(%rsp)
    180018ed5:	push   %rdi
    180018ed6:	sub    $0x20,%rsp
-   180018eda:	lea    0xdbb8f(%rip),%rax        # 0x1800f4a70
+   180018eda:	lea    0xdbb87(%rip),%rax        # 0x1800f4a68
    180018ee1:	mov    %edx,%edi
    180018ee3:	mov    %rax,(%rcx)
    180018ee6:	mov    %rcx,%rbx
    180018ee9:	mov    0x68(%rcx),%rdx
    180018eed:	cmp    $0x10,%rdx
    180018ef1:	jb     0x180018f24
    180018ef3:	mov    0x50(%rcx),%rcx
@@ -56349,15 +56349,15 @@
    180019e6a:	mov    %rax,%rcx
    180019e6d:	lea    0xdac50(%rip),%rdx        # 0x1800f4ac4
    180019e74:	call   0x1800033f0
    180019e79:	mov    %rax,%rcx
    180019e7c:	lea    0xdabfd(%rip),%rdx        # 0x1800f4a80
    180019e83:	call   0x1800033f0
    180019e88:	mov    %rax,%rcx
-   180019e8b:	lea    0xdabe6(%rip),%rdx        # 0x1800f4a78
+   180019e8b:	lea    0xdabde(%rip),%rdx        # 0x1800f4a70
    180019e92:	call   0x1800033f0
    180019e97:	mov    %rax,%rcx
    180019e9a:	mov    $0x2b7,%edx
    180019e9f:	call   *0xd842b(%rip)        # 0x1800f22d0
    180019ea5:	nop
    180019ea6:	lea    0x130(%rsp),%rcx
    180019eae:	call   0x180008870
@@ -58422,15 +58422,15 @@
    18001c5ba:	mov    %rax,%rcx
    18001c5bd:	lea    0xd8500(%rip),%rdx        # 0x1800f4ac4
    18001c5c4:	call   0x1800033f0
    18001c5c9:	mov    %rax,%rcx
    18001c5cc:	lea    0xd84ad(%rip),%rdx        # 0x1800f4a80
    18001c5d3:	call   0x1800033f0
    18001c5d8:	mov    %rax,%rcx
-   18001c5db:	lea    0xd8496(%rip),%rdx        # 0x1800f4a78
+   18001c5db:	lea    0xd848e(%rip),%rdx        # 0x1800f4a70
    18001c5e2:	call   0x1800033f0
    18001c5e7:	mov    %rax,%rcx
    18001c5ea:	mov    $0x206,%edx
    18001c5ef:	call   *0xd5cdb(%rip)        # 0x1800f22d0
    18001c5f5:	lea    0x618(%rsp),%rdx
    18001c5fd:	lea    0x3e0(%rsp),%rcx
    18001c605:	call   0x18000e120
@@ -58482,15 +58482,15 @@
    18001c6d2:	mov    %rax,%rcx
    18001c6d5:	lea    0xd83e8(%rip),%rdx        # 0x1800f4ac4
    18001c6dc:	call   0x1800033f0
    18001c6e1:	mov    %rax,%rcx
    18001c6e4:	lea    0xd8395(%rip),%rdx        # 0x1800f4a80
    18001c6eb:	call   0x1800033f0
    18001c6f0:	mov    %rax,%rcx
-   18001c6f3:	lea    0xd837e(%rip),%rdx        # 0x1800f4a78
+   18001c6f3:	lea    0xd8376(%rip),%rdx        # 0x1800f4a70
    18001c6fa:	call   0x1800033f0
    18001c6ff:	mov    %rax,%rcx
    18001c702:	mov    $0x208,%edx
    18001c707:	call   *0xd5bc3(%rip)        # 0x1800f22d0
    18001c70d:	lea    0x618(%rsp),%rdx
    18001c715:	lea    0x3e0(%rsp),%rcx
    18001c71d:	call   0x18000e120
@@ -58561,15 +58561,15 @@
    18001c844:	mov    %rax,%rcx
    18001c847:	lea    0xd8276(%rip),%rdx        # 0x1800f4ac4
    18001c84e:	call   0x1800033f0
    18001c853:	mov    %rax,%rcx
    18001c856:	lea    0xd8223(%rip),%rdx        # 0x1800f4a80
    18001c85d:	call   0x1800033f0
    18001c862:	mov    %rax,%rcx
-   18001c865:	lea    0xd820c(%rip),%rdx        # 0x1800f4a78
+   18001c865:	lea    0xd8204(%rip),%rdx        # 0x1800f4a70
    18001c86c:	call   0x1800033f0
    18001c871:	mov    %rax,%rcx
    18001c874:	mov    $0x239,%edx
    18001c879:	call   *0xd5a51(%rip)        # 0x1800f22d0
    18001c87f:	nop
    18001c880:	lea    0x658(%rsp),%rcx
    18001c888:	call   0x180008870
@@ -58668,15 +58668,15 @@
    18001ca41:	call   0x1800033f0
    18001ca46:	lea    0xd8077(%rip),%rdx        # 0x1800f4ac4
    18001ca4d:	mov    %rax,%rcx
    18001ca50:	call   0x1800033f0
    18001ca55:	lea    0xd8024(%rip),%rdx        # 0x1800f4a80
    18001ca5c:	mov    %rax,%rcx
    18001ca5f:	call   0x1800033f0
-   18001ca64:	lea    0xd800d(%rip),%rdx        # 0x1800f4a78
+   18001ca64:	lea    0xd8005(%rip),%rdx        # 0x1800f4a70
    18001ca6b:	mov    %rax,%rcx
    18001ca6e:	call   0x1800033f0
    18001ca73:	mov    $0x259,%edx
    18001ca78:	mov    %rax,%rcx
    18001ca7b:	call   *0xd584f(%rip)        # 0x1800f22d0
    18001ca81:	nop
    18001ca82:	lea    0x658(%rsp),%rcx
@@ -59271,15 +59271,15 @@
    18001d355:	mov    %rax,%rcx
    18001d358:	lea    0xd7765(%rip),%rdx        # 0x1800f4ac4
    18001d35f:	call   0x1800033f0
    18001d364:	mov    %rax,%rcx
    18001d367:	lea    0xd7712(%rip),%rdx        # 0x1800f4a80
    18001d36e:	call   0x1800033f0
    18001d373:	mov    %rax,%rcx
-   18001d376:	lea    0xd76fb(%rip),%rdx        # 0x1800f4a78
+   18001d376:	lea    0xd76f3(%rip),%rdx        # 0x1800f4a70
    18001d37d:	call   0x1800033f0
    18001d382:	mov    %rax,%rcx
    18001d385:	mov    $0x338,%edx
    18001d38a:	call   *0xd4f40(%rip)        # 0x1800f22d0
    18001d390:	nop
    18001d391:	lea    0x70(%rbp),%rcx
    18001d395:	call   0x180008870
@@ -59328,15 +59328,15 @@
    18001d453:	mov    %rax,%rcx
    18001d456:	lea    0xd7667(%rip),%rdx        # 0x1800f4ac4
    18001d45d:	call   0x1800033f0
    18001d462:	mov    %rax,%rcx
    18001d465:	lea    0xd7614(%rip),%rdx        # 0x1800f4a80
    18001d46c:	call   0x1800033f0
    18001d471:	mov    %rax,%rcx
-   18001d474:	lea    0xd75fd(%rip),%rdx        # 0x1800f4a78
+   18001d474:	lea    0xd75f5(%rip),%rdx        # 0x1800f4a70
    18001d47b:	call   0x1800033f0
    18001d480:	mov    %rax,%rcx
    18001d483:	mov    $0x336,%edx
    18001d488:	call   *0xd4e42(%rip)        # 0x1800f22d0
    18001d48e:	nop
    18001d48f:	lea    0x70(%rbp),%rcx
    18001d493:	call   0x180008870
@@ -59389,15 +59389,15 @@
    18001d565:	mov    %rax,%rcx
    18001d568:	lea    0xd7555(%rip),%rdx        # 0x1800f4ac4
    18001d56f:	call   0x1800033f0
    18001d574:	mov    %rax,%rcx
    18001d577:	lea    0xd7502(%rip),%rdx        # 0x1800f4a80
    18001d57e:	call   0x1800033f0
    18001d583:	mov    %rax,%rcx
-   18001d586:	lea    0xd74eb(%rip),%rdx        # 0x1800f4a78
+   18001d586:	lea    0xd74e3(%rip),%rdx        # 0x1800f4a70
    18001d58d:	call   0x1800033f0
    18001d592:	mov    %rax,%rcx
    18001d595:	mov    $0x343,%edx
    18001d59a:	call   *0xd4d30(%rip)        # 0x1800f22d0
    18001d5a0:	nop
    18001d5a1:	lea    0x70(%rbp),%rcx
    18001d5a5:	call   0x180008870
@@ -59450,15 +59450,15 @@
    18001d677:	mov    %rax,%rcx
    18001d67a:	lea    0xd7443(%rip),%rdx        # 0x1800f4ac4
    18001d681:	call   0x1800033f0
    18001d686:	mov    %rax,%rcx
    18001d689:	lea    0xd73f0(%rip),%rdx        # 0x1800f4a80
    18001d690:	call   0x1800033f0
    18001d695:	mov    %rax,%rcx
-   18001d698:	lea    0xd73d9(%rip),%rdx        # 0x1800f4a78
+   18001d698:	lea    0xd73d1(%rip),%rdx        # 0x1800f4a70
    18001d69f:	call   0x1800033f0
    18001d6a4:	mov    %rax,%rcx
    18001d6a7:	mov    $0x342,%edx
    18001d6ac:	call   *0xd4c1e(%rip)        # 0x1800f22d0
    18001d6b2:	nop
    18001d6b3:	lea    0x70(%rbp),%rcx
    18001d6b7:	call   0x180008870
@@ -59511,15 +59511,15 @@
    18001d789:	mov    %rax,%rcx
    18001d78c:	lea    0xd7331(%rip),%rdx        # 0x1800f4ac4
    18001d793:	call   0x1800033f0
    18001d798:	mov    %rax,%rcx
    18001d79b:	lea    0xd72de(%rip),%rdx        # 0x1800f4a80
    18001d7a2:	call   0x1800033f0
    18001d7a7:	mov    %rax,%rcx
-   18001d7aa:	lea    0xd72c7(%rip),%rdx        # 0x1800f4a78
+   18001d7aa:	lea    0xd72bf(%rip),%rdx        # 0x1800f4a70
    18001d7b1:	call   0x1800033f0
    18001d7b6:	mov    %rax,%rcx
    18001d7b9:	mov    $0x33b,%edx
    18001d7be:	call   *0xd4b0c(%rip)        # 0x1800f22d0
    18001d7c4:	nop
    18001d7c5:	lea    0x70(%rbp),%rcx
    18001d7c9:	call   0x180008870
@@ -59572,15 +59572,15 @@
    18001d89b:	mov    %rax,%rcx
    18001d89e:	lea    0xd721f(%rip),%rdx        # 0x1800f4ac4
    18001d8a5:	call   0x1800033f0
    18001d8aa:	mov    %rax,%rcx
    18001d8ad:	lea    0xd71cc(%rip),%rdx        # 0x1800f4a80
    18001d8b4:	call   0x1800033f0
    18001d8b9:	mov    %rax,%rcx
-   18001d8bc:	lea    0xd71b5(%rip),%rdx        # 0x1800f4a78
+   18001d8bc:	lea    0xd71ad(%rip),%rdx        # 0x1800f4a70
    18001d8c3:	call   0x1800033f0
    18001d8c8:	mov    %rax,%rcx
    18001d8cb:	mov    $0x33a,%edx
    18001d8d0:	call   *0xd49fa(%rip)        # 0x1800f22d0
    18001d8d6:	nop
    18001d8d7:	lea    0x70(%rbp),%rcx
    18001d8db:	call   0x180008870
@@ -60328,15 +60328,15 @@
    18001e3fd:	mov    %rax,%rcx
    18001e400:	lea    0xd66bd(%rip),%rdx        # 0x1800f4ac4
    18001e407:	call   0x1800033f0
    18001e40c:	mov    %rax,%rcx
    18001e40f:	lea    0xd666a(%rip),%rdx        # 0x1800f4a80
    18001e416:	call   0x1800033f0
    18001e41b:	mov    %rax,%rcx
-   18001e41e:	lea    0xd6653(%rip),%rdx        # 0x1800f4a78
+   18001e41e:	lea    0xd664b(%rip),%rdx        # 0x1800f4a70
    18001e425:	call   0x1800033f0
    18001e42a:	mov    %rax,%rcx
    18001e42d:	mov    $0x197,%edx
    18001e432:	call   *0xd3e98(%rip)        # 0x1800f22d0
    18001e438:	nop
    18001e439:	lea    0x40(%rbp),%rcx
    18001e43d:	call   0x180008870
@@ -60389,15 +60389,15 @@
    18001e501:	mov    %rax,%rcx
    18001e504:	lea    0xd65b9(%rip),%rdx        # 0x1800f4ac4
    18001e50b:	call   0x1800033f0
    18001e510:	mov    %rax,%rcx
    18001e513:	lea    0xd6566(%rip),%rdx        # 0x1800f4a80
    18001e51a:	call   0x1800033f0
    18001e51f:	mov    %rax,%rcx
-   18001e522:	lea    0xd654f(%rip),%rdx        # 0x1800f4a78
+   18001e522:	lea    0xd6547(%rip),%rdx        # 0x1800f4a70
    18001e529:	call   0x1800033f0
    18001e52e:	mov    %rax,%rcx
    18001e531:	mov    $0x18b,%edx
    18001e536:	call   *0xd3d94(%rip)        # 0x1800f22d0
    18001e53c:	nop
    18001e53d:	lea    0x40(%rbp),%rcx
    18001e541:	call   0x180008870
@@ -60450,15 +60450,15 @@
    18001e605:	mov    %rax,%rcx
    18001e608:	lea    0xd64b5(%rip),%rdx        # 0x1800f4ac4
    18001e60f:	call   0x1800033f0
    18001e614:	mov    %rax,%rcx
    18001e617:	lea    0xd6462(%rip),%rdx        # 0x1800f4a80
    18001e61e:	call   0x1800033f0
    18001e623:	mov    %rax,%rcx
-   18001e626:	lea    0xd644b(%rip),%rdx        # 0x1800f4a78
+   18001e626:	lea    0xd6443(%rip),%rdx        # 0x1800f4a70
    18001e62d:	call   0x1800033f0
    18001e632:	mov    %rax,%rcx
    18001e635:	mov    $0x191,%edx
    18001e63a:	call   *0xd3c90(%rip)        # 0x1800f22d0
    18001e640:	nop
    18001e641:	lea    0x40(%rbp),%rcx
    18001e645:	call   0x180008870
@@ -60511,15 +60511,15 @@
    18001e71c:	mov    %rax,%rcx
    18001e71f:	lea    0xd639e(%rip),%rdx        # 0x1800f4ac4
    18001e726:	call   0x1800033f0
    18001e72b:	mov    %rax,%rcx
    18001e72e:	lea    0xd634b(%rip),%rdx        # 0x1800f4a80
    18001e735:	call   0x1800033f0
    18001e73a:	mov    %rax,%rcx
-   18001e73d:	lea    0xd6334(%rip),%rdx        # 0x1800f4a78
+   18001e73d:	lea    0xd632c(%rip),%rdx        # 0x1800f4a70
    18001e744:	call   0x1800033f0
    18001e749:	mov    %rax,%rcx
    18001e74c:	mov    $0x186,%edx
    18001e751:	call   *0xd3b79(%rip)        # 0x1800f22d0
    18001e757:	nop
    18001e758:	lea    0x40(%rbp),%rcx
    18001e75c:	call   0x180008870
@@ -64701,15 +64701,15 @@
    18002281a:	jne    0x18002292a
    180022820:	test   %dil,%dil
    180022823:	jne    0x18002292a
    180022829:	mov    $0x1,%r12b
    18002282c:	xor    %bl,%bl
    18002282e:	mov    %bl,0x28(%rsp)
    180022832:	lea    0xd3f5b(%rip),%rax        # 0x1800f6794
-   180022839:	lea    0xd21f8(%rip),%rdx        # 0x1800f4a38
+   180022839:	lea    0xd21f4(%rip),%rdx        # 0x1800f4a34
    180022840:	test   %r12b,%r12b
    180022843:	cmovne %rax,%rdx
    180022847:	xor    %r15d,%r15d
    18002284a:	mov    %r15,0x98(%rbp)
    180022851:	mov    %r15,0xa8(%rbp)
    180022858:	movq   $0xf,0xb0(%rbp)
    180022863:	mov    %r15b,0x98(%rbp)
@@ -65912,15 +65912,15 @@
    180023bbe:	mov    %rax,%rcx
    180023bc1:	lea    0xd0efc(%rip),%rdx        # 0x1800f4ac4
    180023bc8:	call   0x1800033f0
    180023bcd:	mov    %rax,%rcx
    180023bd0:	lea    0xd2df9(%rip),%rdx        # 0x1800f69d0
    180023bd7:	call   0x1800033f0
    180023bdc:	mov    %rax,%rcx
-   180023bdf:	lea    0xd0e92(%rip),%rdx        # 0x1800f4a78
+   180023bdf:	lea    0xd0e8a(%rip),%rdx        # 0x1800f4a70
    180023be6:	call   0x1800033f0
    180023beb:	mov    %rax,%rcx
    180023bee:	mov    $0x2e,%edx
    180023bf3:	call   *0xce6d7(%rip)        # 0x1800f22d0
    180023bf9:	nop
    180023bfa:	lea    0x30(%rbp),%rcx
    180023bfe:	call   0x180008870
@@ -65975,15 +65975,15 @@
    180023ccf:	mov    %rax,%rcx
    180023cd2:	lea    0xd0deb(%rip),%rdx        # 0x1800f4ac4
    180023cd9:	call   0x1800033f0
    180023cde:	mov    %rax,%rcx
    180023ce1:	lea    0xd2ce8(%rip),%rdx        # 0x1800f69d0
    180023ce8:	call   0x1800033f0
    180023ced:	mov    %rax,%rcx
-   180023cf0:	lea    0xd0d81(%rip),%rdx        # 0x1800f4a78
+   180023cf0:	lea    0xd0d79(%rip),%rdx        # 0x1800f4a70
    180023cf7:	call   0x1800033f0
    180023cfc:	mov    %rax,%rcx
    180023cff:	mov    $0x2c,%edx
    180023d04:	call   *0xce5c6(%rip)        # 0x1800f22d0
    180023d0a:	nop
    180023d0b:	lea    0x30(%rbp),%rcx
    180023d0f:	call   0x180008870
@@ -66036,15 +66036,15 @@
    180023dd6:	mov    %rax,%rcx
    180023dd9:	lea    0xd0ce4(%rip),%rdx        # 0x1800f4ac4
    180023de0:	call   0x1800033f0
    180023de5:	mov    %rax,%rcx
    180023de8:	lea    0xd2be1(%rip),%rdx        # 0x1800f69d0
    180023def:	call   0x1800033f0
    180023df4:	mov    %rax,%rcx
-   180023df7:	lea    0xd0c7a(%rip),%rdx        # 0x1800f4a78
+   180023df7:	lea    0xd0c72(%rip),%rdx        # 0x1800f4a70
    180023dfe:	call   0x1800033f0
    180023e03:	mov    %rax,%rcx
    180023e06:	mov    $0x2d,%edx
    180023e0b:	call   *0xce4bf(%rip)        # 0x1800f22d0
    180023e11:	nop
    180023e12:	lea    0x30(%rbp),%rcx
    180023e16:	call   0x180008870
@@ -66531,15 +66531,15 @@
    180024528:	mov    %rax,%rcx
    18002452b:	lea    0xd0592(%rip),%rdx        # 0x1800f4ac4
    180024532:	call   0x1800033f0
    180024537:	mov    %rax,%rcx
    18002453a:	lea    0xd248f(%rip),%rdx        # 0x1800f69d0
    180024541:	call   0x1800033f0
    180024546:	mov    %rax,%rcx
-   180024549:	lea    0xd0528(%rip),%rdx        # 0x1800f4a78
+   180024549:	lea    0xd0520(%rip),%rdx        # 0x1800f4a70
    180024550:	call   0x1800033f0
    180024555:	mov    %rax,%rcx
    180024558:	mov    $0x78,%edx
    18002455d:	call   *0xcdd6d(%rip)        # 0x1800f22d0
    180024563:	nop
    180024564:	lea    0x190(%rbp),%rcx
    18002456b:	call   0x180008870
@@ -66588,15 +66588,15 @@
    180024637:	mov    %rax,%rcx
    18002463a:	lea    0xd0483(%rip),%rdx        # 0x1800f4ac4
    180024641:	call   0x1800033f0
    180024646:	mov    %rax,%rcx
    180024649:	lea    0xd2380(%rip),%rdx        # 0x1800f69d0
    180024650:	call   0x1800033f0
    180024655:	mov    %rax,%rcx
-   180024658:	lea    0xd0419(%rip),%rdx        # 0x1800f4a78
+   180024658:	lea    0xd0411(%rip),%rdx        # 0x1800f4a70
    18002465f:	call   0x1800033f0
    180024664:	mov    %rax,%rcx
    180024667:	mov    $0x7e,%edx
    18002466c:	call   *0xcdc5e(%rip)        # 0x1800f22d0
    180024672:	nop
    180024673:	lea    0x190(%rbp),%rcx
    18002467a:	call   0x180008870
@@ -91314,15 +91314,15 @@
    18003bb74:	lea    0x310(%rsp),%rcx
    18003bb7c:	call   0x180004f90
    18003bb81:	nop
    18003bb82:	mov    0x38(%r12),%rcx
    18003bb87:	mov    0x680(%r12),%rdi
    18003bb8f:	mov    (%rcx),%rax
    18003bb92:	call   *0xa8(%rax)
-   18003bb98:	imul   0xb8e1d(%rip),%eax        # 0x1800f49bc
+   18003bb98:	imul   0xb8e2d(%rip),%eax        # 0x1800f49cc
    18003bb9f:	movslq %eax,%r8
    18003bba2:	lea    0x310(%rsp),%rax
    18003bbaa:	mov    %rax,0x20(%rsp)
    18003bbaf:	mov    %esi,%r9d
    18003bbb2:	mov    0x38(%r12),%rdx
    18003bbb7:	lea    0x680(%r12),%rcx
    18003bbbf:	call   *0x8(%rdi)
@@ -93548,15 +93548,15 @@
    18003e63f:	mov    %rax,%rcx
    18003e642:	lea    0xb647b(%rip),%rdx        # 0x1800f4ac4
    18003e649:	call   0x1800033f0
    18003e64e:	mov    %rax,%rcx
    18003e651:	lea    0xb9fc8(%rip),%rdx        # 0x1800f8620
    18003e658:	call   0x1800033f0
    18003e65d:	mov    %rax,%rcx
-   18003e660:	lea    0xb6411(%rip),%rdx        # 0x1800f4a78
+   18003e660:	lea    0xb6409(%rip),%rdx        # 0x1800f4a70
    18003e667:	call   0x1800033f0
    18003e66c:	mov    %rax,%rcx
    18003e66f:	mov    $0x376,%edx
    18003e674:	call   *0xb3c56(%rip)        # 0x1800f22d0
    18003e67a:	nop
    18003e67b:	lea    0x330(%rsp),%rcx
    18003e683:	call   0x180008870
@@ -93611,15 +93611,15 @@
    18003e771:	mov    %rax,%rcx
    18003e774:	lea    0xb6349(%rip),%rdx        # 0x1800f4ac4
    18003e77b:	call   0x1800033f0
    18003e780:	mov    %rax,%rcx
    18003e783:	lea    0xb9e96(%rip),%rdx        # 0x1800f8620
    18003e78a:	call   0x1800033f0
    18003e78f:	mov    %rax,%rcx
-   18003e792:	lea    0xb62df(%rip),%rdx        # 0x1800f4a78
+   18003e792:	lea    0xb62d7(%rip),%rdx        # 0x1800f4a70
    18003e799:	call   0x1800033f0
    18003e79e:	mov    %rax,%rcx
    18003e7a1:	mov    $0x377,%edx
    18003e7a6:	call   *0xb3b24(%rip)        # 0x1800f22d0
    18003e7ac:	nop
    18003e7ad:	lea    0x330(%rsp),%rcx
    18003e7b5:	call   0x180008870
@@ -97138,15 +97138,15 @@
    1800418b5:	mov    %rax,%rcx
    1800418b8:	lea    0xb3205(%rip),%rdx        # 0x1800f4ac4
    1800418bf:	call   0x1800033f0
    1800418c4:	mov    %rax,%rcx
    1800418c7:	lea    0xb73e2(%rip),%rdx        # 0x1800f8cb0
    1800418ce:	call   0x1800033f0
    1800418d3:	mov    %rax,%rcx
-   1800418d6:	lea    0xb319b(%rip),%rdx        # 0x1800f4a78
+   1800418d6:	lea    0xb3193(%rip),%rdx        # 0x1800f4a70
    1800418dd:	call   0x1800033f0
    1800418e2:	mov    %rax,%rcx
    1800418e5:	mov    $0x4a,%edx
    1800418ea:	call   *0xb09e0(%rip)        # 0x1800f22d0
    1800418f0:	nop
    1800418f1:	lea    0x60(%rbp),%rcx
    1800418f5:	call   0x180008870
@@ -97203,15 +97203,15 @@
    1800419d1:	mov    %rax,%rcx
    1800419d4:	lea    0xb30e9(%rip),%rdx        # 0x1800f4ac4
    1800419db:	call   0x1800033f0
    1800419e0:	mov    %rax,%rcx
    1800419e3:	lea    0xb72c6(%rip),%rdx        # 0x1800f8cb0
    1800419ea:	call   0x1800033f0
    1800419ef:	mov    %rax,%rcx
-   1800419f2:	lea    0xb307f(%rip),%rdx        # 0x1800f4a78
+   1800419f2:	lea    0xb3077(%rip),%rdx        # 0x1800f4a70
    1800419f9:	call   0x1800033f0
    1800419fe:	mov    %rax,%rcx
    180041a01:	mov    $0x48,%edx
    180041a06:	call   *0xb08c4(%rip)        # 0x1800f22d0
    180041a0c:	nop
    180041a0d:	lea    0x60(%rbp),%rcx
    180041a11:	call   0x180008870
@@ -97266,15 +97266,15 @@
    180041add:	mov    %rax,%rcx
    180041ae0:	lea    0xb2fdd(%rip),%rdx        # 0x1800f4ac4
    180041ae7:	call   0x1800033f0
    180041aec:	mov    %rax,%rcx
    180041aef:	lea    0xb71ba(%rip),%rdx        # 0x1800f8cb0
    180041af6:	call   0x1800033f0
    180041afb:	mov    %rax,%rcx
-   180041afe:	lea    0xb2f73(%rip),%rdx        # 0x1800f4a78
+   180041afe:	lea    0xb2f6b(%rip),%rdx        # 0x1800f4a70
    180041b05:	call   0x1800033f0
    180041b0a:	mov    %rax,%rcx
    180041b0d:	mov    $0x49,%edx
    180041b12:	call   *0xb07b8(%rip)        # 0x1800f22d0
    180041b18:	nop
    180041b19:	lea    0x60(%rbp),%rcx
    180041b1d:	call   0x180008870
@@ -98280,15 +98280,15 @@
    180042a02:	jl     0x180042a09
    180042a04:	cmp    %rax,%rdx
    180042a07:	jne    0x180042a2c
    180042a09:	lea    0x30(%rsp),%rdx
    180042a0e:	lea    0x618(%r14),%rcx
    180042a15:	call   0x180042080
    180042a1a:	xor    %r8d,%r8d
-   180042a1d:	lea    0xb2014(%rip),%rdx        # 0x1800f4a38
+   180042a1d:	lea    0xb2010(%rip),%rdx        # 0x1800f4a34
    180042a24:	mov    %rax,%rcx
    180042a27:	call   0x18000c600
    180042a2c:	xor    %esi,%esi
    180042a2e:	mov    %rsi,0x38(%rsp)
    180042a33:	mov    %rsi,0x40(%rsp)
    180042a38:	lea    0x60(%rsi),%ecx
    180042a3b:	call   0x1800e0a40
@@ -100999,15 +100999,15 @@
    180045951:	nop
    180045952:	lea    0xc40(%rbp),%rcx
    180045959:	call   0x180008870
    18004595e:	lea    0xb368b(%rip),%rdx        # 0x1800f8ff0
    180045965:	lea    0xca0(%rbp),%rcx
    18004596c:	call   0x180004f90
    180045971:	nop
-   180045972:	mov    0xaf0a7(%rip),%r8d        # 0x1800f4a20
+   180045972:	mov    0xaf0b7(%rip),%r8d        # 0x1800f4a30
    180045979:	lea    0xc20(%rbp),%rdx
    180045980:	mov    0x8(%r15),%rcx
    180045984:	call   0x1800c8ed0
    180045989:	mov    %rax,%rbx
    18004598c:	lea    0xca0(%rbp),%rdx
    180045993:	lea    0x48(%rsp),%rcx
    180045998:	call   0x18000f7f0
@@ -101495,15 +101495,15 @@
    18004615f:	movq   $0xf,0x58(%rbp)
    180046167:	movq   $0x9,0x50(%rbp)
    18004616f:	movsd  0xb2e79(%rip),%xmm0        # 0x1800f8ff0
    180046177:	movsd  %xmm0,0x40(%rbp)
    18004617c:	movzbl 0xb2e75(%rip),%eax        # 0x1800f8ff8
    180046183:	mov    %al,0x48(%rbp)
    180046186:	movb   $0x0,0x49(%rbp)
-   18004618a:	mov    0xae88f(%rip),%r8d        # 0x1800f4a20
+   18004618a:	mov    0xae89f(%rip),%r8d        # 0x1800f4a30
    180046191:	lea    0x60(%rbp),%rdx
    180046195:	mov    0x8(%r14),%rcx
    180046199:	call   0x1800c8ed0
    18004619e:	mov    %rax,-0x58(%rbp)
    1800461a2:	mov    0x40(%rsp),%rdi
    1800461a7:	mov    %rdi,0x60(%rsp)
    1800461ac:	mov    0x8(%rdi),%rbx
@@ -102706,15 +102706,15 @@
    180047356:	mov    %rdx,%rax
    180047359:	shr    $0x3f,%rax
    18004735d:	add    %rax,%rdx
    180047360:	mov    $0x1,%r11d
    180047366:	test   %edx,%edx
    180047368:	jle    0x18004750c
    18004736e:	mov    %rdi,%rbx
-   180047371:	mov    0xad6a8(%rip),%r10d        # 0x1800f4a20
+   180047371:	mov    0xad6b8(%rip),%r10d        # 0x1800f4a30
    180047378:	nopl   0x0(%rax,%rax,1)
    180047380:	mov    %r9d,%eax
    180047383:	cltd
    180047384:	idiv   %r10d
    180047387:	mov    %eax,%r14d
    18004738a:	mov    %edi,%r15d
    18004738d:	mov    0x8(%r8,%rbx,1),%rcx
@@ -102782,15 +102782,15 @@
    18004747b:	movups -0x80(%rbp),%xmm0
    18004747f:	movaps %xmm0,-0x40(%rbp)
    180047483:	mov    %rax,%r8
    180047486:	lea    -0x40(%rbp),%rdx
    18004748a:	lea    -0x58(%rbp),%rcx
    18004748e:	call   0x18000f9e0
    180047493:	mov    -0x58(%rbp),%rsi
-   180047497:	mov    0xad582(%rip),%r10d        # 0x1800f4a20
+   180047497:	mov    0xad592(%rip),%r10d        # 0x1800f4a30
    18004749e:	mov    $0x1,%r11d
    1800474a4:	inc    %r15d
    1800474a7:	add    $0x4,%r12
    1800474ab:	mov    0x5a8(%r13),%r8
    1800474b2:	mov    0x8(%rbx,%r8,1),%rax
    1800474b7:	sub    (%rbx,%r8,1),%rax
    1800474bb:	sar    $0x2,%rax
@@ -103242,15 +103242,15 @@
    180047ba5:	movq   $0xf,0x78(%rbp)
    180047bad:	movb   $0x0,0x60(%rbp)
    180047bb1:	mov    $0xa,%r8d
    180047bb7:	lea    0xb12ba(%rip),%rdx        # 0x1800f8e78
    180047bbe:	lea    0x60(%rbp),%rcx
    180047bc2:	call   0x18000c600
    180047bc7:	nop
-   180047bc8:	movslq 0xace51(%rip),%r8        # 0x1800f4a20
+   180047bc8:	movslq 0xace61(%rip),%r8        # 0x1800f4a30
    180047bcf:	imul   -0x50(%rbp),%r8
    180047bd4:	lea    0x68(%r13),%rbx
    180047bd8:	mov    (%rbx),%rax
    180047bdb:	lea    0x60(%rbp),%rcx
    180047bdf:	mov    %rcx,0x20(%rsp)
    180047be4:	mov    %r12d,%r9d
    180047be7:	mov    0x8(%r13),%rdx
@@ -103298,15 +103298,15 @@
    180047c80:	shr    $0x3f,%rax
    180047c84:	add    %rax,%rdx
    180047c87:	test   %edx,%edx
    180047c89:	jle    0x180047f99
    180047c8f:	mov    %r10,%r8
    180047c92:	mov    %rdi,%r15
    180047c95:	mov    0x60(%rbp),%r12
-   180047c99:	mov    0xacd80(%rip),%r9d        # 0x1800f4a20
+   180047c99:	mov    0xacd90(%rip),%r9d        # 0x1800f4a30
    180047ca0:	mov    %r14d,%eax
    180047ca3:	cltd
    180047ca4:	idiv   %r9d
    180047ca7:	mov    %eax,%ebx
    180047ca9:	mov    %eax,%ecx
    180047cab:	imul   %r9d,%ecx
    180047caf:	mov    %r14d,%eax
@@ -103387,15 +103387,15 @@
    180047dcc:	mov    %rdi,0x10(%rbp)
    180047dd0:	movups 0x20(%rbp),%xmm0
    180047dd4:	movaps %xmm0,0x20(%rbp)
    180047dd8:	lea    0x20(%rbp),%rdx
    180047ddc:	lea    0x68(%rsp),%rcx
    180047de1:	call   0x18000f9e0
    180047de6:	mov    %rax,%rdx
-   180047de9:	mov    0xacc30(%rip),%r9d        # 0x1800f4a20
+   180047de9:	mov    0xacc40(%rip),%r9d        # 0x1800f4a30
    180047df0:	mov    0x50(%rsp),%r10
    180047df5:	mov    0x44(%rsp),%r11d
    180047dfa:	mov    0x24(%rdx),%eax
    180047dfd:	imul   %r9d,%eax
    180047e01:	add    -0x68(%rbp),%eax
    180047e04:	mov    %r14d,%ecx
    180047e07:	jmp    0x180047ef5
@@ -103446,15 +103446,15 @@
    180047ebb:	mov    %rdi,-0x38(%rbp)
    180047ebf:	movups 0x20(%rbp),%xmm0
    180047ec3:	movaps %xmm0,0x20(%rbp)
    180047ec7:	lea    0x20(%rbp),%rdx
    180047ecb:	lea    0x68(%rsp),%rcx
    180047ed0:	call   0x18000f9e0
    180047ed5:	mov    %rax,%rdx
-   180047ed8:	mov    0xacb41(%rip),%r9d        # 0x1800f4a20
+   180047ed8:	mov    0xacb51(%rip),%r9d        # 0x1800f4a30
    180047edf:	mov    0x50(%rsp),%r10
    180047ee4:	mov    0x44(%rsp),%r11d
    180047ee9:	imul   0x24(%rdx),%r9d
    180047eee:	lea    (%r9,%r14,1),%eax
    180047ef2:	mov    -0x68(%rbp),%ecx
    180047ef5:	mov    $0x1,%edx
    180047efa:	movslq %eax,%r8
@@ -103468,15 +103468,15 @@
    180047f15:	mov    %r10,0x50(%rsp)
    180047f1a:	lea    0x5a8(%r13),%rsi
    180047f21:	mov    (%rsi),%r10
    180047f24:	mov    0x8(%r15,%r10,1),%rax
    180047f29:	sub    (%r15,%r10,1),%rax
    180047f2d:	sar    $0x2,%rax
    180047f31:	mov    %r10,%r8
-   180047f34:	mov    0xacae5(%rip),%r9d        # 0x1800f4a20
+   180047f34:	mov    0xacaf5(%rip),%r9d        # 0x1800f4a30
    180047f3b:	cmp    %eax,%r11d
    180047f3e:	jge    0x180047f4a
    180047f40:	mov    0x50(%rsp),%r10
    180047f45:	jmp    0x180047ce0
    180047f4a:	mov    0x48(%rsp),%r14d
    180047f4f:	inc    %r14d
    180047f52:	mov    %r14d,0x48(%rsp)
@@ -103565,15 +103565,15 @@
    1800480bb:	movb   $0x0,0x20(%rbp)
    1800480bf:	mov    $0x10,%r8d
    1800480c5:	lea    0xb0dd4(%rip),%rdx        # 0x1800f8ea0
    1800480cc:	lea    0x20(%rbp),%rcx
    1800480d0:	call   0x18000c600
    1800480d5:	nop
    1800480d6:	mov    0x658(%r13),%r8d
-   1800480dd:	imul   0xac93b(%rip),%r8d        # 0x1800f4a20
+   1800480dd:	imul   0xac94b(%rip),%r8d        # 0x1800f4a30
    1800480e5:	lea    0x188(%r13),%rcx
    1800480ec:	mov    (%rcx),%rax
    1800480ef:	lea    0x20(%rbp),%rdx
    1800480f3:	mov    %rdx,0x20(%rsp)
    1800480f8:	mov    %r12d,%r9d
    1800480fb:	mov    0x8(%r13),%rdx
    1800480ff:	call   *0x8(%rax)
@@ -105262,15 +105262,15 @@
    180049ba6:	mov    %ecx,0x658(%rbx)
    180049bac:	mov    %ecx,%edx
    180049bae:	lea    0x140(%rbx),%rcx
    180049bb5:	mov    (%rcx),%rax
    180049bb8:	call   *0x10(%rax)
    180049bbb:	mov    0x658(%rbx),%edx
    180049bc1:	lea    0x188(%rbx),%rcx
-   180049bc8:	movslq 0xaae51(%rip),%rax        # 0x1800f4a20
+   180049bc8:	movslq 0xaae61(%rip),%rax        # 0x1800f4a30
    180049bcf:	mov    (%rcx),%r8
    180049bd2:	imul   %rax,%rdx
    180049bd6:	call   *0x10(%r8)
    180049bda:	mov    0x548(%rbx),%rdx
    180049be1:	lea    0x150(%rbx),%rcx
    180049be8:	mov    0x550(%rbx),%rax
    180049bef:	sub    %rdx,%rax
@@ -109598,15 +109598,15 @@
    18004daf5:	mov    %rax,%rcx
    18004daf8:	lea    0xa6fc5(%rip),%rdx        # 0x1800f4ac4
    18004daff:	call   0x1800033f0
    18004db04:	mov    %rax,%rcx
    18004db07:	lea    0xabe72(%rip),%rdx        # 0x1800f9980
    18004db0e:	call   0x1800033f0
    18004db13:	mov    %rax,%rcx
-   18004db16:	lea    0xa6f5b(%rip),%rdx        # 0x1800f4a78
+   18004db16:	lea    0xa6f53(%rip),%rdx        # 0x1800f4a70
    18004db1d:	call   0x1800033f0
    18004db22:	mov    %rax,%rcx
    18004db25:	mov    $0xe3,%edx
    18004db2a:	call   *0xa47a0(%rip)        # 0x1800f22d0
    18004db30:	nop
    18004db31:	lea    0x60(%rbp),%rcx
    18004db35:	call   0x180008870
@@ -109675,15 +109675,15 @@
    18004dc54:	mov    %rax,%rcx
    18004dc57:	lea    0xa6e66(%rip),%rdx        # 0x1800f4ac4
    18004dc5e:	call   0x1800033f0
    18004dc63:	mov    %rax,%rcx
    18004dc66:	lea    0xabd13(%rip),%rdx        # 0x1800f9980
    18004dc6d:	call   0x1800033f0
    18004dc72:	mov    %rax,%rcx
-   18004dc75:	lea    0xa6dfc(%rip),%rdx        # 0x1800f4a78
+   18004dc75:	lea    0xa6df4(%rip),%rdx        # 0x1800f4a70
    18004dc7c:	call   0x1800033f0
    18004dc81:	mov    %rax,%rcx
    18004dc84:	mov    $0xd3,%edx
    18004dc89:	call   *0xa4641(%rip)        # 0x1800f22d0
    18004dc8f:	nop
    18004dc90:	lea    0x60(%rbp),%rcx
    18004dc94:	call   0x180008870
@@ -109754,15 +109754,15 @@
    18004ddaf:	mov    %rax,%rcx
    18004ddb2:	lea    0xa6d0b(%rip),%rdx        # 0x1800f4ac4
    18004ddb9:	call   0x1800033f0
    18004ddbe:	mov    %rax,%rcx
    18004ddc1:	lea    0xabbb8(%rip),%rdx        # 0x1800f9980
    18004ddc8:	call   0x1800033f0
    18004ddcd:	mov    %rax,%rcx
-   18004ddd0:	lea    0xa6ca1(%rip),%rdx        # 0x1800f4a78
+   18004ddd0:	lea    0xa6c99(%rip),%rdx        # 0x1800f4a70
    18004ddd7:	call   0x1800033f0
    18004dddc:	mov    %rax,%rcx
    18004dddf:	mov    $0xd4,%edx
    18004dde4:	call   *0xa44e6(%rip)        # 0x1800f22d0
    18004ddea:	nop
    18004ddeb:	lea    0x60(%rbp),%rcx
    18004ddef:	call   0x180008870
@@ -111726,15 +111726,15 @@
    18004f85d:	mov    %rax,%rcx
    18004f860:	lea    0xa525d(%rip),%rdx        # 0x1800f4ac4
    18004f867:	call   0x1800033f0
    18004f86c:	mov    %rax,%rcx
    18004f86f:	lea    0xaa10a(%rip),%rdx        # 0x1800f9980
    18004f876:	call   0x1800033f0
    18004f87b:	mov    %rax,%rcx
-   18004f87e:	lea    0xa51f3(%rip),%rdx        # 0x1800f4a78
+   18004f87e:	lea    0xa51eb(%rip),%rdx        # 0x1800f4a70
    18004f885:	call   0x1800033f0
    18004f88a:	mov    %rax,%rcx
    18004f88d:	mov    $0x7b,%edx
    18004f892:	call   *0xa2a38(%rip)        # 0x1800f22d0
    18004f898:	nop
    18004f899:	lea    0x140(%rsp),%rcx
    18004f8a1:	call   0x180008870
@@ -111781,15 +111781,15 @@
    18004f960:	mov    %rax,%rcx
    18004f963:	lea    0xa515a(%rip),%rdx        # 0x1800f4ac4
    18004f96a:	call   0x1800033f0
    18004f96f:	mov    %rax,%rcx
    18004f972:	lea    0xaa007(%rip),%rdx        # 0x1800f9980
    18004f979:	call   0x1800033f0
    18004f97e:	mov    %rax,%rcx
-   18004f981:	lea    0xa50f0(%rip),%rdx        # 0x1800f4a78
+   18004f981:	lea    0xa50e8(%rip),%rdx        # 0x1800f4a70
    18004f988:	call   0x1800033f0
    18004f98d:	mov    %rax,%rcx
    18004f990:	mov    $0x6f,%edx
    18004f995:	call   *0xa2935(%rip)        # 0x1800f22d0
    18004f99b:	nop
    18004f99c:	lea    0x140(%rsp),%rcx
    18004f9a4:	call   0x180008870
@@ -112984,15 +112984,15 @@
    180050a0c:	mov    %rax,%rcx
    180050a0f:	lea    0xa40ae(%rip),%rdx        # 0x1800f4ac4
    180050a16:	call   0x1800033f0
    180050a1b:	mov    %rax,%rcx
    180050a1e:	lea    0xa8f5b(%rip),%rdx        # 0x1800f9980
    180050a25:	call   0x1800033f0
    180050a2a:	mov    %rax,%rcx
-   180050a2d:	lea    0xa4044(%rip),%rdx        # 0x1800f4a78
+   180050a2d:	lea    0xa403c(%rip),%rdx        # 0x1800f4a70
    180050a34:	call   0x1800033f0
    180050a39:	mov    %rax,%rcx
    180050a3c:	mov    $0xc9,%edx
    180050a41:	call   *0xa1889(%rip)        # 0x1800f22d0
    180050a47:	nop
    180050a48:	lea    0x70(%rbp),%rcx
    180050a4c:	call   0x180008870
@@ -113047,15 +113047,15 @@
    180050b1a:	mov    %rax,%rcx
    180050b1d:	lea    0xa3fa0(%rip),%rdx        # 0x1800f4ac4
    180050b24:	call   0x1800033f0
    180050b29:	mov    %rax,%rcx
    180050b2c:	lea    0xa8e4d(%rip),%rdx        # 0x1800f9980
    180050b33:	call   0x1800033f0
    180050b38:	mov    %rax,%rcx
-   180050b3b:	lea    0xa3f36(%rip),%rdx        # 0x1800f4a78
+   180050b3b:	lea    0xa3f2e(%rip),%rdx        # 0x1800f4a70
    180050b42:	call   0x1800033f0
    180050b47:	mov    %rax,%rcx
    180050b4a:	mov    $0xbe,%edx
    180050b4f:	call   *0xa177b(%rip)        # 0x1800f22d0
    180050b55:	nop
    180050b56:	lea    0x70(%rbp),%rcx
    180050b5a:	call   0x180008870
@@ -113108,15 +113108,15 @@
    180050c20:	mov    %rax,%rcx
    180050c23:	lea    0xa3e9a(%rip),%rdx        # 0x1800f4ac4
    180050c2a:	call   0x1800033f0
    180050c2f:	mov    %rax,%rcx
    180050c32:	lea    0xa8d47(%rip),%rdx        # 0x1800f9980
    180050c39:	call   0x1800033f0
    180050c3e:	mov    %rax,%rcx
-   180050c41:	lea    0xa3e30(%rip),%rdx        # 0x1800f4a78
+   180050c41:	lea    0xa3e28(%rip),%rdx        # 0x1800f4a70
    180050c48:	call   0x1800033f0
    180050c4d:	mov    %rax,%rcx
    180050c50:	mov    $0xcb,%edx
    180050c55:	call   *0xa1675(%rip)        # 0x1800f22d0
    180050c5b:	nop
    180050c5c:	lea    0x70(%rbp),%rcx
    180050c60:	call   0x180008870
@@ -113173,15 +113173,15 @@
    180050d3e:	mov    %rax,%rcx
    180050d41:	lea    0xa3d7c(%rip),%rdx        # 0x1800f4ac4
    180050d48:	call   0x1800033f0
    180050d4d:	mov    %rax,%rcx
    180050d50:	lea    0xa8c29(%rip),%rdx        # 0x1800f9980
    180050d57:	call   0x1800033f0
    180050d5c:	mov    %rax,%rcx
-   180050d5f:	lea    0xa3d12(%rip),%rdx        # 0x1800f4a78
+   180050d5f:	lea    0xa3d0a(%rip),%rdx        # 0x1800f4a70
    180050d66:	call   0x1800033f0
    180050d6b:	mov    %rax,%rcx
    180050d6e:	mov    $0xc4,%edx
    180050d73:	call   *0xa1557(%rip)        # 0x1800f22d0
    180050d79:	nop
    180050d7a:	lea    0x70(%rbp),%rcx
    180050d7e:	call   0x180008870
@@ -113243,15 +113243,15 @@
    180050e69:	mov    %rax,%rcx
    180050e6c:	lea    0xa3c51(%rip),%rdx        # 0x1800f4ac4
    180050e73:	call   0x1800033f0
    180050e78:	mov    %rax,%rcx
    180050e7b:	lea    0xa8afe(%rip),%rdx        # 0x1800f9980
    180050e82:	call   0x1800033f0
    180050e87:	mov    %rax,%rcx
-   180050e8a:	lea    0xa3be7(%rip),%rdx        # 0x1800f4a78
+   180050e8a:	lea    0xa3bdf(%rip),%rdx        # 0x1800f4a70
    180050e91:	call   0x1800033f0
    180050e96:	mov    %rax,%rcx
    180050e99:	mov    $0xc3,%edx
    180050e9e:	call   *0xa142c(%rip)        # 0x1800f22d0
    180050ea4:	nop
    180050ea5:	lea    0x70(%rbp),%rcx
    180050ea9:	call   0x180008870
@@ -115272,27 +115272,27 @@
    180052d7a:	mov    %rax,%rdx
    180052d7d:	lea    0x8(%rdi),%rcx
    180052d81:	call   0x1800123a0
    180052d86:	call   0x18000ac00
    180052d8b:	mov    %rax,%rdx
    180052d8e:	lea    0x8(%rdi),%rcx
    180052d92:	call   0x1800123a0
-   180052d97:	lea    0xa1c9a(%rip),%rdx        # 0x1800f4a38
+   180052d97:	lea    0xa1c96(%rip),%rdx        # 0x1800f4a34
    180052d9e:	lea    0x28(%rsp),%rcx
    180052da3:	call   0x180004f90
    180052da8:	nop
    180052da9:	call   0x18000acd0
    180052dae:	mov    %rax,%rdx
    180052db1:	lea    0x28(%rsp),%r8
    180052db6:	mov    %rdi,%rcx
    180052db9:	call   *0xa00a9(%rip)        # 0x1800f2e68
    180052dbf:	nop
    180052dc0:	lea    0x28(%rsp),%rcx
    180052dc5:	call   0x180008870
-   180052dca:	lea    0xa1c67(%rip),%rdx        # 0x1800f4a38
+   180052dca:	lea    0xa1c63(%rip),%rdx        # 0x1800f4a34
    180052dd1:	lea    0x68(%rsp),%rcx
    180052dd6:	call   0x180004f90
    180052ddb:	nop
    180052ddc:	call   0x18000ad90
    180052de1:	mov    %rax,%rdx
    180052de4:	lea    0x68(%rsp),%r8
    180052de9:	mov    %rdi,%rcx
@@ -115356,27 +115356,27 @@
    180052ed3:	mov    %rax,%rdx
    180052ed6:	lea    0x8(%rbp),%r8
    180052eda:	mov    %rdi,%rcx
    180052edd:	call   *0x9ff85(%rip)        # 0x1800f2e68
    180052ee3:	nop
    180052ee4:	lea    0x8(%rbp),%rcx
    180052ee8:	call   0x180008870
-   180052eed:	lea    0xa1b44(%rip),%rdx        # 0x1800f4a38
+   180052eed:	lea    0xa1b40(%rip),%rdx        # 0x1800f4a34
    180052ef4:	lea    0x28(%rbp),%rcx
    180052ef8:	call   0x180004f90
    180052efd:	nop
    180052efe:	call   0x18000ab50
    180052f03:	mov    %rax,%rdx
    180052f06:	lea    0x28(%rbp),%r8
    180052f0a:	mov    %rdi,%rcx
    180052f0d:	call   *0x9ff55(%rip)        # 0x1800f2e68
    180052f13:	nop
    180052f14:	lea    0x28(%rbp),%rcx
    180052f18:	call   0x180008870
-   180052f1d:	lea    0xa1b14(%rip),%rdx        # 0x1800f4a38
+   180052f1d:	lea    0xa1b10(%rip),%rdx        # 0x1800f4a34
    180052f24:	lea    0x48(%rsp),%rcx
    180052f29:	call   0x180004f90
    180052f2e:	nop
    180052f2f:	call   0x18000af00
    180052f34:	mov    %rax,%rdx
    180052f37:	lea    0x48(%rsp),%r8
    180052f3c:	mov    %rdi,%rcx
@@ -116196,15 +116196,15 @@
    180053d81:	mov    %rax,%rcx
    180053d84:	call   0x18000c600
    180053d89:	call   0x18000ab50
    180053d8e:	mov    %rax,%rdx
    180053d91:	lea    0x58(%r13),%rcx
    180053d95:	call   0x180054390
    180053d9a:	xor    %r8d,%r8d
-   180053d9d:	lea    0xa0c94(%rip),%rdx        # 0x1800f4a38
+   180053d9d:	lea    0xa0c90(%rip),%rdx        # 0x1800f4a34
    180053da4:	mov    %rax,%rcx
    180053da7:	call   0x18000c600
    180053dac:	call   0x18000b070
    180053db1:	mov    %rax,%rdx
    180053db4:	lea    0x58(%r13),%rcx
    180053db8:	call   0x180054390
    180053dbd:	mov    0x88(%rsp),%rcx
@@ -116218,15 +116218,15 @@
    180053ddb:	mov    %rax,%rcx
    180053dde:	call   0x18000c600
    180053de3:	call   0x18000af00
    180053de8:	mov    %rax,%rdx
    180053deb:	lea    0x58(%r13),%rcx
    180053def:	call   0x180054390
    180053df4:	xor    %r8d,%r8d
-   180053df7:	lea    0xa0c3a(%rip),%rdx        # 0x1800f4a38
+   180053df7:	lea    0xa0c36(%rip),%rdx        # 0x1800f4a34
    180053dfe:	mov    %rax,%rcx
    180053e01:	call   0x18000c600
    180053e06:	mov    %rbx,%r14
    180053e09:	cmpb   $0x0,0x3c(%r13)
    180053e0e:	lea    0xa5e5b(%rip),%rax        # 0x1800f9c70
    180053e15:	cmovne %rax,%r14
    180053e19:	call   0x18000ae40
@@ -116458,15 +116458,15 @@
    1800541c9:	mov    %rax,%rcx
    1800541cc:	lea    0xa08f1(%rip),%rdx        # 0x1800f4ac4
    1800541d3:	call   0x1800033f0
    1800541d8:	mov    %rax,%rcx
    1800541db:	lea    0xa5b6e(%rip),%rdx        # 0x1800f9d50
    1800541e2:	call   0x1800033f0
    1800541e7:	mov    %rax,%rcx
-   1800541ea:	lea    0xa0887(%rip),%rdx        # 0x1800f4a78
+   1800541ea:	lea    0xa087f(%rip),%rdx        # 0x1800f4a70
    1800541f1:	call   0x1800033f0
    1800541f6:	mov    %rax,%rcx
    1800541f9:	mov    $0xfe,%edx
    1800541fe:	call   *0x9e0cc(%rip)        # 0x1800f22d0
    180054204:	nop
    180054205:	lea    0x2d0(%rsp),%rcx
    18005420d:	call   0x180008870
@@ -119239,15 +119239,15 @@
    180056954:	sub    %edx,%eax
    180056956:	sar    $1,%eax
    180056958:	mov    %eax,%ebx
    18005695a:	mov    %eax,-0x61(%rbp)
    18005695d:	mov    (%r14),%rax
    180056960:	mov    %r14,%rcx
    180056963:	call   *0xa8(%rax)
-   180056969:	imul   0x9e04c(%rip),%eax        # 0x1800f49bc
+   180056969:	imul   0x9e05c(%rip),%eax        # 0x1800f49cc
    180056970:	mov    %eax,-0x69(%rbp)
    180056973:	movl   $0xbb8,0x50(%rsp)
    18005697b:	lea    -0x69(%rbp),%rcx
    18005697f:	lea    -0x61(%rbp),%rdx
    180056983:	cmp    %eax,%ebx
    180056985:	cmovge %rdx,%rcx
    180056989:	lea    0x50(%rsp),%rax
@@ -119584,15 +119584,15 @@
    180056e48:	je     0x180056f00
    180056e4e:	lea    0x10(%r12),%rdi
    180056e53:	cmpb   $0x0,0x1c0(%r15)
    180056e5b:	je     0x180056f27
    180056e61:	mov    (%r15),%rcx
    180056e64:	mov    (%rcx),%rax
    180056e67:	call   *0xa8(%rax)
-   180056e6d:	imul   0x9db48(%rip),%eax        # 0x1800f49bc
+   180056e6d:	imul   0x9db58(%rip),%eax        # 0x1800f49cc
    180056e74:	mov    0x0(%r13),%r9d
    180056e78:	mov    %rdi,-0x70(%rbp)
    180056e7c:	cmp    %eax,%r9d
    180056e7f:	ja     0x180056ec5
    180056e81:	lea    0x140(%r15),%rax
    180056e88:	mov    %rax,-0x68(%rbp)
    180056e8c:	mov    %r13,-0x60(%rbp)
@@ -129470,15 +129470,15 @@
    18005f37e:	xor    %rsp,%rax
    18005f381:	mov    %rax,0x70(%rbp)
    18005f385:	mov    %r9,%rdi
    18005f388:	mov    %rcx,%rsi
    18005f38b:	mov    %rcx,0x40(%rsp)
    18005f390:	xor    %r15d,%r15d
    18005f393:	mov    %r15d,0x20(%rsp)
-   18005f398:	lea    0x956d1(%rip),%rax        # 0x1800f4a70
+   18005f398:	lea    0x956c9(%rip),%rax        # 0x1800f4a68
    18005f39f:	mov    %rax,(%rcx)
    18005f3a2:	mov    %rdx,0x8(%rcx)
    18005f3a6:	add    $0x10,%rcx
    18005f3aa:	mov    %r8,%rdx
    18005f3ad:	call   0x180004eb0
    18005f3b2:	nop
    18005f3b3:	lea    0x30(%rsi),%rcx
@@ -150114,15 +150114,15 @@
    180071bae:	call   0x1800127d0
    180071bb3:	test   %al,%al
    180071bb5:	je     0x180071bcb
    180071bb7:	lea    0x8be52(%rip),%rdx        # 0x1800fda10
    180071bbe:	mov    %rbx,%rcx
    180071bc1:	call   0x180062510
    180071bc6:	jmp    0x180071d1d
-   180071bcb:	lea    0x82e66(%rip),%rdx        # 0x1800f4a38
+   180071bcb:	lea    0x82e62(%rip),%rdx        # 0x1800f4a34
    180071bd2:	mov    %rdi,%rcx
    180071bd5:	call   0x1800127d0
    180071bda:	test   %al,%al
    180071bdc:	je     0x180071bf2
    180071bde:	lea    0x8be83(%rip),%rdx        # 0x1800fda68
    180071be5:	mov    %rbx,%rcx
    180071be8:	call   0x180062510
@@ -152304,15 +152304,15 @@
    180073b77:	add    $0xfffffffffffffff8,%rax
    180073b7b:	cmp    $0x1f,%rax
    180073b7f:	jbe    0x180073b88
    180073b81:	call   *0x7f661(%rip)        # 0x1800f31e8
    180073b87:	int3
    180073b88:	call   0x1800e0a7c
    180073b8d:	xor    %r8d,%r8d
-   180073b90:	lea    0x80ea1(%rip),%rdx        # 0x1800f4a38
+   180073b90:	lea    0x80e9d(%rip),%rdx        # 0x1800f4a34
    180073b97:	lea    0x1f0(%r15),%rcx
    180073b9e:	call   0x18000c600
    180073ba3:	mov    (%r14),%rbx
    180073ba6:	mov    0x8(%rbx),%r8
    180073baa:	mov    %r14,%rdx
    180073bad:	mov    %r14,%rcx
    180073bb0:	call   0x180004500
@@ -152613,15 +152613,15 @@
    1800740e4:	add    $0xfffffffffffffff8,%rax
    1800740e8:	cmp    $0x1f,%rax
    1800740ec:	jbe    0x1800740f5
    1800740ee:	call   *0x7f0f4(%rip)        # 0x1800f31e8
    1800740f4:	int3
    1800740f5:	call   0x1800e0a7c
    1800740fa:	xor    %r8d,%r8d
-   1800740fd:	lea    0x80934(%rip),%rdx        # 0x1800f4a38
+   1800740fd:	lea    0x80930(%rip),%rdx        # 0x1800f4a34
    180074104:	lea    0x210(%r15),%rcx
    18007410b:	call   0x18000c600
    180074110:	mov    %r13,%rcx
    180074113:	call   0x18000c770
    180074118:	nop
    180074119:	mov    -0x58(%rbp),%rcx
    18007411d:	test   %rcx,%rcx
@@ -171403,15 +171403,15 @@
    180086569:	call   *0x6c829(%rip)        # 0x1800f2d98
    18008656f:	mov    %rax,%r14
    180086572:	mov    %rdi,0x180(%rbp)
    180086579:	mov    %rdi,0x190(%rbp)
    180086580:	movq   $0xf,0x198(%rbp)
    18008658b:	movb   $0x0,0x180(%rbp)
    180086592:	xor    %r8d,%r8d
-   180086595:	lea    0x6e49c(%rip),%rdx        # 0x1800f4a38
+   180086595:	lea    0x6e498(%rip),%rdx        # 0x1800f4a34
    18008659c:	lea    0x180(%rbp),%rcx
    1800865a3:	call   0x18000c600
    1800865a8:	nop
    1800865a9:	lea    0x180(%rbp),%r9
    1800865b0:	mov    %r15d,%r8d
    1800865b3:	lea    0x228(%rbp),%rdx
    1800865ba:	mov    0x58(%r12),%rcx
@@ -172917,15 +172917,15 @@
    180087f3f:	call   *0x6ae03(%rip)        # 0x1800f2d48
    180087f45:	mov    %rax,%r14
    180087f48:	mov    %rsi,0x180(%rbp)
    180087f4f:	mov    %rsi,0x190(%rbp)
    180087f56:	movq   $0xf,0x198(%rbp)
    180087f61:	movb   $0x0,0x180(%rbp)
    180087f68:	xor    %r8d,%r8d
-   180087f6b:	lea    0x6cac6(%rip),%rdx        # 0x1800f4a38
+   180087f6b:	lea    0x6cac2(%rip),%rdx        # 0x1800f4a34
    180087f72:	lea    0x180(%rbp),%rcx
    180087f79:	call   0x18000c600
    180087f7e:	nop
    180087f7f:	lea    0x180(%rbp),%r9
    180087f86:	mov    %r12d,%r8d
    180087f89:	lea    0x248(%rbp),%rdx
    180087f90:	mov    0x58(%r13),%rcx
@@ -177025,15 +177025,15 @@
    18008c46f:	test   %eax,%eax
    18008c471:	jle    0x18008c52a
    18008c477:	nopw   0x0(%rax,%rax,1)
    18008c480:	mov    %r13d,%edx
    18008c483:	mov    %r15,%rcx
    18008c486:	call   *0x65ee4(%rip)        # 0x1800f2370
    18008c48c:	mov    %rax,%rdi
-   18008c48f:	lea    0x685a2(%rip),%rdx        # 0x1800f4a38
+   18008c48f:	lea    0x6859e(%rip),%rdx        # 0x1800f4a34
    18008c496:	lea    0x548(%rbp),%rcx
    18008c49d:	call   0x180004f90
    18008c4a2:	nop
    18008c4a3:	lea    0x548(%rbp),%r9
    18008c4aa:	mov    %r13d,%r8d
    18008c4ad:	lea    0x618(%rbp),%rdx
    18008c4b4:	mov    0x58(%r14),%rcx
@@ -179450,15 +179450,15 @@
    18008ee71:	test   %eax,%eax
    18008ee73:	jle    0x18008ef28
    18008ee79:	nopl   0x0(%rax)
    18008ee80:	mov    %esi,%edx
    18008ee82:	mov    %r15,%rcx
    18008ee85:	call   *0x6359d(%rip)        # 0x1800f2428
    18008ee8b:	mov    %rax,%rdi
-   18008ee8e:	lea    0x65ba3(%rip),%rdx        # 0x1800f4a38
+   18008ee8e:	lea    0x65b9f(%rip),%rdx        # 0x1800f4a34
    18008ee95:	lea    0x1f0(%rbp),%rcx
    18008ee9c:	call   0x180004f90
    18008eea1:	nop
    18008eea2:	lea    0x1f0(%rbp),%r9
    18008eea9:	mov    %esi,%r8d
    18008eeac:	lea    0x280(%rbp),%rdx
    18008eeb3:	mov    0x50(%r13),%rcx
@@ -181017,15 +181017,15 @@
    18009091a:	call   *0x61b60(%rip)        # 0x1800f2480
    180090920:	mov    %rax,%r14
    180090923:	mov    %rsi,0x1f0(%rbp)
    18009092a:	mov    %rsi,0x200(%rbp)
    180090931:	movq   $0xf,0x208(%rbp)
    18009093c:	movb   $0x0,0x1f0(%rbp)
    180090943:	xor    %r8d,%r8d
-   180090946:	lea    0x640eb(%rip),%rdx        # 0x1800f4a38
+   180090946:	lea    0x640e7(%rip),%rdx        # 0x1800f4a34
    18009094d:	lea    0x1f0(%rbp),%rcx
    180090954:	call   0x18000c600
    180090959:	nop
    18009095a:	lea    0x1f0(%rbp),%r9
    180090961:	mov    %r12d,%r8d
    180090964:	lea    0x230(%rbp),%rdx
    18009096b:	mov    0x58(%r15),%rcx
@@ -185029,15 +185029,15 @@
    180095065:	call   0x180008870
    18009506a:	inc    %edi
    18009506c:	add    $0x8,%rsi
    180095070:	mov    %r12,%rcx
    180095073:	call   *0x5d447(%rip)        # 0x1800f24c0
    180095079:	cmp    %eax,%edi
    18009507b:	jl     0x180094f00
-   180095081:	lea    0x5f9b0(%rip),%rdx        # 0x1800f4a38
+   180095081:	lea    0x5f9ac(%rip),%rdx        # 0x1800f4a34
    180095088:	lea    0x4080(%rbp),%rcx
    18009508f:	call   0x180004f90
    180095094:	nop
    180095095:	lea    0x4080(%rbp),%r9
    18009509c:	xor    %r8d,%r8d
    18009509f:	lea    0x6200(%rbp),%rdx
    1800950a6:	mov    0x68(%r13),%rcx
@@ -185186,15 +185186,15 @@
    180095332:	mov    %r12,%rcx
    180095335:	call   *0x5d17d(%rip)        # 0x1800f24b8
    18009533b:	cmp    %eax,%edi
    18009533d:	jl     0x1800952a0
    180095343:	mov    $0x1,%esi
    180095348:	cmp    %esi,0x48(%r13)
    18009534c:	jle    0x180095602
-   180095352:	lea    0x5f6df(%rip),%rdx        # 0x1800f4a38
+   180095352:	lea    0x5f6db(%rip),%rdx        # 0x1800f4a34
    180095359:	lea    0x4120(%rbp),%rcx
    180095360:	call   0x180004f90
    180095365:	nop
    180095366:	lea    -0x1(%rsi),%edi
    180095369:	lea    0x4120(%rbp),%r9
    180095370:	mov    %edi,%r8d
    180095373:	lea    0x6120(%rbp),%rdx
@@ -185222,15 +185222,15 @@
    1800953d4:	call   0x180008870
    1800953d9:	nop
    1800953da:	lea    0x4120(%rbp),%rcx
    1800953e1:	call   0x180008870
    1800953e6:	lea    0x2a0(%rbp),%rcx
    1800953ed:	call   0x18005ebf0
    1800953f2:	nop
-   1800953f3:	lea    0x5f63e(%rip),%rdx        # 0x1800f4a38
+   1800953f3:	lea    0x5f63a(%rip),%rdx        # 0x1800f4a34
    1800953fa:	lea    0x4140(%rbp),%rcx
    180095401:	call   0x180004f90
    180095406:	nop
    180095407:	movslq %esi,%rdx
    18009540a:	shl    $0x5,%rdx
    18009540e:	add    0xd0(%rbp),%rdx
    180095415:	lea    -0x68(%rbp),%r8
@@ -188299,15 +188299,15 @@
    180098b0d:	lea    0x52c0(%rbp),%rcx
    180098b14:	call   0x180008870
    180098b19:	xor    %esi,%esi
    180098b1b:	cmp    %esi,0x48(%r13)
    180098b1f:	jle    0x180098c72
    180098b25:	movslq %ebx,%r14
    180098b28:	nopl   0x0(%rax,%rax,1)
-   180098b30:	lea    0x5bf01(%rip),%rdx        # 0x1800f4a38
+   180098b30:	lea    0x5befd(%rip),%rdx        # 0x1800f4a34
    180098b37:	lea    0x47a0(%rbp),%rcx
    180098b3e:	call   0x180004f90
    180098b43:	nop
    180098b44:	lea    0x47a0(%rbp),%r9
    180098b4b:	mov    %esi,%r8d
    180098b4e:	lea    0x5380(%rbp),%rdx
    180098b55:	mov    0x70(%r13),%rcx
@@ -189921,15 +189921,15 @@
    18009a7d6:	mov    -0x48(%rbp),%r12
    18009a7da:	mov    0x54(%rsp),%r14d
    18009a7df:	mov    $0x1,%edi
    18009a7e4:	mov    %ecx,%eax
    18009a7e6:	cmp    %edi,%ecx
    18009a7e8:	jle    0x18009a890
    18009a7ee:	xchg   %ax,%ax
-   18009a7f0:	lea    0x5a241(%rip),%rdx        # 0x1800f4a38
+   18009a7f0:	lea    0x5a23d(%rip),%rdx        # 0x1800f4a34
    18009a7f7:	lea    0x4d60(%rbp),%rcx
    18009a7fe:	call   0x180004f90
    18009a803:	nop
    18009a804:	lea    0x4d60(%rbp),%r9
    18009a80b:	mov    %edi,%r8d
    18009a80e:	lea    0x5ac0(%rbp),%rdx
    18009a815:	mov    0x70(%r13),%rcx
@@ -189969,15 +189969,15 @@
    18009a8b0:	xor    %edi,%edi
    18009a8b2:	mov    0x88(%r13),%rax
    18009a8b9:	sub    0x80(%r13),%rax
    18009a8c0:	sar    $0x3,%rax
    18009a8c4:	test   %rax,%rax
    18009a8c7:	je     0x18009a9b6
    18009a8cd:	nopl   (%rax)
-   18009a8d0:	lea    0x5a161(%rip),%rdx        # 0x1800f4a38
+   18009a8d0:	lea    0x5a15d(%rip),%rdx        # 0x1800f4a34
    18009a8d7:	lea    0x4d40(%rbp),%rcx
    18009a8de:	call   0x180004f90
    18009a8e3:	nop
    18009a8e4:	lea    0x4d40(%rbp),%r9
    18009a8eb:	mov    %esi,%r8d
    18009a8ee:	lea    0x5ae0(%rbp),%rdx
    18009a8f5:	mov    0x70(%r13),%rcx
@@ -192755,15 +192755,15 @@
    18009d961:	test   %eax,%eax
    18009d963:	jle    0x18009da17
    18009d969:	nopl   0x0(%rax)
    18009d970:	mov    %ebx,%edx
    18009d972:	mov    %r12,%rcx
    18009d975:	call   *0x54c0d(%rip)        # 0x1800f2588
    18009d97b:	mov    %rax,%rsi
-   18009d97e:	lea    0x570b3(%rip),%rdx        # 0x1800f4a38
+   18009d97e:	lea    0x570af(%rip),%rdx        # 0x1800f4a34
    18009d985:	lea    0x430(%rbp),%rcx
    18009d98c:	call   0x180004f90
    18009d991:	nop
    18009d992:	lea    0x430(%rbp),%r9
    18009d999:	mov    %ebx,%r8d
    18009d99c:	lea    0x410(%rbp),%rdx
    18009d9a3:	mov    0x58(%r15),%rcx
@@ -192800,15 +192800,15 @@
    18009da23:	test   %eax,%eax
    18009da25:	jle    0x18009dad7
    18009da2b:	nopl   0x0(%rax,%rax,1)
    18009da30:	mov    %ebx,%edx
    18009da32:	mov    %r12,%rcx
    18009da35:	call   *0x54b55(%rip)        # 0x1800f2590
    18009da3b:	mov    %rax,%rsi
-   18009da3e:	lea    0x56ff3(%rip),%rdx        # 0x1800f4a38
+   18009da3e:	lea    0x56fef(%rip),%rdx        # 0x1800f4a34
    18009da45:	lea    0x430(%rbp),%rcx
    18009da4c:	call   0x180004f90
    18009da51:	nop
    18009da52:	lea    0x430(%rbp),%r9
    18009da59:	mov    %ebx,%r8d
    18009da5c:	lea    0x410(%rbp),%rdx
    18009da63:	mov    0x60(%r15),%rcx
@@ -201712,15 +201712,15 @@
    1800a77de:	movq   $0xf,0x598(%rbp)
    1800a77e9:	movb   $0x0,0x580(%rbp)
    1800a77f0:	lea    0x580(%rbp),%r9
    1800a77f7:	lea    0x520(%rbp),%r8
    1800a77fe:	mov    %edi,%edx
    1800a7800:	mov    %r15,%rcx
    1800a7803:	call   *0x4aedf(%rip)        # 0x1800f26e8
-   1800a7809:	lea    0x4d228(%rip),%rdx        # 0x1800f4a38
+   1800a7809:	lea    0x4d224(%rip),%rdx        # 0x1800f4a34
    1800a7810:	lea    0x540(%rbp),%rcx
    1800a7817:	call   0x180004f90
    1800a781c:	nop
    1800a781d:	lea    0x540(%rbp),%r9
    1800a7824:	mov    %edi,%r8d
    1800a7827:	lea    0x5f0(%rbp),%rdx
    1800a782e:	mov    0x50(%r14),%rcx
@@ -201745,15 +201745,15 @@
    1800a7881:	call   0x180008870
    1800a7886:	nop
    1800a7887:	lea    0x540(%rbp),%rcx
    1800a788e:	call   0x180008870
    1800a7893:	lea    0x690(%rbp),%rcx
    1800a789a:	call   0x18005ebf0
    1800a789f:	nop
-   1800a78a0:	lea    0x4d191(%rip),%rdx        # 0x1800f4a38
+   1800a78a0:	lea    0x4d18d(%rip),%rdx        # 0x1800f4a34
    1800a78a7:	lea    0x540(%rbp),%rcx
    1800a78ae:	call   0x180004f90
    1800a78b3:	nop
    1800a78b4:	lea    -0x28(%rbp),%r8
    1800a78b8:	lea    0x580(%rbp),%rdx
    1800a78bf:	lea    0x640(%rbp),%rcx
    1800a78c6:	call   *0x4b1cc(%rip)        # 0x1800f2a98
@@ -202832,15 +202832,15 @@
    1800a8aa9:	call   *0x49cf1(%rip)        # 0x1800f27a0
    1800a8aaf:	mov    %rax,%r14
    1800a8ab2:	mov    %rdi,0x180(%rbp)
    1800a8ab9:	mov    %rdi,0x190(%rbp)
    1800a8ac0:	movq   $0xf,0x198(%rbp)
    1800a8acb:	movb   $0x0,0x180(%rbp)
    1800a8ad2:	xor    %r8d,%r8d
-   1800a8ad5:	lea    0x4bf5c(%rip),%rdx        # 0x1800f4a38
+   1800a8ad5:	lea    0x4bf58(%rip),%rdx        # 0x1800f4a34
    1800a8adc:	lea    0x180(%rbp),%rcx
    1800a8ae3:	call   0x18000c600
    1800a8ae8:	nop
    1800a8ae9:	lea    0x180(%rbp),%r9
    1800a8af0:	mov    %r15d,%r8d
    1800a8af3:	lea    0x228(%rbp),%rdx
    1800a8afa:	mov    0x58(%r12),%rcx
@@ -217978,15 +217978,15 @@
    1800b7fa2:	mov    -0x18(%rbp),%rdx
    1800b7fa6:	add    %rsi,%rdx
    1800b7fa9:	lea    0x610(%rbp),%rcx
    1800b7fb0:	call   0x180004eb0
    1800b7fb5:	mov    %rax,0x5d0(%rbp)
    1800b7fbc:	or     $0x1,%r13d
    1800b7fc0:	jmp    0x1800b7fe0
-   1800b7fc2:	lea    0x3ca6f(%rip),%rdx        # 0x1800f4a38
+   1800b7fc2:	lea    0x3ca6b(%rip),%rdx        # 0x1800f4a34
    1800b7fc9:	lea    0x6d8(%rbp),%rcx
    1800b7fd0:	call   0x180004f90
    1800b7fd5:	mov    %rax,0x5d0(%rbp)
    1800b7fdc:	or     $0x2,%r13d
    1800b7fe0:	mov    %r13d,-0x70(%rbp)
    1800b7fe4:	mov    0x118(%rbp),%rdi
    1800b7feb:	add    %rsi,%rdi
@@ -218795,23 +218795,23 @@
    1800b8de5:	nop
    1800b8de6:	lea    0x2a0(%rbp),%rdx
    1800b8ded:	mov    %rax,%rcx
    1800b8df0:	call   *0x39bc2(%rip)        # 0x1800f29b8
    1800b8df6:	nop
    1800b8df7:	lea    0x610(%rbp),%rcx
    1800b8dfe:	call   *0x39bd4(%rip)        # 0x1800f29d8
-   1800b8e04:	lea    0x3bc2d(%rip),%rdx        # 0x1800f4a38
+   1800b8e04:	lea    0x3bc29(%rip),%rdx        # 0x1800f4a34
    1800b8e0b:	lea    0x698(%rbp),%rcx
    1800b8e12:	call   0x180004f90
    1800b8e17:	nop
    1800b8e18:	lea    0x44cd9(%rip),%rdx        # 0x1800fdaf8
    1800b8e1f:	lea    0x638(%rbp),%rcx
    1800b8e26:	call   0x180004f90
    1800b8e2b:	nop
-   1800b8e2c:	lea    0x3bc05(%rip),%rdx        # 0x1800f4a38
+   1800b8e2c:	lea    0x3bc01(%rip),%rdx        # 0x1800f4a34
    1800b8e33:	lea    0x530(%rbp),%rcx
    1800b8e3a:	call   0x180004f90
    1800b8e3f:	nop
    1800b8e40:	lea    0x80(%rbp),%rax
    1800b8e47:	mov    %rax,0x40(%rsp)
    1800b8e4c:	lea    0xb0(%rbp),%rax
    1800b8e53:	mov    %rax,0x38(%rsp)
@@ -239239,15 +239239,15 @@
    1800cc2ff:	test   %r14d,%r14d
    1800cc302:	jg     0x1800cc0e0
    1800cc308:	mov    0x38(%r15),%r14
    1800cc30c:	mov    0x40(%r15),%rsi
    1800cc310:	mov    0x40(%rsp),%r12
    1800cc315:	cmp    %rsi,%r14
    1800cc318:	je     0x1800cc4a7
-   1800cc31e:	lea    0x2874b(%rip),%r13        # 0x1800f4a70
+   1800cc31e:	lea    0x28743(%rip),%r13        # 0x1800f4a68
    1800cc325:	data16 data16 nopw 0x0(%rax,%rax,1)
    1800cc330:	mov    (%r14),%rdi
    1800cc333:	mov    (%rdi),%rax
    1800cc336:	mov    %rdi,%rcx
    1800cc339:	call   *0x28(%rax)
    1800cc33c:	cltd
    1800cc33d:	idivl  0x10(%r12)
@@ -247263,15 +247263,15 @@
    1800d4041:	call   0x180004f90
    1800d4046:	nop
    1800d4047:	lea    0x6d8(%rbp),%rdx
    1800d404e:	lea    0x88(%rbp),%rcx
    1800d4055:	call   0x180055a90
    1800d405a:	nop
    1800d405b:	jmp    0x1800d4085
-   1800d405d:	lea    0x209d4(%rip),%rdx        # 0x1800f4a38
+   1800d405d:	lea    0x209d0(%rip),%rdx        # 0x1800f4a34
    1800d4064:	lea    0x6d8(%rbp),%rcx
    1800d406b:	call   0x180004f90
    1800d4070:	nop
    1800d4071:	lea    0x6d8(%rbp),%rdx
    1800d4078:	lea    0x88(%rbp),%rcx
    1800d407f:	call   0x180055a90
    1800d4084:	nop
@@ -289114,95 +289114,90 @@
    1800f49ac:	outsb  %ds:(%rsi),(%dx)
    1800f49ad:	and    %dh,0x6f(%eax)
    1800f49b1:	jae    0x1800f4a1c
    1800f49b3:	je     0x1800f4a1e
    1800f49b5:	outsl  %ds:(%rsi),(%dx)
    1800f49b6:	outsb  %ds:(%rsi),(%dx)
    1800f49b7:	add    %al,(%rax)
-   1800f49b9:	add    %al,(%rax)
-   1800f49bb:	add    %al,0x0(%rax)
-   1800f49be:	add    %al,(%rax)
-   1800f49c0:	ds add %edi,(%rdx)
-   1800f49c3:	add    %esp,(%rsi)
-   1800f49c5:	add    %esp,0x35012901(%rip)        # 0x1b51072cc
-   1800f49cb:	add    %esp,(%rdi)
-   1800f49cd:	add    %esp,(%rcx,%rax,1)
-   1800f49d0:	add    %edi,(%rcx,%r8,1)
-   1800f49d4:	rex add %eax,0x1(%rcx)
-   1800f49d8:	sub    $0x2e012c01,%eax
-   1800f49dd:	add    %ebp,(%rbx)
-   1800f49df:	add    %ecx,%ebx
-   1800f49e1:	add    %bh,%al
-   1800f49e3:	add    -0x47fd4bfe(%rbp),%dh
-   1800f49e9:	add    %dl,%al
-   1800f49eb:	add    -0x30fd4cfe(%rsi),%dh
-   1800f49f1:	add    %cl,%cl
-   1800f49f3:	add    %ch,%cl
-   1800f49f5:	add    %dh,%cl
-   1800f49f7:	add    -0x43fd45fe(%rbx),%bh
-   1800f49fd:	add    0x61006502(%rcx),%bh
-   1800f4a03:	add    %cl,0x0(%rdi)
-   1800f4a06:	rex.WRX add %r10b,0x0(%rdx)
-   1800f4a0a:	pop    %rsp
-   1800f4a0b:	add    %dl,0x0(%rax)
-   1800f4a0e:	rex.WRB add %r13b,0x0(%r9)
-   1800f4a12:	movsxd (%rax),%eax
-   1800f4a14:	add    %ch,0x0(%eax)
-   1800f4a18:	push   %rbp
-   1800f4a19:	add    %dl,0x56(%rax,%rax,1)
-   1800f4a1d:	add    %dl,0x0(%rbx)
-   1800f4a20:	and    %al,(%rax)
-   1800f4a22:	add    %al,(%rax)
-   1800f4a24:	add    %al,(%rax)
-   1800f4a26:	add    %al,(%rax)
-   1800f4a28:	add    %al,(%rcx)
-   1800f4a2a:	(bad)
-   1800f4a2b:	(bad)
-   1800f4a2c:	add    $0x5,%al
-   1800f4a2e:	add    (%rdx),%eax
-   1800f4a30:	or     %cl,(%rcx)
-   1800f4a32:	or     (%rbx),%cl
-   1800f4a34:	femms
-   1800f4a36:	or     $0xc,%eax
-   1800f4a3b:	add    %al,(%rax)
-   1800f4a3d:	add    %al,(%rax)
-   1800f4a3f:	add    %al,-0x4d(%rax)
-   1800f4a42:	(bad)
-   1800f4a43:	addb   $0x0,(%rcx)
+   1800f49b9:	add    %eax,(%rdi)
+   1800f49bb:	(bad)
+   1800f49bc:	add    $0x5,%al
+   1800f49be:	add    (%rdx),%eax
+   1800f49c0:	or     %cl,(%rcx)
+   1800f49c2:	or     (%rbx),%cl
+   1800f49c4:	femms
+   1800f49c6:	or     $0xc,%eax
+   1800f49cb:	add    %al,0x0(%rax)
+   1800f49ce:	add    %al,(%rax)
+   1800f49d0:	ds add %edi,(%rdx)
+   1800f49d3:	add    %esp,(%rsi)
+   1800f49d5:	add    %esp,0x35012901(%rip)        # 0x1b51072dc
+   1800f49db:	add    %esp,(%rdi)
+   1800f49dd:	add    %esp,(%rcx,%rax,1)
+   1800f49e0:	add    %edi,(%rcx,%r8,1)
+   1800f49e4:	rex add %eax,0x1(%rcx)
+   1800f49e8:	sub    $0x2e012c01,%eax
+   1800f49ed:	add    %ebp,(%rbx)
+   1800f49ef:	add    %ecx,%ebx
+   1800f49f1:	add    %bh,%al
+   1800f49f3:	add    -0x47fd4bfe(%rbp),%dh
+   1800f49f9:	add    %dl,%al
+   1800f49fb:	add    -0x30fd4cfe(%rsi),%dh
+   1800f4a01:	add    %cl,%cl
+   1800f4a03:	add    %ch,%cl
+   1800f4a05:	add    %dh,%cl
+   1800f4a07:	add    -0x43fd45fe(%rbx),%bh
+   1800f4a0d:	add    0x61006502(%rcx),%bh
+   1800f4a13:	add    %cl,0x0(%rdi)
+   1800f4a16:	rex.WRX add %r10b,0x0(%rdx)
+   1800f4a1a:	pop    %rsp
+   1800f4a1b:	add    %dl,0x0(%rax)
+   1800f4a1e:	rex.WRB add %r13b,0x0(%r9)
+   1800f4a22:	movsxd (%rax),%eax
+   1800f4a24:	add    %ch,0x0(%eax)
+   1800f4a28:	push   %rbp
+   1800f4a29:	add    %dl,0x56(%rax,%rax,1)
+   1800f4a2d:	add    %dl,0x0(%rbx)
+   1800f4a30:	and    %al,(%rax)
+   1800f4a32:	add    %al,(%rax)
+   1800f4a34:	add    %al,(%rax)
+   1800f4a36:	add    %al,(%rax)
+   1800f4a38:	rex mov $0x16,%bl
+   1800f4a3b:	addb   $0x0,(%rcx)
+   1800f4a3e:	add    %al,(%rax)
+   1800f4a40:	add    %ch,0x18000(%rbx)
    1800f4a46:	add    %al,(%rax)
-   1800f4a48:	add    %ch,0x18000(%rbx)
-   1800f4a4e:	add    %al,(%rax)
-   1800f4a50:	shl    $1,%ah
-   1800f4a52:	add    %al,0x1(%rax)
-   1800f4a58:	(bad)
-   1800f4a5d:	(bad)
-   1800f4a5e:	jae    0x1800f4ad4
-	...
-   1800f4a68:	adc    %dh,0x180(%rsi,%rdx,1)
-   1800f4a6f:	add    %dl,%al
-   1800f4a71:	mov    (%rcx),%es
-   1800f4a73:	addb   $0x0,(%rcx)
-   1800f4a76:	add    %al,(%rax)
-   1800f4a78:	cmp    (%rax),%al
-   1800f4a7a:	add    %al,(%rax)
-   1800f4a7c:	add    %al,(%rax)
+   1800f4a48:	shl    $1,%ah
+   1800f4a4a:	add    %al,0x1(%rax)
+   1800f4a50:	(bad)
+   1800f4a55:	(bad)
+   1800f4a56:	jae    0x1800f4acc
+	...
+   1800f4a60:	adc    %dh,0x180(%rsi,%rdx,1)
+   1800f4a67:	add    %dl,%al
+   1800f4a69:	mov    (%rcx),%es
+   1800f4a6b:	addb   $0x0,(%rcx)
+   1800f4a6e:	add    %al,(%rax)
+   1800f4a70:	cmp    (%rax),%al
+	...
    1800f4a7e:	add    %al,(%rax)
    1800f4a80:	cmp    0x6c(%r10,%r12,2),%bl
    1800f4a85:	fs pop %rsp
    1800f4a87:	outsl  %ds:(%rsi),(%dx)
    1800f4a88:	jo     0x1800f4aef
    1800f4a8a:	outsb  %ds:(%rsi),(%dx)
    1800f4a8b:	insl   (%dx),%es:(%rdi)
    1800f4a8c:	insl   (%dx),%es:(%rdi)
    1800f4a8d:	pop    %rdi
    1800f4a8e:	xor    %esi,(%rdi)
    1800f4a90:	xor    %esi,(%rsp,%rsi,1)
-   1800f4a93:	xor    0x36323239(%rip),%esi        # 0x1b6417cd2
-   1800f4a99:	(bad)
-   1800f4a9a:	xor    %ebx,0x6f(%rdi,%rsi,2)
+   1800f4a93:	xor    0x30393932(%rip),%esi        # 0x1b04883cb
+   1800f4a99:	xor    (%rcx),%bh
+   1800f4a9b:	pop    %rsp
+   1800f4a9c:	ja     0x1800f4b0d
    1800f4a9e:	jb     0x1800f4b0b
    1800f4aa0:	pop    %rsp
    1800f4aa1:	jo     0x1800f4b0f
    1800f4aa3:	(bad)
    1800f4aa4:	je     0x1800f4b0c
    1800f4aa6:	outsl  %ds:(%rsi),(%dx)
    1800f4aa7:	jb     0x1800f4b16
@@ -292454,17 +292449,18 @@
    1800f69d8:	jo     0x1800f6a3f
    1800f69da:	outsb  %ds:(%rsi),(%dx)
    1800f69db:	insl   (%dx),%es:(%rdi)
    1800f69dc:	insl   (%dx),%es:(%rdi)
    1800f69dd:	pop    %rdi
    1800f69de:	xor    %esi,(%rdi)
    1800f69e0:	xor    %esi,(%rsp,%rsi,1)
-   1800f69e3:	xor    0x36323239(%rip),%esi        # 0x1b6419c22
-   1800f69e9:	(bad)
-   1800f69ea:	xor    %ebx,0x6f(%rdi,%rsi,2)
+   1800f69e3:	xor    0x30393932(%rip),%esi        # 0x1b048a31b
+   1800f69e9:	xor    (%rcx),%bh
+   1800f69eb:	pop    %rsp
+   1800f69ec:	ja     0x1800f6a5d
    1800f69ee:	jb     0x1800f6a5b
    1800f69f0:	pop    %rsp
    1800f69f1:	jo     0x1800f6a5f
    1800f69f3:	(bad)
    1800f69f4:	je     0x1800f6a5c
    1800f69f6:	outsl  %ds:(%rsi),(%dx)
    1800f69f7:	jb     0x1800f6a66
@@ -292624,17 +292620,18 @@
    1800f6b78:	jo     0x1800f6bdf
    1800f6b7a:	outsb  %ds:(%rsi),(%dx)
    1800f6b7b:	insl   (%dx),%es:(%rdi)
    1800f6b7c:	insl   (%dx),%es:(%rdi)
    1800f6b7d:	pop    %rdi
    1800f6b7e:	xor    %esi,(%rdi)
    1800f6b80:	xor    %esi,(%rsp,%rsi,1)
-   1800f6b83:	xor    0x36323239(%rip),%esi        # 0x1b6419dc2
-   1800f6b89:	(bad)
-   1800f6b8a:	xor    %ebx,0x6f(%rdi,%rsi,2)
+   1800f6b83:	xor    0x30393932(%rip),%esi        # 0x1b048a4bb
+   1800f6b89:	xor    (%rcx),%bh
+   1800f6b8b:	pop    %rsp
+   1800f6b8c:	ja     0x1800f6bfd
    1800f6b8e:	jb     0x1800f6bfb
    1800f6b90:	pop    %rsp
    1800f6b91:	jo     0x1800f6bff
    1800f6b93:	(bad)
    1800f6b94:	je     0x1800f6bfc
    1800f6b96:	outsl  %ds:(%rsi),(%dx)
    1800f6b97:	jb     0x1800f6c06
@@ -292666,55 +292663,58 @@
    1800f6bd1:	jb     0x1800f6bf3
    1800f6bd3:	imul   $0x6e,0x72(%rbp),%esp
    1800f6bd7:	gs insb (%dx),%es:(%rdi)
    1800f6bd9:	and    %ah,0x72(%rcx)
    1800f6bdc:	addr32 jne 0x1800f6c4c
    1800f6bdf:	outsb  %gs:(%rsi),(%dx)
    1800f6be1:	je     0x1800f6be3
-	...
-   1800f6bef:	add    %bh,(%rsi)
-   1800f6bf1:	add    %edi,(%rdx)
-   1800f6bf3:	add    %esp,(%rsi)
-   1800f6bf5:	add    %esp,0x35012901(%rip)        # 0x1b51094fc
-   1800f6bfb:	add    %esp,(%rdi)
-   1800f6bfd:	add    %esp,(%rcx,%rax,1)
-   1800f6c00:	add    %edi,(%rcx,%r8,1)
-   1800f6c04:	rex add %eax,0x1(%rcx)
-   1800f6c08:	sub    $0x2e012c01,%eax
-   1800f6c0d:	add    %ebp,(%rbx)
-   1800f6c0f:	add    %ecx,%ebx
-   1800f6c11:	add    %bh,%al
-   1800f6c13:	add    -0x47fd4bfe(%rbp),%dh
-   1800f6c19:	add    %dl,%al
-   1800f6c1b:	add    -0x30fd4cfe(%rsi),%dh
-   1800f6c21:	add    %cl,%cl
-   1800f6c23:	add    %ch,%cl
-   1800f6c25:	add    %dh,%cl
-   1800f6c27:	add    -0x43fd45fe(%rbx),%bh
-   1800f6c2d:	add    0x61006502(%rcx),%bh
-   1800f6c33:	add    %cl,0x0(%rdi)
-   1800f6c36:	rex.WRX add %r10b,0x0(%rdx)
-   1800f6c3a:	pop    %rsp
-   1800f6c3b:	add    %dl,0x0(%rax)
-   1800f6c3e:	rex.WRB add %r13b,0x0(%r9)
-   1800f6c42:	movsxd (%rax),%eax
-   1800f6c44:	add    %ch,0x0(%eax)
-   1800f6c48:	push   %rbp
-   1800f6c49:	add    %dl,0x56(%rax,%rax,1)
-   1800f6c4d:	add    %dl,0x0(%rbx)
-   1800f6c50:	add    %al,(%rcx)
-   1800f6c52:	(bad)
-   1800f6c53:	(bad)
-   1800f6c54:	add    $0x5,%al
-   1800f6c56:	add    (%rdx),%eax
-   1800f6c58:	or     %cl,(%rcx)
-   1800f6c5a:	or     (%rbx),%cl
-   1800f6c5c:	femms
-   1800f6c5e:	or     $0x16b6880c,%eax
-   1800f6c63:	addb   $0x0,(%rcx)
+   1800f6be3:	add    %al,(%rax)
+   1800f6be5:	add    %al,(%rax)
+   1800f6be7:	add    %al,(%rax)
+   1800f6be9:	add    %eax,(%rdi)
+   1800f6beb:	(bad)
+   1800f6bec:	add    $0x5,%al
+   1800f6bee:	add    (%rdx),%eax
+   1800f6bf0:	or     %cl,(%rcx)
+   1800f6bf2:	or     (%rbx),%cl
+   1800f6bf4:	femms
+   1800f6bf6:	or     $0xc,%eax
+   1800f6bfb:	add    %al,(%rax)
+   1800f6bfd:	add    %al,(%rax)
+   1800f6bff:	add    %bh,(%rsi)
+   1800f6c01:	add    %edi,(%rdx)
+   1800f6c03:	add    %esp,(%rsi)
+   1800f6c05:	add    %esp,0x35012901(%rip)        # 0x1b510950c
+   1800f6c0b:	add    %esp,(%rdi)
+   1800f6c0d:	add    %esp,(%rcx,%rax,1)
+   1800f6c10:	add    %edi,(%rcx,%r8,1)
+   1800f6c14:	rex add %eax,0x1(%rcx)
+   1800f6c18:	sub    $0x2e012c01,%eax
+   1800f6c1d:	add    %ebp,(%rbx)
+   1800f6c1f:	add    %ecx,%ebx
+   1800f6c21:	add    %bh,%al
+   1800f6c23:	add    -0x47fd4bfe(%rbp),%dh
+   1800f6c29:	add    %dl,%al
+   1800f6c2b:	add    -0x30fd4cfe(%rsi),%dh
+   1800f6c31:	add    %cl,%cl
+   1800f6c33:	add    %ch,%cl
+   1800f6c35:	add    %dh,%cl
+   1800f6c37:	add    -0x43fd45fe(%rbx),%bh
+   1800f6c3d:	add    0x61006502(%rcx),%bh
+   1800f6c43:	add    %cl,0x0(%rdi)
+   1800f6c46:	rex.WRX add %r10b,0x0(%rdx)
+   1800f6c4a:	pop    %rsp
+   1800f6c4b:	add    %dl,0x0(%rax)
+   1800f6c4e:	rex.WRB add %r13b,0x0(%r9)
+   1800f6c52:	movsxd (%rax),%eax
+   1800f6c54:	add    %ch,0x0(%eax)
+   1800f6c58:	push   %rbp
+   1800f6c59:	add    %dl,0x56(%rax,%rax,1)
+   1800f6c5d:	add    %dl,0x0(%rbx)
+   1800f6c60:	mov    %dh,0x18016(%rsi)
    1800f6c66:	add    %al,(%rax)
    1800f6c68:	shlb   $1,0x180(%rdx,%rax,1)
    1800f6c6f:	add    %ah,%al
    1800f6c71:	sbb    $0x1800e,%eax
    1800f6c76:	add    %al,(%rax)
    1800f6c78:	loopne 0x1800f6c97
    1800f6c7a:	(bad)
@@ -294472,54 +294472,56 @@
    1800f7dd3:	and    %ch,0x65(%rbx)
    1800f7dd6:	jb     0x1800f7e46
    1800f7dd8:	gs insb (%dx),%es:(%rdi)
    1800f7dda:	and    %ch,0x61(%rsi)
    1800f7ddd:	insl   (%dx),%es:(%rdi)
    1800f7dde:	and    %ah,%gs:(%rdi)
 	...
-   1800f7ded:	add    %al,(%rax)
-   1800f7def:	add    %bh,(%rsi)
-   1800f7df1:	add    %edi,(%rdx)
-   1800f7df3:	add    %esp,(%rsi)
-   1800f7df5:	add    %esp,0x35012901(%rip)        # 0x1b510a6fc
-   1800f7dfb:	add    %esp,(%rdi)
-   1800f7dfd:	add    %esp,(%rcx,%rax,1)
-   1800f7e00:	add    %edi,(%rcx,%r8,1)
-   1800f7e04:	rex add %eax,0x1(%rcx)
-   1800f7e08:	sub    $0x2e012c01,%eax
-   1800f7e0d:	add    %ebp,(%rbx)
-   1800f7e0f:	add    %ecx,%ebx
-   1800f7e11:	add    %bh,%al
-   1800f7e13:	add    -0x47fd4bfe(%rbp),%dh
-   1800f7e19:	add    %dl,%al
-   1800f7e1b:	add    -0x30fd4cfe(%rsi),%dh
-   1800f7e21:	add    %cl,%cl
-   1800f7e23:	add    %ch,%cl
-   1800f7e25:	add    %dh,%cl
-   1800f7e27:	add    -0x43fd45fe(%rbx),%bh
-   1800f7e2d:	add    0x61006502(%rcx),%bh
-   1800f7e33:	add    %cl,0x0(%rdi)
-   1800f7e36:	rex.WRX add %r10b,0x0(%rdx)
-   1800f7e3a:	pop    %rsp
-   1800f7e3b:	add    %dl,0x0(%rax)
-   1800f7e3e:	rex.WRB add %r13b,0x0(%r9)
-   1800f7e42:	movsxd (%rax),%eax
-   1800f7e44:	add    %ch,0x0(%eax)
-   1800f7e48:	push   %rbp
-   1800f7e49:	add    %dl,0x56(%rax,%rax,1)
-   1800f7e4d:	add    %dl,0x0(%rbx)
-   1800f7e50:	add    %al,(%rcx)
-   1800f7e52:	(bad)
-   1800f7e53:	(bad)
-   1800f7e54:	add    $0x5,%al
-   1800f7e56:	add    (%rdx),%eax
-   1800f7e58:	or     %cl,(%rcx)
-   1800f7e5a:	or     (%rbx),%cl
-   1800f7e5c:	femms
-   1800f7e5e:	or     $0x16de700c,%eax
+   1800f7de9:	add    %eax,(%rdi)
+   1800f7deb:	(bad)
+   1800f7dec:	add    $0x5,%al
+   1800f7dee:	add    (%rdx),%eax
+   1800f7df0:	or     %cl,(%rcx)
+   1800f7df2:	or     (%rbx),%cl
+   1800f7df4:	femms
+   1800f7df6:	or     $0xc,%eax
+   1800f7dfb:	add    %al,(%rax)
+   1800f7dfd:	add    %al,(%rax)
+   1800f7dff:	add    %bh,(%rsi)
+   1800f7e01:	add    %edi,(%rdx)
+   1800f7e03:	add    %esp,(%rsi)
+   1800f7e05:	add    %esp,0x35012901(%rip)        # 0x1b510a70c
+   1800f7e0b:	add    %esp,(%rdi)
+   1800f7e0d:	add    %esp,(%rcx,%rax,1)
+   1800f7e10:	add    %edi,(%rcx,%r8,1)
+   1800f7e14:	rex add %eax,0x1(%rcx)
+   1800f7e18:	sub    $0x2e012c01,%eax
+   1800f7e1d:	add    %ebp,(%rbx)
+   1800f7e1f:	add    %ecx,%ebx
+   1800f7e21:	add    %bh,%al
+   1800f7e23:	add    -0x47fd4bfe(%rbp),%dh
+   1800f7e29:	add    %dl,%al
+   1800f7e2b:	add    -0x30fd4cfe(%rsi),%dh
+   1800f7e31:	add    %cl,%cl
+   1800f7e33:	add    %ch,%cl
+   1800f7e35:	add    %dh,%cl
+   1800f7e37:	add    -0x43fd45fe(%rbx),%bh
+   1800f7e3d:	add    0x61006502(%rcx),%bh
+   1800f7e43:	add    %cl,0x0(%rdi)
+   1800f7e46:	rex.WRX add %r10b,0x0(%rdx)
+   1800f7e4a:	pop    %rsp
+   1800f7e4b:	add    %dl,0x0(%rax)
+   1800f7e4e:	rex.WRB add %r13b,0x0(%r9)
+   1800f7e52:	movsxd (%rax),%eax
+   1800f7e54:	add    %ch,0x0(%eax)
+   1800f7e58:	push   %rbp
+   1800f7e59:	add    %dl,0x56(%rax,%rax,1)
+   1800f7e5d:	add    %dl,0x0(%rbx)
+   1800f7e60:	jo     0x1800f7e40
+   1800f7e62:	(bad)
    1800f7e63:	addb   $0x0,(%rcx)
    1800f7e66:	add    %al,(%rax)
    1800f7e68:	rex xor (%rbx),%eax
    1800f7e6b:	addb   $0x0,(%rcx)
    1800f7e6e:	add    %al,(%rax)
    1800f7e70:	loopne 0x1800f7e8f
    1800f7e72:	(bad)
@@ -295438,17 +295440,18 @@
    1800f8628:	jo     0x1800f868f
    1800f862a:	outsb  %ds:(%rsi),(%dx)
    1800f862b:	insl   (%dx),%es:(%rdi)
    1800f862c:	insl   (%dx),%es:(%rdi)
    1800f862d:	pop    %rdi
    1800f862e:	xor    %esi,(%rdi)
    1800f8630:	xor    %esi,(%rsp,%rsi,1)
-   1800f8633:	xor    0x36323239(%rip),%esi        # 0x1b641b872
-   1800f8639:	(bad)
-   1800f863a:	xor    %ebx,0x6f(%rdi,%rsi,2)
+   1800f8633:	xor    0x30393932(%rip),%esi        # 0x1b048bf6b
+   1800f8639:	xor    (%rcx),%bh
+   1800f863b:	pop    %rsp
+   1800f863c:	ja     0x1800f86ad
    1800f863e:	jb     0x1800f86ab
    1800f8640:	pop    %rsp
    1800f8641:	jo     0x1800f86af
    1800f8643:	(bad)
    1800f8644:	je     0x1800f86ac
    1800f8646:	outsl  %ds:(%rsi),(%dx)
    1800f8647:	jb     0x1800f86b6
@@ -296145,17 +296148,18 @@
    1800f8cb8:	jo     0x1800f8d1f
    1800f8cba:	outsb  %ds:(%rsi),(%dx)
    1800f8cbb:	insl   (%dx),%es:(%rdi)
    1800f8cbc:	insl   (%dx),%es:(%rdi)
    1800f8cbd:	pop    %rdi
    1800f8cbe:	xor    %esi,(%rdi)
    1800f8cc0:	xor    %esi,(%rsp,%rsi,1)
-   1800f8cc3:	xor    0x36323239(%rip),%esi        # 0x1b641bf02
-   1800f8cc9:	(bad)
-   1800f8cca:	xor    %ebx,0x6f(%rdi,%rsi,2)
+   1800f8cc3:	xor    0x30393932(%rip),%esi        # 0x1b048c5fb
+   1800f8cc9:	xor    (%rcx),%bh
+   1800f8ccb:	pop    %rsp
+   1800f8ccc:	ja     0x1800f8d3d
    1800f8cce:	jb     0x1800f8d3b
    1800f8cd0:	pop    %rsp
    1800f8cd1:	jo     0x1800f8d3f
    1800f8cd3:	(bad)
    1800f8cd4:	je     0x1800f8d3c
    1800f8cd6:	outsl  %ds:(%rsi),(%dx)
    1800f8cd7:	jb     0x1800f8d46
@@ -297360,56 +297364,56 @@
    1800f9688:	cmc
    1800f9689:	test   %edx,-0x10d(%rax)
    1800f968f:	(bad)
    1800f9690:	add    %al,(%rax)
    1800f9692:	add    %al,(%rax)
    1800f9694:	add    %al,(%rax)
    1800f9696:	and    %al,0x0(%rax)
-   1800f9699:	add    %al,(%rax)
-   1800f969b:	add    %al,(%rax)
-   1800f969d:	add    %al,(%rax)
-   1800f969f:	add    %bh,(%rsi)
-   1800f96a1:	add    %edi,(%rdx)
-   1800f96a3:	add    %esp,(%rsi)
-   1800f96a5:	add    %esp,0x35012901(%rip)        # 0x1b510bfac
-   1800f96ab:	add    %esp,(%rdi)
-   1800f96ad:	add    %esp,(%rcx,%rax,1)
-   1800f96b0:	add    %edi,(%rcx,%r8,1)
-   1800f96b4:	rex add %eax,0x1(%rcx)
-   1800f96b8:	sub    $0x2e012c01,%eax
-   1800f96bd:	add    %ebp,(%rbx)
-   1800f96bf:	add    %ecx,%ebx
-   1800f96c1:	add    %bh,%al
-   1800f96c3:	add    -0x47fd4bfe(%rbp),%dh
-   1800f96c9:	add    %dl,%al
-   1800f96cb:	add    -0x30fd4cfe(%rsi),%dh
-   1800f96d1:	add    %cl,%cl
-   1800f96d3:	add    %ch,%cl
-   1800f96d5:	add    %dh,%cl
-   1800f96d7:	add    -0x43fd45fe(%rbx),%bh
-   1800f96dd:	add    0x61006502(%rcx),%bh
-   1800f96e3:	add    %cl,0x0(%rdi)
-   1800f96e6:	rex.WRX add %r10b,0x0(%rdx)
-   1800f96ea:	pop    %rsp
-   1800f96eb:	add    %dl,0x0(%rax)
-   1800f96ee:	rex.WRB add %r13b,0x0(%r9)
-   1800f96f2:	movsxd (%rax),%eax
-   1800f96f4:	add    %ch,0x0(%eax)
-   1800f96f8:	push   %rbp
-   1800f96f9:	add    %dl,0x56(%rax,%rax,1)
-   1800f96fd:	add    %dl,0x0(%rbx)
-   1800f9700:	add    %al,(%rcx)
-   1800f9702:	(bad)
-   1800f9703:	(bad)
-   1800f9704:	add    $0x5,%al
-   1800f9706:	add    (%rdx),%eax
-   1800f9708:	or     %cl,(%rcx)
-   1800f970a:	or     (%rbx),%cl
-   1800f970c:	femms
-   1800f970e:	or     $0x16e4600c,%eax
+   1800f9699:	add    %eax,(%rdi)
+   1800f969b:	(bad)
+   1800f969c:	add    $0x5,%al
+   1800f969e:	add    (%rdx),%eax
+   1800f96a0:	or     %cl,(%rcx)
+   1800f96a2:	or     (%rbx),%cl
+   1800f96a4:	femms
+   1800f96a6:	or     $0xc,%eax
+   1800f96ab:	add    %al,(%rax)
+   1800f96ad:	add    %al,(%rax)
+   1800f96af:	add    %bh,(%rsi)
+   1800f96b1:	add    %edi,(%rdx)
+   1800f96b3:	add    %esp,(%rsi)
+   1800f96b5:	add    %esp,0x35012901(%rip)        # 0x1b510bfbc
+   1800f96bb:	add    %esp,(%rdi)
+   1800f96bd:	add    %esp,(%rcx,%rax,1)
+   1800f96c0:	add    %edi,(%rcx,%r8,1)
+   1800f96c4:	rex add %eax,0x1(%rcx)
+   1800f96c8:	sub    $0x2e012c01,%eax
+   1800f96cd:	add    %ebp,(%rbx)
+   1800f96cf:	add    %ecx,%ebx
+   1800f96d1:	add    %bh,%al
+   1800f96d3:	add    -0x47fd4bfe(%rbp),%dh
+   1800f96d9:	add    %dl,%al
+   1800f96db:	add    -0x30fd4cfe(%rsi),%dh
+   1800f96e1:	add    %cl,%cl
+   1800f96e3:	add    %ch,%cl
+   1800f96e5:	add    %dh,%cl
+   1800f96e7:	add    -0x43fd45fe(%rbx),%bh
+   1800f96ed:	add    0x61006502(%rcx),%bh
+   1800f96f3:	add    %cl,0x0(%rdi)
+   1800f96f6:	rex.WRX add %r10b,0x0(%rdx)
+   1800f96fa:	pop    %rsp
+   1800f96fb:	add    %dl,0x0(%rax)
+   1800f96fe:	rex.WRB add %r13b,0x0(%r9)
+   1800f9702:	movsxd (%rax),%eax
+   1800f9704:	add    %ch,0x0(%eax)
+   1800f9708:	push   %rbp
+   1800f9709:	add    %dl,0x56(%rax,%rax,1)
+   1800f970d:	add    %dl,0x0(%rbx)
+   1800f9710:	(bad)
+   1800f9711:	in     $0x16,%al
    1800f9713:	addb   $0x0,(%rcx)
    1800f9716:	add    %al,(%rax)
    1800f9718:	jo     0x1800f96ed
    1800f971a:	add    $0x80,%al
    1800f971c:	add    %eax,(%rax)
    1800f971e:	add    %al,(%rax)
    1800f9720:	(bad)
@@ -297677,17 +297681,18 @@
    1800f9988:	jo     0x1800f99ef
    1800f998a:	outsb  %ds:(%rsi),(%dx)
    1800f998b:	insl   (%dx),%es:(%rdi)
    1800f998c:	insl   (%dx),%es:(%rdi)
    1800f998d:	pop    %rdi
    1800f998e:	xor    %esi,(%rdi)
    1800f9990:	xor    %esi,(%rsp,%rsi,1)
-   1800f9993:	xor    0x36323239(%rip),%esi        # 0x1b641cbd2
-   1800f9999:	(bad)
-   1800f999a:	xor    %ebx,0x6f(%rdi,%rsi,2)
+   1800f9993:	xor    0x30393932(%rip),%esi        # 0x1b048d2cb
+   1800f9999:	xor    (%rcx),%bh
+   1800f999b:	pop    %rsp
+   1800f999c:	ja     0x1800f9a0d
    1800f999e:	jb     0x1800f9a0b
    1800f99a0:	pop    %rsp
    1800f99a1:	jo     0x1800f9a0f
    1800f99a3:	(bad)
    1800f99a4:	je     0x1800f9a0c
    1800f99a6:	outsl  %ds:(%rsi),(%dx)
    1800f99a7:	jb     0x1800f9a16
@@ -297960,52 +297965,57 @@
    1800f9bdc:	add    %eax,(%rax)
    1800f9bde:	add    %al,(%rax)
    1800f9be0:	jnp    0x1800f9bf6
    1800f9be2:	scas   %es:(%rdi),%al
    1800f9be3:	rex.RXB loope 0x1800f9c60
    1800f9be6:	test   %bh,(%rdi)
 	...
-   1800f9bf8:	ds add %edi,(%rdx)
-   1800f9bfb:	add    %esp,(%rsi)
-   1800f9bfd:	add    %esp,0x35012901(%rip)        # 0x1b510c504
-   1800f9c03:	add    %esp,(%rdi)
-   1800f9c05:	add    %esp,(%rcx,%rax,1)
-   1800f9c08:	add    %edi,(%rcx,%r8,1)
-   1800f9c0c:	rex add %eax,0x1(%rcx)
-   1800f9c10:	sub    $0x2e012c01,%eax
-   1800f9c15:	add    %ebp,(%rbx)
-   1800f9c17:	add    %ecx,%ebx
-   1800f9c19:	add    %bh,%al
-   1800f9c1b:	add    -0x47fd4bfe(%rbp),%dh
-   1800f9c21:	add    %dl,%al
-   1800f9c23:	add    -0x30fd4cfe(%rsi),%dh
-   1800f9c29:	add    %cl,%cl
-   1800f9c2b:	add    %ch,%cl
-   1800f9c2d:	add    %dh,%cl
-   1800f9c2f:	add    -0x43fd45fe(%rbx),%bh
-   1800f9c35:	add    0x61006502(%rcx),%bh
-   1800f9c3b:	add    %cl,0x0(%rdi)
-   1800f9c3e:	rex.WRX add %r10b,0x0(%rdx)
-   1800f9c42:	pop    %rsp
-   1800f9c43:	add    %dl,0x0(%rax)
-   1800f9c46:	rex.WRB add %r13b,0x0(%r9)
-   1800f9c4a:	movsxd (%rax),%eax
-   1800f9c4c:	add    %ch,0x0(%eax)
-   1800f9c50:	push   %rbp
-   1800f9c51:	add    %dl,0x56(%rax,%rax,1)
-   1800f9c55:	add    %dl,0x0(%rbx)
-   1800f9c58:	add    %al,(%rcx)
-   1800f9c5a:	(bad)
-   1800f9c5b:	(bad)
-   1800f9c5c:	add    $0x5,%al
-   1800f9c5e:	add    (%rdx),%eax
-   1800f9c60:	or     %cl,(%rcx)
-   1800f9c62:	or     (%rbx),%cl
-   1800f9c64:	femms
-   1800f9c66:	or     $0x6c61660c,%eax
+   1800f9bf0:	add    %al,(%rcx)
+   1800f9bf2:	(bad)
+   1800f9bf3:	(bad)
+   1800f9bf4:	add    $0x5,%al
+   1800f9bf6:	add    (%rdx),%eax
+   1800f9bf8:	or     %cl,(%rcx)
+   1800f9bfa:	or     (%rbx),%cl
+   1800f9bfc:	femms
+   1800f9bfe:	or     $0xc,%eax
+   1800f9c03:	add    %al,(%rax)
+   1800f9c05:	add    %al,(%rax)
+   1800f9c07:	add    %bh,(%rsi)
+   1800f9c09:	add    %edi,(%rdx)
+   1800f9c0b:	add    %esp,(%rsi)
+   1800f9c0d:	add    %esp,0x35012901(%rip)        # 0x1b510c514
+   1800f9c13:	add    %esp,(%rdi)
+   1800f9c15:	add    %esp,(%rcx,%rax,1)
+   1800f9c18:	add    %edi,(%rcx,%r8,1)
+   1800f9c1c:	rex add %eax,0x1(%rcx)
+   1800f9c20:	sub    $0x2e012c01,%eax
+   1800f9c25:	add    %ebp,(%rbx)
+   1800f9c27:	add    %ecx,%ebx
+   1800f9c29:	add    %bh,%al
+   1800f9c2b:	add    -0x47fd4bfe(%rbp),%dh
+   1800f9c31:	add    %dl,%al
+   1800f9c33:	add    -0x30fd4cfe(%rsi),%dh
+   1800f9c39:	add    %cl,%cl
+   1800f9c3b:	add    %ch,%cl
+   1800f9c3d:	add    %dh,%cl
+   1800f9c3f:	add    -0x43fd45fe(%rbx),%bh
+   1800f9c45:	add    0x61006502(%rcx),%bh
+   1800f9c4b:	add    %cl,0x0(%rdi)
+   1800f9c4e:	rex.WRX add %r10b,0x0(%rdx)
+   1800f9c52:	pop    %rsp
+   1800f9c53:	add    %dl,0x0(%rax)
+   1800f9c56:	rex.WRB add %r13b,0x0(%r9)
+   1800f9c5a:	movsxd (%rax),%eax
+   1800f9c5c:	add    %ch,0x0(%eax)
+   1800f9c60:	push   %rbp
+   1800f9c61:	add    %dl,0x56(%rax,%rax,1)
+   1800f9c65:	add    %dl,0x0(%rbx)
+   1800f9c68:	data16 (bad)
+   1800f9c6a:	insb   (%dx),%es:(%rdi)
    1800f9c6b:	jae    0x1800f9cd2
    1800f9c6d:	add    %al,(%rax)
    1800f9c6f:	add    %dh,0x75(%rdx,%rsi,2)
    1800f9c73:	add    %al,%gs:(%rax)
    1800f9c76:	add    %al,(%rax)
    1800f9c78:	enter  $0x16f3,$0x80
    1800f9c7c:	add    %eax,(%rax)
@@ -298112,17 +298122,18 @@
    1800f9d58:	jo     0x1800f9dbf
    1800f9d5a:	outsb  %ds:(%rsi),(%dx)
    1800f9d5b:	insl   (%dx),%es:(%rdi)
    1800f9d5c:	insl   (%dx),%es:(%rdi)
    1800f9d5d:	pop    %rdi
    1800f9d5e:	xor    %esi,(%rdi)
    1800f9d60:	xor    %esi,(%rsp,%rsi,1)
-   1800f9d63:	xor    0x36323239(%rip),%esi        # 0x1b641cfa2
-   1800f9d69:	(bad)
-   1800f9d6a:	xor    %ebx,0x6f(%rdi,%rsi,2)
+   1800f9d63:	xor    0x30393932(%rip),%esi        # 0x1b048d69b
+   1800f9d69:	xor    (%rcx),%bh
+   1800f9d6b:	pop    %rsp
+   1800f9d6c:	ja     0x1800f9ddd
    1800f9d6e:	jb     0x1800f9ddb
    1800f9d70:	pop    %rsp
    1800f9d71:	jo     0x1800f9ddf
    1800f9d73:	(bad)
    1800f9d74:	je     0x1800f9ddc
    1800f9d76:	outsl  %ds:(%rsi),(%dx)
    1800f9d77:	jb     0x1800f9de6
@@ -497745,17 +497756,17 @@
    180169cf8:	movsxd 0x74(%rcx),%esp
    180169cfb:	imul   $0x26d00000,0x6e(%rdi),%ebp
    180169d02:	sbb    0x1(%rax),%al
    180169d08:	jo     0x180169d31
    180169d0a:	sbb    0x1(%rax),%al
    180169d10:	add    %al,(%rax)
    180169d12:	add    %al,(%rax)
-   180169d14:	mov    $0x663039,%ebx
-   180169d19:	add    %al,(%rax)
-   180169d1b:	add    %cl,-0x38000000(%rip)        # 0x148169d21
+   180169d14:	imul   $0x6630,(%rdi),%esi
+   180169d1a:	add    %al,(%rax)
+   180169d1c:	or     $0xc8000000,%eax
    180169d21:	add    (%rax),%eax
    180169d23:	add    %ch,0xf(%rax)
    180169d26:	(bad)
    180169d27:	add    %ch,-0x3(%rax)
    180169d2a:	(bad)
    180169d2b:	add    %al,(%rax)
    180169d2d:	add    %al,(%rax)
@@ -539165,16 +539176,18 @@
    180185fa0:	add    %ch,-0x50400000(%rdi)
    180185fa6:	add    %al,(%rax)
    180185fa8:	jo     0x180185f5a
    180185faa:	add    %al,(%rax)
    180185fac:	xor    %dh,-0x4e000000(%rcx)
    180185fb2:	add    %al,(%rax)
    180185fb4:	shl    $0xf,%dl
-   180185fb7:	add    %bh,-0x1d3bfff1(%rcx,%rcx,2)
-   180185fbe:	verr   (%rax)
+   180185fb7:	add    %cl,%ah
+   180185fb9:	sldt   %r12
+   180185fbd:	loop   0x180185fce
+   180185fbf:	add    %dh,(%rax)
    180185fc1:	rex.WX (bad)
    180185fc4:	xor    %al,%cl
    180185fc6:	add    %al,(%rax)
    180185fc8:	rex roll $0x0,(%rax)
    180185fcc:	add    %bh,%dh
    180185fce:	add    %al,(%rax)
    180185fd0:	and    %bh,%bh
@@ -584326,101 +584339,100 @@
    18019c09f:	add    %cl,0x70(%rdi)
    18019c0a2:	outsb  %gs:(%rsi),(%dx)
    18019c0a4:	rex.WRB
    18019c0a5:	rex.WRB
    18019c0a6:	cs fs insb (%dx),%es:(%rdi)
    18019c0a9:	insb   (%dx),%es:(%rdi)
    18019c0aa:	add    %al,(%rax)
-   18019c0ac:	sub    (%rcx),%eax
-   18019c0ae:	movsxd 0x4d(%rbp),%esi
+   18019c0ac:	add    %esp,0x75(%r11)
+   18019c0b0:	rex.WRB
    18019c0b1:	gs insl (%dx),%es:(%rdi)
    18019c0b3:	rex.B insb (%dx),%es:(%rdi)
    18019c0b5:	insb   (%dx),%es:(%rdi)
    18019c0b6:	outsl  %ds:(%rsi),(%dx)
    18019c0b7:	movsxd 0x76(%rdi),%ebx
    18019c0ba:	xor    (%rax),%al
-   18019c0bc:	xor    (%rcx),%al
-   18019c0be:	movsxd 0x4d(%rbp),%esi
+   18019c0bc:	add    %rsp,0x75(%rbx)
+   18019c0c0:	rex.WRB
    18019c0c1:	gs insl (%dx),%es:(%rdi)
    18019c0c3:	rex.RX jb 0x18019c12b
    18019c0c6:	gs pop %rdi
    18019c0c8:	jbe    0x18019c0fc
    18019c0ca:	add    %al,(%rax)
-   18019c0cc:	xchg   %eax,%esp
+   18019c0cc:	stos   %al,%es:(%rdi)
    18019c0cd:	add    %esp,0x75(%rbx)
    18019c0d0:	rex.WRB
    18019c0d1:	gs insl (%dx),%es:(%rdi)
    18019c0d3:	movsxd 0x79(%rax),%esi
    18019c0d6:	rex.W je 0x18019c148
    18019c0d9:	rex.R pop %rdi
    18019c0db:	jbe    0x18019c10f
-   18019c0dd:	add    %cl,0x4d756301(%rax)
+   18019c0dd:	add    %bl,0x4d756301(%rsi)
    18019c0e3:	gs insl (%dx),%es:(%rdi)
    18019c0e5:	movsxd 0x79(%rax),%esi
    18019c0e8:	rex.R je 0x18019c15a
    18019c0eb:	rex.W pop %rdi
    18019c0ed:	jbe    0x18019c121
-   18019c0ef:	add    %dl,0x4d756301(%rdx)
+   18019c0ef:	add    %ch,0x4d756301(%rax)
    18019c0f5:	gs insl (%dx),%es:(%rdi)
    18019c0f7:	movsxd 0x79(%rax),%esi
    18019c0fa:	rex.W je 0x18019c16c
    18019c0fd:	rex.R
    18019c0fe:	rex.B jae 0x18019c17a
    18019c101:	outsb  %ds:(%rsi),(%dx)
    18019c102:	movsxd 0x76(%rdi),%ebx
    18019c105:	xor    (%rax),%al
-   18019c107:	add    %al,0x4d756301(%rsi)
-   18019c10d:	gs insl (%dx),%es:(%rdi)
+   18019c107:	add    %bl,0x654d7563(%rcx,%rax,1)
+   18019c10e:	insl   (%dx),%es:(%rdi)
    18019c10f:	movsxd 0x79(%rax),%esi
    18019c112:	rex.R je 0x18019c184
    18019c115:	rex.W
    18019c116:	rex.B jae 0x18019c192
    18019c119:	outsb  %ds:(%rsi),(%dx)
    18019c11a:	movsxd 0x76(%rdi),%ebx
    18019c11d:	xor    (%rax),%al
-   18019c11f:	add    %al,0x4d756301(%rax)
+   18019c11f:	add    %dl,0x4d756301(%rsi)
    18019c125:	gs insl (%dx),%es:(%rdi)
    18019c127:	movsxd 0x79(%rax),%esi
    18019c12a:	rex.R je 0x18019c19c
    18019c12d:	rex.R
    18019c12e:	rex.B jae 0x18019c1aa
    18019c131:	outsb  %ds:(%rsi),(%dx)
    18019c132:	movsxd 0x76(%rdi),%ebx
    18019c135:	xor    (%rax),%al
-   18019c137:	add    %ah,0x47756300(%rbx)
-   18019c13d:	gs je  0x18019c185
+   18019c137:	add    %ah,0x65477563(%rax,%rax,1)
+   18019c13e:	je     0x18019c185
    18019c140:	jb     0x18019c1b4
    18019c142:	outsl  %ds:(%rsi),(%dx)
    18019c143:	jb     0x18019c193
    18019c145:	(bad)
    18019c146:	insl   (%dx),%es:(%rdi)
    18019c147:	add    %al,%gs:(%rax)
-   18019c14a:	add    (%rcx),%eax
-   18019c14c:	movsxd 0x49(%rbp),%esi
+   18019c14a:	or     $0x49756301,%eax
    18019c14f:	outsb  %ds:(%rsi),(%dx)
-   18019c150:	imul   $0x7563007e,0x0(%rax,%rax,1),%esi
+   18019c150:	imul   $0x7563007f,0x0(%rax,%rax,1),%esi
    18019c158:	rex.R jb 0x18019c1c4
    18019c15b:	jbe    0x18019c1c2
    18019c15d:	jb     0x18019c1a6
    18019c15f:	gs je  0x18019c1b8
    18019c162:	gs jb  0x18019c1d8
-   18019c165:	imul   $0x610000,0x6e(%rdi),%ebp
+   18019c165:	imul   $0x620000,0x6e(%rdi),%ebp
    18019c16c:	movsxd 0x44(%rbp),%esi
    18019c16f:	gs jbe 0x18019c1db
    18019c172:	movsxd 0x47(%rbp),%esp
    18019c175:	gs je  0x18019c178
-   18019c178:	add    %ah,%fs:0x75(%rbx)
+   18019c178:	add    %ah,%gs:0x75(%rbx)
    18019c17c:	rex.R
    18019c17d:	gs jbe 0x18019c1e9
    18019c180:	movsxd 0x47(%rbp),%esp
    18019c183:	gs je  0x18019c1c9
    18019c186:	outsl  %ds:(%rsi),(%dx)
    18019c187:	jne    0x18019c1f7
    18019c189:	je     0x18019c18b
-   18019c18b:	add    %ah,0x0(%rdx)
+   18019c18b:	add    %ah,0x0(%rbx)
    18019c18e:	movsxd 0x44(%rbp),%esi
    18019c191:	gs jbe 0x18019c1fd
    18019c194:	movsxd 0x47(%rbp),%esp
    18019c197:	gs je  0x18019c1db
    18019c19a:	je     0x18019c210
    18019c19c:	jb     0x18019c207
    18019c19e:	(bad)
@@ -584437,114 +584449,112 @@
    18019c1b8:	movsxd 0x43(%rbp),%esi
    18019c1bb:	je     0x18019c235
    18019c1bd:	rex.R
    18019c1be:	gs jae 0x18019c235
    18019c1c1:	jb     0x18019c232
    18019c1c3:	jns    0x18019c224
    18019c1c5:	jbe    0x18019c1f9
-   18019c1c7:	add    %ah,(%rcx)
+   18019c1c7:	add    %ah,(%rdx)
    18019c1c9:	add    %ah,0x75(%rbx)
    18019c1cc:	rex.XB je 0x18019c247
    18019c1cf:	push   %rax
    18019c1d0:	jne    0x18019c245
    18019c1d2:	push   $0x72727543
    18019c1d7:	outsb  %gs:(%rsi),(%dx)
    18019c1d9:	je     0x18019c23a
    18019c1db:	jbe    0x18019c20f
-   18019c1dd:	add    %bl,(%rdi)
+   18019c1dd:	add    %ah,(%rax)
    18019c1df:	add    %ah,0x75(%rbx)
    18019c1e2:	rex.XB je 0x18019c25d
    18019c1e5:	push   %rax
    18019c1e6:	outsl  %ds:(%rsi),(%dx)
    18019c1e7:	jo     0x18019c22c
    18019c1e9:	jne    0x18019c25d
    18019c1eb:	jb     0x18019c252
    18019c1ed:	outsb  %ds:(%rsi),(%dx)
    18019c1ee:	je     0x18019c24f
    18019c1f0:	jbe    0x18019c224
    18019c1f2:	add    %al,(%rax)
-   18019c1f4:	and    $0x0,%al
-   18019c1f6:	movsxd 0x43(%rbp),%esi
+   18019c1f4:	and    $0x43756300,%eax
    18019c1f9:	je     0x18019c273
    18019c1fb:	push   %rbx
    18019c1fc:	gs je  0x18019c242
    18019c1ff:	jne    0x18019c273
    18019c201:	jb     0x18019c268
    18019c203:	outsb  %ds:(%rsi),(%dx)
    18019c204:	je     0x18019c206
-   18019c206:	and    (%rax),%eax
+   18019c206:	and    $0x0,%al
    18019c208:	movsxd 0x43(%rbp),%esi
    18019c20b:	je     0x18019c285
    18019c20d:	push   %rbx
    18019c20e:	gs je  0x18019c254
    18019c211:	(bad)
    18019c212:	movsxd 0x65(%rax),%ebp
    18019c215:	rex.XB outsl %ds:(%rsi),(%dx)
    18019c217:	outsb  %ds:(%rsi),(%dx)
-   18019c218:	imul   $0x1c4,0x0(%rdi),%sp
+   18019c218:	imul   $0x1da,0x0(%rdi),%sp
    18019c21e:	movsxd 0x4d(%rbp),%esi
    18019c221:	outsl  %ds:(%rsi),(%dx)
    18019c222:	fs jne 0x18019c291
    18019c225:	rex.WR outsl %gs:(%rsi),(%dx)
    18019c228:	(bad)
    18019c229:	add    %al,%fs:(%rax)
-   18019c22c:	movb   $0x63,(%rcx)
-   18019c22f:	jne    0x18019c27e
+   18019c22c:	faddl  (%rcx)
+   18019c22e:	movsxd 0x4d(%rbp),%esi
    18019c231:	outsl  %ds:(%rsi),(%dx)
    18019c232:	fs jne 0x18019c2a1
    18019c235:	rex.WR outsl %gs:(%rsi),(%dx)
    18019c238:	(bad)
    18019c239:	fs rex.R (bad)
    18019c23c:	je     0x18019c29f
    18019c23e:	rex.RB js 0x18019c241
-   18019c241:	add    %bh,0x4d756301(%rsi)
-   18019c247:	outsl  %ds:(%rsi),(%dx)
+   18019c241:	add    %dl,%ah
+   18019c243:	add    %esp,0x75(%rbx)
+   18019c246:	rex.WRB outsl %ds:(%rsi),(%dx)
    18019c248:	fs jne 0x18019c2b7
    18019c24b:	gs rex.RXB
    18019c24d:	gs je  0x18019c296
    18019c250:	jne    0x18019c2c0
    18019c252:	movsxd 0x6f(%rcx,%rbp,2),%esi
    18019c256:	outsb  %ds:(%rsi),(%dx)
-   18019c257:	add    %dh,(%rcx)
-   18019c259:	add    %esp,0x75(%rbx)
-   18019c25c:	rex.WRB
+   18019c257:	add    %al,0x1(%rdi)
+   18019c25a:	movsxd 0x4d(%rbp),%esi
    18019c25d:	gs insl (%dx),%es:(%rdi)
    18019c25f:	rex.RX jb 0x18019c2c7
    18019c262:	rex.W outsl %gs:(%rsi),(%dx)
    18019c265:	jae    0x18019c2db
-   18019c267:	add    %bh,(%rbx)
-   18019c269:	add    %esp,0x75(%rbx)
-   18019c26c:	rex.WRB
+   18019c267:	add    %dl,0x1(%rcx)
+   18019c26a:	movsxd 0x4d(%rbp),%esi
    18019c26d:	gs insl (%dx),%es:(%rdi)
    18019c26f:	rex.W outsl %ds:(%rsi),(%dx)
    18019c271:	jae    0x18019c2e7
    18019c273:	rex.B insb (%dx),%es:(%rdi)
    18019c275:	insb   (%dx),%es:(%rdi)
    18019c276:	outsl  %ds:(%rsi),(%dx)
    18019c277:	movsxd (%rax),%eax
-   18019c279:	add    %al,(%rbx)
+   18019c279:	add    %bl,(%rbx)
    18019c27b:	add    0x75(%rbx),%ah
    18019c27e:	push   %rbx
    18019c27f:	je     0x18019c2f3
    18019c281:	gs (bad)
    18019c283:	insl   (%dx),%es:(%rdi)
    18019c284:	push   %rbx
    18019c285:	jns    0x18019c2f5
    18019c287:	movsxd 0x72(%rax),%ebp
    18019c28a:	outsl  %ds:(%rsi),(%dx)
    18019c28b:	outsb  %ds:(%rsi),(%dx)
-   18019c28c:	imul   $0x63011200,0x65(%rdx),%edi
+   18019c28c:	imul   $0x63012000,0x65(%rdx),%edi
    18019c293:	jne    0x18019c2e1
    18019c295:	(bad)
    18019c296:	jne    0x18019c306
    18019c298:	movsxd 0x4b(%rax),%ebp
    18019c29b:	gs jb  0x18019c30c
    18019c29e:	gs insb (%dx),%es:(%rdi)
    18019c2a0:	add    %al,(%rax)
-   18019c2a2:	pop    %rdi
+   18019c2a2:	(bad)
    18019c2a3:	add    %ah,0x75(%rbx)
    18019c2a6:	rex.R
    18019c2a7:	gs jbe 0x18019c313
    18019c2aa:	movsxd 0x43(%rbp),%esp
    18019c2ad:	(bad)
    18019c2ae:	outsb  %ds:(%rsi),(%dx)
    18019c2af:	movsxd 0x65(%r11),%esp
@@ -584558,77 +584568,78 @@
    18019c2c3:	(bad)
    18019c2c4:	(bad)
    18019c2c5:	insb   (%dx),%es:(%rdi)
    18019c2c6:	gs push %rax
    18019c2c8:	gs gs jb 0x18019c30d
    18019c2cc:	movsxd 0x65(%rbx),%esp
    18019c2cf:	jae    0x18019c344
-   18019c2d1:	add    %bl,%dl
+   18019c2d1:	add    %dh,%al
    18019c2d3:	add    %esp,0x75(%rbx)
    18019c2d6:	push   %rax
    18019c2d7:	jb     0x18019c348
    18019c2d9:	imul   $0x7453,0x72(%rbp,%riz,2),%bp
    18019c2e0:	outsl  %ds:(%rsi),(%dx)
    18019c2e1:	jo     0x18019c2e3
-   18019c2e3:	add    %bh,0x0(%rdi)
-   18019c2e6:	movsxd 0x45(%rbp),%esi
+   18019c2e3:	add    %al,0x45756300(%rax)
    18019c2e9:	jbe    0x18019c350
    18019c2eb:	outsb  %ds:(%rsi),(%dx)
    18019c2ec:	je     0x18019c331
    18019c2ee:	jb     0x18019c355
    18019c2f0:	(bad)
    18019c2f1:	je     0x18019c358
-   18019c2f3:	add    %al,0x76457563(%rax,%rax,1)
-   18019c2fa:	outsb  %gs:(%rsi),(%dx)
+   18019c2f3:	add    %al,0x45756300(%rbp)
+   18019c2f9:	jbe    0x18019c360
+   18019c2fb:	outsb  %ds:(%rsi),(%dx)
    18019c2fc:	je     0x18019c350
    18019c2fe:	movsxd %gs:0x72(%rdi),%ebp
-   18019c302:	add    %cl,%fs:0x45756300(%rax)
+   18019c302:	add    %cl,%fs:0x45756300(%rcx)
    18019c309:	jbe    0x18019c370
    18019c30b:	outsb  %ds:(%rsi),(%dx)
    18019c30c:	je     0x18019c361
    18019c30e:	jns    0x18019c37e
    18019c310:	movsxd 0x72(%rax),%ebp
    18019c313:	outsl  %ds:(%rsi),(%dx)
    18019c314:	outsb  %ds:(%rsi),(%dx)
-   18019c315:	imul   $0x810000,0x65(%rdx),%edi
+   18019c315:	imul   $0x820000,0x65(%rdx),%edi
    18019c31c:	movsxd 0x45(%rbp),%esi
    18019c31f:	jbe    0x18019c386
    18019c321:	outsb  %ds:(%rsi),(%dx)
    18019c322:	je     0x18019c368
    18019c324:	gs jae 0x18019c39b
    18019c327:	jb     0x18019c398
    18019c329:	jns    0x18019c38a
    18019c32b:	jbe    0x18019c35f
-   18019c32d:	add    %bh,0x4d756301(%rip)        # 0x1cd8f2634
+   18019c32d:	add    %dl,0x1(%rbx)
+   18019c330:	movsxd 0x4d(%rbp),%esi
    18019c333:	gs insl (%dx),%es:(%rdi)
    18019c335:	rex.W outsl %ds:(%rsi),(%dx)
    18019c337:	jae    0x18019c3ad
    18019c339:	rex.RXB
    18019c33a:	gs je  0x18019c381
    18019c33d:	gs jbe 0x18019c3a9
    18019c340:	movsxd 0x50(%rbp),%esp
    18019c343:	outsl  %ds:(%rsi),(%dx)
    18019c344:	imul   $0x765f7265,0x74(%rsi),%ebp
    18019c34b:	xor    (%rax),%al
-   18019c34d:	add    %cl,0x75467563(%rax,%rax,1)
-   18019c354:	outsb  %ds:(%rsi),(%dx)
+   18019c34d:	add    %cl,0x46756300(%rbp)
+   18019c353:	jne    0x18019c3c3
    18019c355:	movsxd 0x65(%rdi),%eax
    18019c358:	je     0x18019c39b
    18019c35a:	je     0x18019c3d0
    18019c35c:	jb     0x18019c3c7
    18019c35e:	(bad)
-   18019c363:	add    %ch,0x0(%rdx)
+   18019c363:	add    %ch,0x0(%rbx)
    18019c366:	movsxd 0x44(%rbp),%esi
    18019c369:	gs jbe 0x18019c3d5
    18019c36c:	movsxd 0x47(%rbp),%esp
    18019c36f:	gs je  0x18019c3c0
    18019c372:	(bad)
    18019c373:	insl   (%dx),%es:(%rdi)
-   18019c374:	gs add %ch,%bl
-   18019c377:	add    %esp,0x75(%rbx)
+   18019c374:	add    %al,%gs:(%rcx)
+   18019c377:	add    0x75(%rbx),%ah
    18019c37a:	push   %rbx
    18019c37b:	je     0x18019c3ef
    18019c37d:	gs (bad)
    18019c37f:	insl   (%dx),%es:(%rdi)
    18019c380:	rex.XB jb 0x18019c3e8
    18019c383:	(bad)
    18019c384:	je     0x18019c3eb
@@ -584638,44 +584649,43 @@
    18019c38c:	push   %rbx
    18019c38d:	je     0x18019c401
    18019c38f:	gs (bad)
    18019c391:	insl   (%dx),%es:(%rdi)
    18019c392:	push   %rdi
    18019c393:	(bad)
    18019c394:	imul   $0x746e65,0x76(%rbp,%rax,2),%esi
-   18019c39c:	out    %al,(%dx)
-   18019c39d:	add    %esp,0x75(%rbx)
-   18019c3a0:	push   %rbx
+   18019c39c:	add    $0x2,%al
+   18019c39e:	movsxd 0x53(%rbp),%esi
    18019c3a1:	je     0x18019c415
    18019c3a3:	gs (bad)
    18019c3a5:	insl   (%dx),%es:(%rdi)
    18019c3a6:	rex.R
    18019c3a7:	gs jae 0x18019c41e
    18019c3aa:	jb     0x18019c41b
    18019c3ac:	jns    0x18019c40d
    18019c3ae:	jbe    0x18019c3e2
    18019c3b0:	add    %al,(%rax)
-   18019c3b2:	nop
+   18019c3b2:	xchg   %eax,%ecx
    18019c3b3:	add    %ah,0x75(%rbx)
    18019c3b6:	rex.RX jne 0x18019c427
    18019c3b9:	movsxd 0x65(%rbx),%edx
    18019c3bc:	je     0x18019c401
    18019c3be:	(bad)
    18019c3bf:	movsxd 0x65(%rax),%ebp
    18019c3c2:	rex.XB outsl %ds:(%rsi),(%dx)
    18019c3c4:	outsb  %ds:(%rsi),(%dx)
-   18019c3c5:	imul   $0x2700,0x0(%rdi),%sp
+   18019c3c5:	imul   $0x2800,0x0(%rdi),%sp
    18019c3cb:	add    %ah,0x75(%rbx)
    18019c3ce:	rex.XB je 0x18019c449
    18019c3d1:	push   %rbx
    18019c3d2:	jns    0x18019c442
    18019c3d4:	movsxd 0x72(%rax),%ebp
    18019c3d7:	outsl  %ds:(%rsi),(%dx)
    18019c3d8:	outsb  %ds:(%rsi),(%dx)
-   18019c3d9:	imul   $0x16d0000,0x65(%rdx),%edi
+   18019c3d9:	imul   $0x1830000,0x65(%rdx),%edi
    18019c3e0:	movsxd 0x4d(%rbp),%esi
    18019c3e3:	gs insl (%dx),%es:(%rdi)
    18019c3e5:	movsxd 0x79(%rax),%esi
    18019c3e8:	rex.B jae 0x18019c464
    18019c3eb:	outsb  %ds:(%rsi),(%dx)
    18019c3ec:	movsxd (%rax),%eax
    18019c3ee:	outsb  %ds:(%rsi),(%dx)
@@ -584733,39 +584743,39 @@
    18019c46b:	add    %ah,0x75(%rbx)
    18019c46e:	data16 data16 je 0x18019c4b9
    18019c472:	gs je  0x18019c4cb
    18019c475:	gs jb  0x18019c4eb
    18019c478:	imul   $0x66756300,0x6e(%rdi),%ebp
    18019c47f:	data16 je 0x18019c4b8
    18019c482:	xor    $0x5f,%al
-   18019c484:	xor    %esi,(%rax)
+   18019c484:	xor    %esi,(%rcx)
    18019c486:	cs fs insb (%dx),%es:(%rdi)
    18019c489:	insb   (%dx),%es:(%rdi)
    18019c48a:	add    %al,(%rax)
    18019c48c:	(bad)
    18019c48d:	add    %ch,0x76(%rsi)
    18019c490:	jb     0x18019c506
    18019c492:	movsxd 0x65(%rdi),%eax
    18019c495:	je     0x18019c4dc
    18019c497:	jb     0x18019c50b
    18019c499:	outsl  %ds:(%rsi),(%dx)
    18019c49a:	jb     0x18019c4ef
    18019c49c:	je     0x18019c510
-   18019c49e:	imul   $0x6e000b00,0x67(%rsi),%ebp
+   18019c49e:	imul   $0x6e000d00,0x67(%rsi),%ebp
    18019c4a5:	jbe    0x18019c519
    18019c4a7:	je     0x18019c50c
    18019c4a9:	rex.RXB
    18019c4aa:	gs je  0x18019c4fb
    18019c4ad:	jne    0x18019c51c
    18019c4af:	push   %rbx
    18019c4b0:	jne    0x18019c522
    18019c4b2:	jo     0x18019c523
    18019c4b4:	jb     0x18019c52a
    18019c4b6:	gs fs rex.B jb 0x18019c51e
-   18019c4bb:	push   $0x100073
+   18019c4bb:	push   $0x140073
    18019c4c0:	outsb  %ds:(%rsi),(%dx)
    18019c4c1:	jbe    0x18019c535
    18019c4c3:	je     0x18019c528
    18019c4c5:	rex.RXB
    18019c4c6:	gs je  0x18019c51c
    18019c4c9:	jne    0x18019c53b
    18019c4cb:	jo     0x18019c53c
@@ -584800,55 +584810,56 @@
    18019c50d:	insl   (%dx),%es:(%rdi)
    18019c50e:	jo     0x18019c579
    18019c510:	insb   (%dx),%es:(%rdi)
    18019c511:	gs push %rax
    18019c513:	jb     0x18019c584
    18019c515:	addr32 jb 0x18019c579
    18019c518:	insl   (%dx),%es:(%rdi)
-   18019c519:	add    %cl,0x72766e00(%rip)        # 0x1f290331f
-   18019c51f:	je     0x18019c584
-   18019c521:	rex.RXB
-   18019c522:	gs je  0x18019c575
+   18019c519:	add    %dl,(%rcx)
+   18019c51b:	add    %ch,0x76(%rsi)
+   18019c51e:	jb     0x18019c594
+   18019c520:	movsxd 0x65(%rdi),%eax
+   18019c523:	je     0x18019c575
    18019c525:	push   %rsp
    18019c526:	pop    %rax
    18019c527:	push   %rbx
-   18019c528:	imul   $0x6e000c00,0x65(%rdx),%edi
+   18019c528:	imul   $0x6e001000,0x65(%rdx),%edi
    18019c52f:	jbe    0x18019c5a3
    18019c531:	je     0x18019c596
    18019c533:	rex.RXB
    18019c534:	gs je  0x18019c587
    18019c537:	push   %rsp
    18019c538:	pop    %rax
-   18019c539:	add    %cl,(%rdi)
+   18019c539:	add    %dl,(%rbx)
    18019c53b:	add    %ch,0x76(%rsi)
    18019c53e:	jb     0x18019c5b4
    18019c540:	movsxd 0x65(%rdi),%eax
    18019c543:	je     0x18019c595
    18019c545:	jb     0x18019c5b6
    18019c547:	addr32 jb 0x18019c5ab
    18019c54a:	insl   (%dx),%es:(%rdi)
    18019c54b:	rex.WR outsl %ds:(%rsi),(%dx)
    18019c54d:	addr32 push %rbx
-   18019c54f:	imul   $0xe0000,0x65(%rdx),%edi
+   18019c54f:	imul   $0x120000,0x65(%rdx),%edi
    18019c556:	outsb  %ds:(%rsi),(%dx)
    18019c557:	jbe    0x18019c5cb
    18019c559:	je     0x18019c5be
    18019c55b:	rex.RXB
    18019c55c:	gs je  0x18019c5af
    18019c55f:	jb     0x18019c5d0
    18019c561:	addr32 jb 0x18019c5c5
    18019c564:	insl   (%dx),%es:(%rdi)
    18019c565:	rex.WR outsl %ds:(%rsi),(%dx)
    18019c567:	add    %al,(%eax)
    18019c56a:	outsb  %ds:(%rsi),(%dx)
    18019c56b:	jbe    0x18019c5df
    18019c56d:	je     0x18019c5d2
    18019c56f:	ss xor $0x5f,%al
-   18019c572:	xor    %esi,(%rcx)
-   18019c574:	xor    0x30(%rdi),%bl
+   18019c572:	xor    %esi,(%rdx)
+   18019c574:	xor    %bl,0x30(%rdi)
    18019c577:	cs fs insb (%dx),%es:(%rdi)
    18019c57a:	insb   (%dx),%es:(%rdi)
    18019c57b:	add    %dh,(%rbx)
    18019c57d:	add    0x65(%rdi),%al
    18019c580:	je     0x18019c5c5
    18019c582:	jne    0x18019c5f6
    18019c584:	jb     0x18019c5eb
@@ -605479,19 +605490,20 @@
    1801aa2e5:	movabs 0xa1b8a1b0a1a8a1a0,%eax
    1801aa2ee:	shlb   $0xd8,-0x5e2f5e38(%rcx)
    1801aa2f5:	movabs 0xa230a228a1e8a1e0,%eax
    1801aa2fe:	cmp    %ah,-0x5db75dc0(%rdx)
    1801aa304:	push   %rax
    1801aa305:	movabs %al,0xa270a268a260a258
    1801aa30e:	js     0x1801aa2b2
-   1801aa310:	andb   $0x50,-0x55b755c0(%rdx)
+   1801aa310:	andb   $0x48,-0x55bf55c8(%rdx)
    1801aa317:	stos   %al,%es:(%rdi)
-   1801aa318:	push   $0xaa70aa
-   1801aa31d:	push   %rax
-   1801aa31e:	str    0x0(%rax)
+   1801aa318:	(bad)
+   1801aa319:	stos   %al,%es:(%rdi)
+   1801aa31a:	push   $0xf5000aa
+   1801aa31f:	add    %cl,0x0(%rax)
    1801aa322:	add    %al,(%rax)
    1801aa324:	shlb   $0xd8,-0x582f5838(%rdi)
    1801aa32b:	cmpsl  %es:(%rdi),%ds:(%rsi)
    1801aa32c:	loopne 0x1801aa2d5
    1801aa32e:	call   0x178c293da
    1801aa333:	cmpsl  %es:(%rdi),%ds:(%rsi)
    1801aa334:	add    %ch,-0x57ef57f8(%rax)
```

## OpenMM.libs/lib/plugins/OpenMMDrudeCUDA.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000dd6c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 00:23:18 2024
+Time/Date		Tue Apr 30 00:13:27 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000000e200
 SizeOfInitializedData	000000000000c600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000dd6c
@@ -27611,15 +27611,16 @@
    1800141ea:	add    %eax,0x1(%rax)
    1800141f0:	push   %rax
    1800141f1:	mov    $0x1,%bh
    1800141f3:	addb   $0x0,(%rcx)
    1800141f6:	add    %al,(%rax)
    1800141f8:	add    %al,(%rax)
    1800141fa:	add    %al,(%rax)
-   1800141fc:	idivb  (%rcx)
+   1800141fc:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   1800141fd:	(bad)
    1800141fe:	xor    %ah,0x0(%rsi)
    180014201:	add    %al,(%rax)
    180014203:	add    %cl,-0x20000000(%rip)        # 0x160014209
    180014209:	add    (%rax),%al
    18001420b:	add    %dl,0x52(%rax)
    18001420e:	add    %eax,(%rax)
    180014210:	push   %rax
```

## OpenMM.libs/lib/plugins/OpenMMRPMDCUDA.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800101cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 30 00:22:53 2024
+Time/Date		Tue Apr 30 00:12:59 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000010600
 SizeOfInitializedData	000000000000e200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000101cc
@@ -32801,15 +32801,15 @@
    180017910:	movsxd 0x74(%rcx),%esp
    180017913:	imul   $0xe7900000,0x6e(%rdi),%ebp
    18001791a:	add    %eax,0x1(%rax)
    180017920:	xor    %ch,%al
    180017922:	add    %eax,0x1(%rax)
    180017928:	add    %al,(%rax)
    18001792a:	add    %al,(%rax)
-   18001792c:	fnstsw (%rcx)
+   18001792c:	mov    (%rdi),%esi
    18001792e:	xor    %ah,0x0(%rsi)
    180017931:	add    %al,(%rax)
    180017933:	add    %cl,-0x20000000(%rip)        # 0x160017939
    180017939:	add    (%rax),%al
    18001793b:	add    %ah,(%rbx,%rcx,4)
    18001793e:	add    %eax,(%rax)
    180017940:	and    $0x75,%al
```

## Comparing `openmm_cuda-8.1.1.11.8.dist-info/RECORD` & `openmm_cuda-8.1.1.12.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-OpenMM.libs/lib/plugins/OpenMMAmoebaCUDA.dll,sha256=n8y3nGIJXtaFDJHw1Ab2SlTDjyIAfyspxjV-fwTWURA,1075712
-OpenMM.libs/lib/plugins/OpenMMCUDA.dll,sha256=PeQMRRfCWJJSLXy4SgIUfI98aweT8hlZm-WXQv9gZfw,1737216
-OpenMM.libs/lib/plugins/OpenMMDrudeCUDA.dll,sha256=8QPopLEZuSCYj_E915-22YeV2uKXW1qWmauWyI7rDJk,108032
-OpenMM.libs/lib/plugins/OpenMMRPMDCUDA.dll,sha256=TcPMVQ4eePlktZJ1Uqt3GBhSFkAwui5UyX14-7KM-T0,124416
-openmm_cuda-8.1.1.11.8.dist-info/METADATA,sha256=9d8Tu54lfQU_CKx9oPas4u4iXRIBlaU1R_dlxiTtYvw,96
-openmm_cuda-8.1.1.11.8.dist-info/RECORD,,
-openmm_cuda-8.1.1.11.8.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-openmm_cuda-8.1.1.11.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+OpenMM.libs/lib/plugins/OpenMMAmoebaCUDA.dll,sha256=Qg9MeIjOX1Bm4EncQFyAWx2BBU_rTZkS7fwarExgvZg,1075712
+OpenMM.libs/lib/plugins/OpenMMCUDA.dll,sha256=Vwf2Sr4Zufsm3v3hiCUC3ilFAvVCQzjcPTeuiizHt4A,1737216
+OpenMM.libs/lib/plugins/OpenMMDrudeCUDA.dll,sha256=uirVzmqRX7DWnW92ijcACEZUQ_c3jBBQfOnpCWtimTg,108032
+OpenMM.libs/lib/plugins/OpenMMRPMDCUDA.dll,sha256=yNWnvoV7Nr8cRrMa2AiT5fvwJ-KftVaAatObn7Naj7Q,124416
+openmm_cuda-8.1.1.12.dist-info/METADATA,sha256=n2-EUdvNeReXah832pGxNZ4OIh28uBuUuG_2UCPHpnQ,94
+openmm_cuda-8.1.1.12.dist-info/RECORD,,
+openmm_cuda-8.1.1.12.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+openmm_cuda-8.1.1.12.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
```

