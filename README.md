**# physicell**
How to install PhysiCell cell simulator in windows server and run Physicell using HPC.

**Youtube : **
https://youtu.be/C9rEP6v_A7E

**Documentation: **
https://github.com/MathCancer/PhysiCe...

**Download Links : **
________________________________________________________________________
**PhysiCell  - Download link**
https://sourceforge.net/projects/phys...

**Msys2 related information:** 
https://www.msys2.org/ 

**Msys2 download url: **
https://github.com/msys2/msys2-instal...

**Anaconda ( Phython ) :**
https://repo.anaconda.com/archive/Ana...

**Install Steps : **

**Step 1: **
Run packman to install below packages automatically. 

$ pacman -S mingw-w64-x86_64-binutils mingw-w64-x86_64-gcc mingw-w64-x86_64-headers-git mingw-w64-x86_64-gcc-libs mingw-w64-x86_64-libwinpthread-git mingw-w64-x86_64-winpthreads-git mingw-w64-x86_64-lapack mingw-w64-x86_64-openblas mingw-w64-x86_64-libxml2 mingw-w64-x86_64-bzip2 git make

**Individual package:** 
pacman -S 
mingw-w64-x86_64-binutils 
mingw-w64-x86_64-gcc 
mingw-w64-x86_64-headers-git 
mingw-w64-x86_64-gcc-libs 
mingw-w64-x86_64-libwinpthread-git 
mingw-w64-x86_64-winpthreads-git 
mingw-w64-x86_64-lapack 
mingw-w64-x86_64-openblas 
mingw-w64-x86_64-libxml2 
mingw-w64-x86_64-bzip2 
git 
make

**Manual download  : **

https://packages.msys2.org/package/

https://mirror.msys2.org/mingw/mingw6...

**Command to manual install local package**
pacman -U  /home/Administrator/mingw-w64-x86_64-libxml2-2.9.14-2-any.pkg.tar.zst

**Step 2:** 
Add below paths to System PATH variable and make sure they are at top of the list. 

C:\msys64\mingw64\bin
C:\msys64\usr\bin
.\addons\libRoadrunner\roadrunner\bin

**Step 3: **
Verify msys2 installation :
Launch a PowerShell or cmd  and below command  and make sure it returns g++ version. 
g++ --version

**Step 4 :**
Run physicell sample project : 
Extract physicell content to a folder.  Launch a powershell or command prompt and change working directory to Physicell folder. 

**Run below commands to compile and run sample project **

$ make biorobots-sample     #copy files for biorobots 
$ make                      # compile
$ ./biorobots.exe


# FFMPEG installation 

pacman -S mingw-w64-x86_64-ffmpeg
