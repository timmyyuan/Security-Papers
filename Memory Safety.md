# Security Papers About Memory Safety

### NDSS

* **(2018)** CFIXX : Object Type Integrity of c++
> To avoid object corruption (e.g. when attcker try to construct a fake virtual table), the author separate (using hash like page tables) the vtable pointer from the object allocation (that is, this pointer) to a additional metadata area protected by Intel MPX. When programs being executed, all the virual function calls will be checked according the metadata area. This approach can significant improve the weakness of the well-accepted coarse-grained CFI and the overhead is lower than 2% even in chrome.
* **(2018)** Back To The Epilogue: Evading Control Flow Guard via Unaligned Targets.
> BATE attack addresses the weakness that the MSVC compiler would not align all instructions in executables and dynamic link libraries, which makes programs protected by Control Flow Guard flows to invaild address such as epilogues. Using those pop-ret instructions in epilogues, the attack decomposes the control flow integrity and further chains ROP gadgets to haijack control flows.
* **(2018)** Automated Generation of Event-Oriented Exploits in Android Hybrid Apps
* **(2018)** JavaScript Zero: Real JavaScript and Zero Side-Channel Attacks
* **(2018)** SYNODE: Understanding and Automatically Preventing Injection Attacks on NODE.JS.
* **(2017)** A Call to ARMs: Understanding the Costs and Benefits of JIT Spraying Mitigations
  * (reading 2010) JIT Spraying and Mitigations
* **(2017)** Stack Object Protection with Low Fat Pointers
* **(2016)** Leakage-Resilient Layout Randomization for Mobile Devices

### CCS

* **(2017)** FreeGuard : A Faster Secure Heap Allocator
  * (reading 1994) The Slab Allocator: An Object-Caching Kernel Memory Allocator
  * (reading 1995) Dynamic Storage Allocation: A Survey and Critical Review
  * (reading 2015) Understanding glibc malloc
* **(2017)** The Dynamics of Innocent Flesh on the Bone: Code Reuse Ten Years Later
* **(2015)** Control Jujutsu: On the Weaknesses of Fine-Grained Control Flow Integrity
* **(2015)** The Performance Cost of Shadow Stacks and Stack Canaries
* **(2014)** You Can Run but You Can’t Read: Preventing Disclosure Exploits in Executable Code

### Oakland

* **(2015)** Counterfeit Object-oriented Programming: On the Difficult of Preventing Code Reuse Attacks in C++ Applications
* **(2015)** Readactor: Practical Code Randomization Resilient to Memory Disclosure.
* **(2013)** Just-In-Time Code Reuse: On the Effectiveness of Fine-Grained Address Space Layout Randomization
> Since the memory address randomization be well-accepted, multiple memory disclosures has been necessary to craft a ROP attack. Based on this observation, the paper programms adversary routines just-in-time to replace the hard code wrote by experienced attackers. In theory, JIT-ROP shatters the illusion of fine-grained randomization migitation defences.

### USENIX Security

* **(2017)** Oscar: A Practical Page-Permissions-Based Scheme for Thwarting Dangling Pointers
* **(2016)** What Cannot Be Read, Cannot Be Leveraged? Revisiting Assumptions of JIT-ROP Defenses
* **(2015)** Automatic Generation of Data-oriented exploits
> Ever since the control flow haijack has been diffcult to undermine the modern security defenses, data becomes a more feasible attack surface for adversaries. This paper introduced a new approach namely Data Flow Stitch and its implementation FlowStitch, which modifies the noraml data flow to craft information leak and privilege escalation. Based on known vulnerabilities (i.e., buffer overflow and string format vulnerability), Data Flow Stitch selects and filters candidates (i.e., data edges) to stitch vaild data-oriented attacks and be practical on 32-bit and 64-bit programs even under the ASLR.
* **(2014)** Enforcing Forward-Edge Control-Flow Integrity in GCC & LLVM

### OSDI
* **(2016)** Shuffler: Fast and Deployable Continuous Code Re-Randomization

## VEE
* **(2017)** RERANZ: A Light-Weight Virtual Machine to Mitigate Memory Disclosure Attacks

### ASE

* **(2017)** Automatically Assessing Crashes from Heap Overflows

### RAID

* **(2012)** The Last Mile: An Empirical Study of Timing Channels on seL4
