# TIPSBP1

To 'install,' download the package and unzip it. 

This program was compiled with PackageCompiler on:
Julia Version 1.7.3
Commit 742b9abb4d (2022-05-06 12:58 UTC)
Platform Info:
  OS: macOS (x86_64-apple-darwin21.4.0)
  CPU: Apple M2
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-12.0.1 (ORCJIT, westmere)
Environment:
  JULIA_EDITOR = code
  JULIA_NUM_THREADS = 

Runtime: 
real	0m20.764s
user	0m19.021s
sys	0m1.535s

This executable TIPSBP1 reproduces the data in Figures 2 and 3. It can be run with the default parameters D, X, and beta from the paper, "Spin Polarized Excitons from Singlet Fission," or with chosen parameters. To run with default parameters, open a terminal and cd to the path that contains the executable file TIPSBP1_compiled/bin/TIPSBP1. Then execute the program,

./TIPSBP1

To specify unique values of D, X, and beta (in that order) run,

./TIPSBP1 D X beta

where D (MHz), X (MHz), and beta (degree) are replaced by the chosen values.

Information regarding the calculations are detailed in the Supporting Notes 2.4-2.6. 

This populates the Data folder with the data for all figures. The resulting csv text files are:

Year-Month-Day_Figure2.txt: the first column is the field values (mT), the second is the calculated spectrum 
in 2a, the third 2b, and the fourth 2c.

Year-Month-Day_Figure3a-Eigenvalues-Bi.txt: column one is the field in mT, columns 2-6 are the eigenvalues of the quintet M-levels for B||i, where i is x, y, or z.

Year-Month-Day_Figure3a-Hankel.txt: column one is the field in mT, columns 2-4 are the M = 0 ↔ ± 1 transitions for B||z, B||x, B||y, respectively.

Year-Month-Day_Figure3a-Populations-Bi.txt: column one is the field in mT, column two is the energy in GHz, column three is the population for the four quintet transitions when the field is along the dimer axes i = x, y, or z. Arrows in the figure are drawn from the states with low to high population at a given resonance.

Year-Month-Day_Figure3a-Residual.txt: column one is the field in mT, columns 2-4 are the M = ± 1 ↔ ± 2 transitions for B||z, B||x, B||y, respectively.

Year-Month-Day_Figure3d.txt: The first row of this matrix gives values of theta in degrees. The first column gives values of phi in degrees. The inner matrix values are the state selectivity for the corresponding (phi,theta).

Year-Month-Day_Figure3e_M.txt: The first row of this matrix gives values of theta in degrees. The first column gives values of phi in degrees. The inner matrix values are the populations for the corresponding (phi,theta) and the M-level, M = -2, -1, 0, 1, 2.