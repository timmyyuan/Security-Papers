# Security Papers About Memory Safety

### NDSS

* **(2018)** CFIXX : Object Type Integrity of c++
> To avoid object corruption (e.g. when attcker try to construct a fake virtual table), the author separate (using hash like page tables) the vtable pointer from the object allocation (that is, this pointer) to a additional metadata area protected by Intel MPX. When programs being executed, all the virual function calls will be checked according the metadata area. This approach can significant improve the weakness of the well-accepted coarse-grained CFI and the overhead is lower than 2% even in chrome.
* **(2018)** Back To The Epilogue: Evading Control Flow Guard via Unaligned Targets.
> BATE attack addresses the weakness that the MSVC compiler would not align all instructions in executables and dynamic link libraries, which makes programs protected by Control Flow Guard flows to invaild address such as epilogues. Using those pop-ret instructions in epilogues, the attack decomposes the control flow integrity and further chains ROP gadgets to haijack control flows.
* **(2017)** Stack Object Protection with Low Fat Pointers

### CCS

* **(2017)** FreeGuard : A Faster Secure Heap Allocator
* **(2015)** Control Jujutsu: On the Weaknesses of Fine-Grained Control Flow Integrity

### Oakland

* **(2015)** Counterfeit Object-oriented Programming: On the Difficult of Preventing Code Reuse Attacks in C++ Applications

### USENIX Security

* **(2015)** Automatic Generation of Data-oriented exploits
> Ever since the control flow haijack has been diffcult to undermine the modern security defenses, data becomes a more feasible attack surface for adversaries. This paper introduced a new approach namely Data Flow Stitch and its implementation FlowStitch, which modifies the noraml data flow to craft information leak and privilege escalation. Based on known vulnerabilities (i.e., buffer overflow and string format vulnerability), Data Flow Stitch selects and filters candidates (i.e., data edges) to stitch vaild data-oriented attacks and be practical on 32-bit and 64-bit programs even under the ASLR.
* **(2014)** Enforcing Forward-Edge Control-Flow Integrity in GCC & LLVM

### ASE

* **(2017)** Automatically Assessing Crashes from Heap Overflows
