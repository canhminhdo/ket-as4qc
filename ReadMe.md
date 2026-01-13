### An Algebraic Specification for Quantum Computation in Maude
---
This repository presents |AS4QC>, an algebraic specification for quantum computation in Maude, which provides a formal framework for modeling, symbolic and exact reasoning about, and verifying quantum systems.

## Dependencies
- Maude: A high-performance programming and specification language based on rewriting logic.\
Installation instructions are available at [here](http://maude.cs.illinois.edu/w/index.php/The_Maude_System).

## Usage
1. Clone this repository and navigate to the project directory.

2. Load the formal specification |AS4QC> to automate reasoning about quantum computation.

3. Feed a Maude file that is the formal specification of a protocol of interest into Maude.

For example, we can use the following command verify the correctness of Quantum Teleportation:

```console
cd examples && maude teleport.maude
```

For testing, we can validate the algebraic speicfication with some test cases as follows:

```console
cd test && ./tester
```

## Repository structure
- `cpx.maude` for complex number reasoning.

- `qc.maude` for quantum computation reasoning.

- `examples` for case studies.

- `test` for testing.
