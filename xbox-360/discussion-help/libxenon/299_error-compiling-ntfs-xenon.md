# Error compiling ntfs-xenon

## 2012-03-07 03:21:45, posted by: chemone

Hi all, I have a problem when compiling ntfs-xenon, I get this error: [code]* *[vfs.c] In file included from /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:22:0: /home/chemone/Escritorio/ntfs-xenon/source/./ntfsdir.h:59:71: warning: 'struct statvfs' declared inside parameter list [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./ntfsdir.h:59:71: warning: its scope is only this definition or declaration, which is probably not what you want [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c: In function 'zero\_malloc': /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:35:9: warning: implicit declaration of function 'memset' [-Wimplicit-function-declaration] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:35:9: warning: incompatible implicit declaration of built-in function 'memset' [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c: In function '\_ntfs\_readdir': /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:115:9: warning: implicit declaration of function 'strcpy' [-Wimplicit-function-declaration] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:115:9: warning: incompatible implicit declaration of built-in function 'strcpy' [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:117:9: warning: implicit declaration of function 'strlen' [-Wimplicit-function-declaration] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:117:23: warning: incompatible implicit declaration of built-in function 'strlen' [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c: In function '\_ntfs\_open': /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:134:19: warning: assignment makes pointer from integer without a cast [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:135:11: warning: comparison between pointer and integer [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c: In function '\_ntfs\_mount': /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:161:5: warning: implicit declaration of function 'ntfsFindPartitions' [-Wimplicit-function-declaration] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:165:9: warning: implicit declaration of function 'ntfsMount' [-Wimplicit-function-declaration] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c: In function '\_ntfs\_detect\_fs': /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:180:9: warning: format '%d' expects a matching 'int' argument [-Wformat] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:180:9: warning: format '%d' expects a matching 'int' argument [-Wformat] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c: At top level: /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:195:5: error: unknown field 'detect\_fs' specified in initializer /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:195:5: warning: excess elements in struct initializer [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:195:5: warning: (near initialization for 'vfs\_ntfs\_mount\_ops') [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:196:5: error: unknown field 'fs\_name' specified in initializer /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:196:5: warning: excess elements in struct initializer [enabled by default] /home/chemone/Escritorio/ntfs-xenon/source/./vfs.c:196:5: warning: (near initialization for 'vfs\_ntfs\_mount\_ops') [enabled by default] make[2]: *** [vfs.o] Error 1 [/code] I have Ubuntu 10.10 and all libxenon installed and updated.   
   
 Any idea what I can do? Thanks for the help.

## 2012-03-07 13:12:35, posted by: tuxuser

install libxenon repo from ced2911

## 2012-03-10 17:16:50, posted by: chemone

[quote="tuxuser"]  
 install libxenon repo from ced2911  
 [/quote]  
   
 It works. Thanks!!! ;)