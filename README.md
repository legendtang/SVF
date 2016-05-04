SVF is a static tool that enables scalable and precise interprocedural dependence analysis for C programs. SVF allows value-flow construction and pointer analysis to be performed iteratively, thereby providing increasingly improved precision for both. 

SVF accepts the points-to information generated by any pointer analysis (e.g., Andersen’s analysis) and constructs an interprocedural memory SSA form so that the def-use chains of both top-level and address-taken variables are captured. SVF is implemented on top of an industry-strength compiler [LLVM](http://llvm.org) (version 3.8.0). SVF contains a third party software package [CUDD-2.5.0](http://vlsi.colorado.edu/~fabio/CUDD/) (Binary Decision Diagrams (BDDs)), which is used to encode path conditions.

<br />

| About SVF       | Setup  Guide         | User Guide  | Developer Guide  |
| ------------- |:-------------:| -----:|-----:|
| ![About](https://github.com/unsw-corg/SVF/blob/gh-pages/images/help.png?raw=true)| ![Setup](https://github.com/unsw-corg/SVF/blob/gh-pages/images/tools.png?raw=true)  | ![User](https://github.com/unsw-corg/SVF/blob/gh-pages/images/users.png?raw=true)  |  ![Developer](https://github.com/unsw-corg/SVF/blob/gh-pages/images/database.png?raw=true) 
| Introducing SVF -- [what it does](https://github.com/unsw-corg/SVF/wiki/About#what-is-svf) and [how we design it](https://github.com/unsw-corg/SVF/wiki/SVF-Design#svf-design)      | A step by step [setup guide](https://github.com/unsw-corg/SVF/wiki/Setup-Guide#getting-started) to build SVF | Command-line to [run SVF](https://github.com/unsw-corg/SVF/wiki/User-Guide#quick-start), get [analysis outputs](https://github.com/unsw-corg/SVF/wiki/User-Guide#analysis-outputs), and test with [an example](https://github.com/unsw-corg/SVF/wiki/Analyze-a-Simple-C-Program) | Detailed [technical documentation](https://github.com/unsw-corg/SVF/wiki/Technical-documentation) and how to [write your own analyses](https://github.com/unsw-corg/SVF/wiki/Write-your-own-analysis-in-SVF) on top of SVF |


<br />
If you use SVF, you are asked to acknolwedge usage of our tool by citing some of our publications listed in the [homepage](http://unsw-corg.github.io/SVF/) of this web site, especially the following two papers:

Yulei Sui and Jingling Xue. [SVF: Interprocedural Static Value-Flow Analysis in LLVM](http://www.cse.unsw.edu.au/~ysui/papers/cc16.pdf) Compiler Construction (CC '16) 

Yulei Sui, Ding Ye, and Jingling Xue. [Detecting Memory Leaks Statically with Full-Sparse Value-Flow Analysis](http://www.cse.unsw.edu.au/~ysui/papers/tse14.pdf) , IEEE Transactions on Software Engineering (TSE'14) 



