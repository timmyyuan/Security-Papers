# Security Papers About Memory Safety

### NDSS

* **(2018)** CFIXX : Object Type Integrity of c++
* **(2018)** Back To The Epilogue: Evading Control Flow Guard via Unaligned Targets.
  * > BATE attack addresses the weakness that the MSVC compiler would not align all instructions in executables and dynamic link libraries, which makes programs protected by Control Flow Guard flows to invaild address such as epilogues. Using those pop-ret instructions in epilogues, the attack decomposes the control flow integrity and chains ROP attack to achieve control flow haijack.
* **(2017)** Stack Object Protection with Low Fat Pointers

### CCS

* **(2017)** FreeGuard : A Faster Secure Heap Allocator
* **(2015)** Control Jujutsu: On the Weaknesses of Fine-Grained Control Flow Integrity

### Oakland

* **(2015)** Counterfeit Object-oriented Programming: On the Difficult of Preventing Code Reuse Attacks in C++ Applications

### USENIX Security

* **(2014)** Enforcing Forward-Edge Control-Flow Integrity in GCC & LLVM
