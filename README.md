# Dissertation
Literature corpus of my MSc's dissertation thesis.

## Author:
- Quentin DUCASSE (qd14@hw.ac.uk)

## Subject

Many  embedded systems are based on the use of generic or dedicated processors.
These processors have hardware calculation units of variable precision (examples:
ALU or FPU 8, 16, 32, 64 bits).
Some processing algorithms are designed to perform calculations based on a given
accuracy. However, the use of calculations with lower accuracy allows, in some
cases, an acceleration of these same calculations while maintaining sufficient
accuracy for the desired functionality. This acceleration can have several
benefits:
- A reduction in the cost of the calculating component: a less powerful component
is generally cheaper,
- Better energy efficiency: a less powerful component or with a lower frequency/
voltage consumes less energy, and dissipates less heat,
- Better performance: reduced computing time allows you to work on larger datasets
or perform other calculations at constant cost.

The objective of the internship is to analyse a reference application, determine
the parts of code where accuracy can be reduced, and then implement it on one or
more hardware architectures to verify that the accuracy is sufficient and the
performance gain makes sense.
The trainee will have to appropriate the existing digital precision analysis
tools, then implement these tools on an algorithm, to analyse on each code
portion, the loss of precision and its level of acceptability. This step will be
performed on a sequential code in C or C++, in order to allow the use of tools
that do not support the parallelised code.  This first stage will rely on LLVM
or Clang.

In a second step, the application will be based on an architecture with computing
unit(s) of the desired precision (GPU or MPPA). Depending on the profiling and
the results of the analysis, the application code will be modified to take
advantage of the targeted computing units (meaning, exploiting an extended ISA,
with extra instructions that invoke hardware primitives).  
Finally, the global architecture (processor + hardware primitives) will be built
automatically, and the impact of a malicious alteration of synthesis scripts will
be illustrated to motivate the need for cyber-protection when designing such a soc.

## Structure of the literature review
The first part of the literature review will review the different vectors of
precision. What are the elements of a program that have an impact on precision?
Types, sampling, frequency?
The second part will look at the possible applications of such

## Articles read and annotated

- [X] 1989-Imel: Mixed-precision operations from a single opcode
- [X] 2001-Yates: Fixed-point arithmetic, an introduction
- [X] 2008-Baboulin: Accelerating computations with mixed-precision
- [X] 2008-Strzodka: Pipelined mixed-precision on FPGAs
- [X] 2008-Sun: Mixed-precision linear-solver for FPGAs
- [ ] 2009-Goddeke: Performance of solvers in FEM simulations
- [X] 2010-Clark: GPUs mixed-precision lattice QCD solvers
- [X] 2012-Chow: Mixed-precision Monte-Carlo methodology for FPGAs
- [X] 2012-LeGrand: Mixed-Molecular GPU model for molecular dynamics
- [X] 2013-Darulova: Synthesis of fixed-point programs
- [ ] 2013-RubioGonzalez: Precimonius, tuning assistant for FP programs
- [ ] 2014-XuanSang: From Smalltalk to Silicon: Turn Smalltalk code into FPGA
- [ ] 2018-Colangelo: Low numeric Precision Deep Learning inference
- [X] 2018-Darulova: Sound mixed-precision with rewriting
- [ ] 2018-Jia: Deep learning training system
- [ ] 2018-Joubert: Attacking the opioid epidemic
- [ ] 2018-Kurth: Exascale deep learning for climate analysis
- [X] 2018-LeGallo: Mixed-precision in-memory computing
- [ ] 2018-Narang: Mixed-precision training

## Important sites
Precision analysis:
- Precision analysis tools: https://fpbench.org/community.html

Floating-point and fixed-point arithmetic:
- Single and double precision summary: https://blogs.nvidia.com/blog/2019/11/15/whats-the-difference-between-single-double-multi-and-mixed-precision-computing/
- Floating-point standards: https://www.doc.ic.ac.uk/~eedwards/compsys/float/
- Computerphile, Floating point representations:
  - Part1: https://www.youtube.com/watch?v=PZRI1IfStY0
  - Part2: https://www.youtube.com/watch?v=f4ekifyijIg
  - Part3: https://www.youtube.com/watch?v=782QWNOD_Z0

Mixed-precision applications:
- Climate analytics: https://dl.acm.org/doi/10.1109/SC.2018.00054
- Opioid addiction: https://dl.acm.org/doi/10.5555/3291656.3291732
- Nuclear fusion simulation: https://www.ornl.gov/news/david-green-teaming-solve-questions-fusion


## Planning and Deadlines

- Research Report Draft - 16/03
- Research Report Final - 08/04 3:30pm

## Logs
15/02
Read and annotated 1989-Imel

16/02
Read and annotated 2008-Strzodka

17/02
Read 2008-Baboulin

19/02
Re-read 2008-Strzodka and read 2008-Sun.

21/02
Re-read 1989-Imel & 2008-Baboulin.

23/02
Corrections on 2008-Strzodka and 2008-Sun.

27/02
Read and annotated 2010-Clark.

28/02
Read and annotated 2012-LeGrand and 2018-Darulova.

29/02
Read and annotated 2018-LeGallo.

01/03
Found applications and uses of mixed-precision in diverse fields
2018-Joubert, 2018-Kurth.

02/03
Looking for material regarding fixed-point and floating-point
arithmetic. Computerphile serie and 2001-Yates document.
Read and annotated 2013-Darulova.

08/03

09/03

10/03

11/03
