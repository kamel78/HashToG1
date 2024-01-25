# HashToG1
Personalized implementation of the  Koshelev's proposed indifferentiable hashing to elliptic curves
https://eprint.iacr.org/2020/1070 


Demonstration for the BLS12-381 curve (case (q % 27) % 9 =10)

-   The proposed implementation is constant-time and about 20% faster thant the original one (if we ommit contant-time condition, it can be much faster).
-   Some precomputed constant are necessary (3 Lagrange coefficients !)
-   Functions phi, crtRatio and hprime are merged into one code
-   Benchmark is performed using generated data from the orginal implementation (included in "KoshilevTests.py")

Original implementation :
https://github.com/Dimitri-Koshelev/Indifferentiable-hashing-to-ordinary-elliptic-curves-of-j-0-with-the-cost-of-one-exponentiation
https://github.com/zhenfeizhang/indifferentiable-hashing?tab=readme-ov-file
