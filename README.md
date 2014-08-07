Rocket Core Generator
================================================================

Rocket is a 6-stage single-issue in-order pipeline that executes the 64-bit
scalar RISC-V ISA.  Rocket implements an MMU that supports page-based virtual
memory and is able to boot modern operating systems such as Linux.  Rocket
also has an optional IEEE 754-2008-compliant FPU, which implements both
single- and double-precision floating-point operations, including fused
multiply-add.

The following table compares a 32-bit ARM Cortex-A5 core to a 64-bit RISC-V
Rocket core built in the same TSMC process (40GPLUS). Fourth column is the
ratio of RISC-V Rocket to ARM Cortex-A5. Both use single-instruction-issue,
in-order pipelines, yet the RISC-V core is faster, smaller, and uses less
power.

 | ARM Cortex-A5 | RISC-V Rocket | R/A
--- | --- | --- | ---
ISA Register Width | 32 bits | 64 bits | 2
Frequency | >1 GHz | >1 GHz | 1
Dhrystone Performance | 1.57 DMIPS/MHz | 1.72 DMIPS/MHz | 1.1
Area excluding caches | 0.27 mm^2 | 0.14 mm^2 | 0.5
Area with 16KB caches | 0.53 mm^2 | 0.39 mm^2 | 0.7
Area Efficiency | 2.96 DMIPS/MHz/mm^2 | 4.41 DMIPS/MHz/mm^2 | 1.5
Dynamic Power | <0.08 mW/MHz | 0.034 mW/MHz | >= 0.4

We plan to open-source our Rocket core generator in the near future.  We are
currently in the process of cleaning up the repository.  Please stay tuned.
