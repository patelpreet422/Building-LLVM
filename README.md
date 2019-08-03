```
ccmake -G Ninja -DCMAKE_INSTALL_PREFIX='/home/preet/llvm-project-s-s-c/bin-build' -DCMAKE_BUILD_TYPE=Release -DLLVM_ENABLE_PROJECTS='clang;clang-tools-extra;compiler-rt;libcxx;libcxxabi' ../llvm

.
|--llvm-install
|--llvm-build
`--llvm-project


sudo apt-get update
sudo apt-get upgrade
sudo apt-get install build-essential subversion swig python2.7-dev libedit-dev libncurses5-dev

git clone https://github.com/llvm/llvm-project
mkdir llvm-build
cd llvm-build
cmake -G Ninja -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/home/preet/lldb-install ../llvm-project/llvm -DLLVM_ENABLE_PROJECTS="clang;lldb;libcxx;libcxxabi;compiler-rt;clang-tools-extra" -DLLVM_OPTIMIZED_TABLEGEN=ON -DLLVM_PARALLEL_COMPILE_JOBS=2 -DLLVM_PARALLEL_LINK_JOBS=1 -DLLVM_ENABLE_DOXYGEN=ON -DLLVM_BUILD_DOCS=ON
ninja
ninja install
```

