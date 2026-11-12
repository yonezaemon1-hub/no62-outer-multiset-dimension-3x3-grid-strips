# Exact Outer Multiset Dimension of the Three-by-Three Path Grid Strips

Ryutaro Yonezu · Independent Researcher  
No.62 · Preprint v1.0 · 2026-11-10  
Computer-assisted mathematical proof

## Result

For every integer n ≥ 2, the outer multiset dimension of the Cartesian product
P₃ □ P₃ □ Pₙ is 6 for n = 3, 5 for n = 2 or 4 ≤ n ≤ 8, and 4 for n ≥ 9.
The lower bound of 4 for all n uses No.59's universal lower bound for
three nontrivial path factors. The small cases are settled by exhaustive finite
checks. For n ≥ 9, explicit four-landmark sets and exact finite collision
checks establish the upper bound.

The n = 2 graph is isomorphic to the n = 3 graph of the family studied in
No.58. The author's closeout reports this finite overlap, and No.59's
short-grid table gives the value 5. The published main theorem in No.58
covers n ≥ 6.

- [No.58 v1.0 — P₂ □ P₃ □ Pₙ](<https://github.com/yonezaemon1-hub/no58-outer-multiset-dimension-3d-grid/releases/tag/v1.0>)
- [No.59 v1.0 — universal lower bound and P₂-width classification](<https://github.com/yonezaemon1-hub/no59-outer-multiset-dimension-3d-grid-classification/releases/tag/v1.0>)

## Download and verify

The [v1.0 release](https://github.com/yonezaemon1-hub/no62-outer-multiset-dimension-3x3-grid-strips/releases/tag/v1.0) contains
the PDF, the matching TeX source, the reproducibility ZIP and SHA256SUMS.txt.
Download the three assets and the manifest to the same directory.
On Linux, run:

    sha256sum -c SHA256SUMS.txt

On Windows, use Get-FileHash -Algorithm SHA256 on each asset and compare the
result with SHA256SUMS.txt. Then extract No62_v1.0_REPRODUCIBILITY_20261110.zip.

## Reproduce

Use Python 3.10 or newer and a C++17 compiler on PATH (g++, clang++ or MSVC cl).
Run the following from the extracted directory containing the runner.
The checks use Python's standard library and write compilation products to a
temporary directory.

On Linux:

    python3 -B -I reproduce.py

On Windows PowerShell 5.1:

    py -3 -B -I .\reproduce.py

If your Python installation uses the python command, run
python -B -I reproduce.py instead. Keep Python assertions enabled. A full
run verifies the exact release inventory, the frozen file hashes and both
certificate outputs. The runner prints ALL_CERTIFICATES_PASS on success.
A missing C++17 compiler gives a nonzero exit and only partial reproduction.

The Python runner, the two frozen verifier sources, and the two frozen
expected outputs are byte-identical to v0.3. Historical wording in the frozen
outputs records the status when those files were made. The checksums inside
the ZIP apply to its contents.

## Evidence and rights

- **Independent AI differential audit through v0.3:** PASS in the author's
  supplied report. The scope covers the model, finite and infinite claims,
  editorial changes, package integrity, and privacy. Independent checks
  against landmark sets of size at most three were finite. The proof here
  uses No.59 for the general lower bound.
- **Windows PowerShell 5.1:** v0.3 PASS based on the author's supplied
  transcript. The v1.0 release package was checked on Linux. The package
  includes a sanitized summary of the Windows execution.
- **Novelty:** INCONCLUSIVE. **Human peer review:** not performed.
  **Full formal verification:** not performed.
- **Rights:** Copyright © 2026 Ryutaro Yonezu. All rights reserved.

## Author correspondence (metadata update, 2026-11-12)

**Ryutaro Yonezu — Independent Researcher**  
Research correspondence: **yonezaemon1+research@gmail.com**

This contact-information addition does not revise any mathematical claims, frozen verification files, published preprint PDF, release assets, DOI, or existing SHA256 checksums.
