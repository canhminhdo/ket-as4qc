### An Algebraic Specification for Quantum Computation in Maude
---
This repository presents |AS4QC>, an algebraic specification for quantum computation in Maude.

## Dependencies
- Maude is a programming/specification language based on rewriting logic. How to download and install Maude can be found at [here](http://maude.cs.illinois.edu/w/index.php/The_Maude_System).

## How to install
- Clone the source code to your computer and go to the source code directory.

- Feed a Maude file that is the formal specification of a protocol of interest into Maude.

For example, we can type the following command in CLI to verify the correctness of Quantum Teleportation:

```console
cd examples && maude teleport.maude
```

- For testing, we can test the algebraic speicfication with some test cases provided as follows:

```console
cd test && ./tester
```

## Repository structure
- `cpx.maude` file for complex number reasoning.

- `qc.maude` file for quantum computation reasoning.

- `examples` folder for case studies.

- `test` folder for testing.
