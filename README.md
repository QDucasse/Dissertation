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

- [X] 1989-Imel
- [X] 2008-Baboulin
- [X] 2008-Strzodka
- [X] 2008-Sun
- [ ] 2009-Goddeke
- [X] 2010-Clark
- [X] 2012-Chow
- [ ] 2012-LeGrand
- [ ] 2018-Darulova
- [ ] 2018-LeGallo

## Important sites
- Precision analysis tools: https://fpbench.org/community.html
- Single and double precision summary: https://blogs.nvidia.com/blog/2019/11/15/whats-the-difference-between-single-double-multi-and-mixed-precision-computing/
- Floating-point standards: https://www.doc.ic.ac.uk/~eedwards/compsys/float/

Mixed-precision applications:
- Climate analytics: https://dl.acm.org/doi/10.1109/SC.2018.00054
- Opioid addiction: https://dl.acm.org/doi/10.5555/3291656.3291732
- Nuclear fusion simulation: https://www.ornl.gov/news/david-green-teaming-solve-questions-fusion


## Planning and Deadlines

- Research Report Draft - 16/03
- Research Report Final - 08/04 3:30pm

## Logs

19/02
Re-read 2008-Strzodka and read 2008-Sun

21/02
Re-read 1989-Imel & 2008-Baboulin

23/02
Corrections on 2008-Strzodka and 2008-Sun

27/02
Read 2010-Clark
