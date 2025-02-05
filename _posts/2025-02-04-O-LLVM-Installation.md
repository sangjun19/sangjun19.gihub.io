---
title: "O-LLVM Installation"
date: 2025-02-04
description: "O-LLVM Installation"

---
  
---  
# O-LLVM 설치 방법
  
<br>

<span stype="font-size:50%">
참조 : https://github.com/obfuscator-llvm/obfuscator/wiki/Installation  
</span>

환경 : Ubuntu 24.04.1 LTS (GNU/Linux 6.8.0-51-generic x86_64)

>git clone -b llvm-4.0 https://github.com/obfuscator-llvm/obfuscator.git  


<p align="center">
  <img src="/assets/images/git_clone.png" style="display: block; margin: auto;">
</p>  

---  
>mkdir build  
cd build  

<p align="center">
  <img src="/assets/images/build.png" style="display: block; margin: auto;">
</p>  

---
>export CC=gcc-11  
export CXX=g++-11  
cmake -DCMAKE_BUILD_TYPE=Release -DLLVM_INCLUDE_TESTS=OFF ../obfuscator  
  
<p align="center">
  <img src="/assets/images/cmake.png" style="display: block; margin: auto;">
</p>  

---
>make -j8  
 
<p align="center">
  <img src="/assets/images/make-j8.png" style="display: block; margin: auto;">
</p>  
  
---

