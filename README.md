# HashToG1
Personalized implementation of the  Koshelev's proposed indifferentiable hashing to elliptic curves

Demonstration for the BLS12-381 curve (case (q % 27) % 9 =10)

-   The proposed implementation is constant-time and about 25% faster thant the original one.
-   Some precomputed constant are necessary (3 lagurange coefficients !)
-   Functions phi, crtRatio and hprime are merged into one code
-   Benchmark is performed using generated data from the orginal implementation (included in "KoshilevTests.py")

