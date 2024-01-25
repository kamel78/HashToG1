# HashToG1

This is a personalized implementation of Koshelev's proposed indifferentiable hashing to elliptic curves, as described in the paper available at [https://eprint.iacr.org/2020/1070](https://eprint.iacr.org/2020/1070).

## Demonstration for the BLS12-381 Curve

(case \( (q \mod 27) \mod 9 = 10 \)):

- The proposed implementation is constant-time and approximately 20% faster than the original one (excluding the constant-time condition, it can be even faster).
- Some precomputed constants are required (3 Lagrange coefficients).
- The functions phi, crtRatio, and hprime are combined into a single code.
- Benchmarking is conducted using generated data from the original implementation, which is included in "KoshilevTests.py".

## Original Implementations

- [Dimitri-Koshelev's Implementation](https://github.com/Dimitri-Koshelev/Indifferentiable-hashing-to-ordinary-elliptic-curves-of-j-0-with-the-cost-of-one-exponentiation)
- [zhenfeizhang's Implementation](https://github.com/zhenfeizhang/indifferentiable-hashing?tab=readme-ov-file)

## Files

- "Koshelev-hash.ipynb": Contains codes ready to run under Jupyter.
- "KoshelevTests.py": Includes the benchmarking set taken from the original implementation.
