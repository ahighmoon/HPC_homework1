The following results are obtained from Linux environment. The code is problem3.cpp, two executable files with opt flag -O0 and -O3 are p3-0 and p3-3

Number of iterations and time needed for two methods for different N:
N = 10    , Jacobi: 222     iterations, time = 1.38e-5s;
N = 10    , GS    : 112     iterations, time = 1.06e-5s;
N = 1000  , Jacobi: 1848917 iterations, time = 5.36547s;
N = 1000  , GS    : 924460  iterations, time = 9.19932s;
N = 100000, Jacobi: 5000    iterations, time = 1.68664s.
N = 100000, GS	  : 5000    iterations, time = 5.06998s. (I just run 5000 iterations for the case of N = 1e5, it takes too long for the algo to converge at this size)

Run times for N = 100000 for 100 iterations using different compiler optimization flags (-O0 and -O3):
Opt flag = O0: Jacobi runs for 0.27322s  , GS runs for 0.31037s.
Opt flag = O3: Jacobi runs for 0.0350783s, GS runs for 0.101439s.

The following information about my running computer architechure is obtained from the 'lscpu' command in Linux.

Architecture:                    x86_64
CPU op-mode(s):                  32-bit, 64-bit
Address sizes:                   39 bits physical, 48 bits virtual
Byte Order:                      Little Endian
CPU(s):                          8
On-line CPU(s) list:             0-7
Vendor ID:                       GenuineIntel
Model name:                      Intel(R) Core(TM) i5-10210U CPU @ 1.60GHz
CPU family:                      6
Model:                           142
Thread(s) per core:              2
Core(s) per socket:              4
Socket(s):                       1
Stepping:                        12
BogoMIPS:                        4224.01
Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon rep_good nopl xtopology cpuid pni pclmulqdq vmx ssse3 fma cx16 pdcm pcid sse4_1 sse4_2 movbe popcnt aes xsave avx f16c rdrand hypervisor lahf_lm abm 3dnowprefetch invpcid_single ssbd ibrs ibpb stibp ibrs_enhanced tpr_shadow vnmi ept vpid ept_ad fsgsbase bmi1 avx2 smep bmi2 erms invpcid rdseed adx smap clflushopt xsaveopt xsavec xgetbv1 xsaves flush_l1d arch_capabilities
Virtualization:                  VT-x
Hypervisor vendor:               Microsoft
Virtualization type:             full
L1d cache:                       128 KiB (4 instances)
L1i cache:                       128 KiB (4 instances)
L2 cache:                        1 MiB (4 instances)
L3 cache:                        6 MiB (1 instance)
Vulnerability Itlb multihit:     KVM: Mitigation: VMX disabled
Vulnerability L1tf:              Not affected
Vulnerability Mds:               Not affected
Vulnerability Meltdown:          Not affected
Vulnerability Mmio stale data:   Vulnerable: Clear CPU buffers attempted, no microcode; SMT Host state unknown
Vulnerability Retbleed:          Mitigation; Enhanced IBRS
Vulnerability Spec store bypass: Mitigation; Speculative Store Bypass disabled via prctl and seccomp
Vulnerability Spectre v1:        Mitigation; usercopy/swapgs barriers and __user pointer sanitization
Vulnerability Spectre v2:        Mitigation; Enhanced IBRS, IBPB conditional, RSB filling, PBRSB-eIBRS SW sequence
Vulnerability Srbds:             Unknown: Dependent on hypervisor status
Vulnerability Tsx async abort:   Not affected
