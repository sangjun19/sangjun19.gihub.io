---
title: "O-LLVM Installation"
date: 2025-02-04
description: "O-LLVM Installation"

---
  
---  
# O-LLVM 설치 방법
  
<br>
참조 : https://github.com/obfuscator-llvm/obfuscator/wiki/Installation  

환경 : Ubuntu 24.04.1 LTS (GNU/Linux 6.8.0-51-generic x86_64)

>git clone -b llvm-4.0 https://github.com/obfuscator-llvm/obfuscator.git  


<p align="center">
  <img src="/assets/images/git_clone.png" style="display: block; margin: auto;">
</p>  

---  
>mkdir build  
cd build  

![capture2](/assets/images/build.png)  
---
>export CC=gcc-11  
export CXX=g++-11  
cmake -DCMAKE_BUILD_TYPE=Release -DLLVM_INCLUDE_TESTS=OFF ../obfuscator  

![capture3](/assets/images/cmake.png)
---
>make -j8  

![capture4](/assets/images/make-j8.png)  

