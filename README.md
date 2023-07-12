<p align="center">
	<img src="assets/images/circuit.jpg">
</p>

<h1 align="center">
    Quine McCluskey Circuit Minimizer.
</h1>
  <p align="center">
 <img src="https://img.shields.io/github/release/Kumbong/quine_mccluskey.svg" />
 <img src="https://img.shields.io/github/issues/Kumbong/quine_mccluskey.svg">
 <img src="https://img.shields.io/github/issues-closed-raw/Kumbong/quine_mccluskey.svg">
 <img src="https://img.shields.io/snyk/vulnerabilities/github/Kumbong/quine_mccluskey.svg">
 <img src="https://img.shields.io/github/languages/top/kumbong/quine_mccluskey.svg">
 <img src="https://img.shields.io/codefactor/grade/github/kumbong/quine_mccluskey/master.svg">
 <img src="https://travis-ci.org/Kumbong/quine_mccluskey.svg?branch=master">
 </p>

An incredibly efficient, lightning-fast, and incredibly user-friendly command-line interface (CLI) tool for circuit reduction using the Quine McCluskey algorithm.

## Usage :computer:
You can use the following optional arguments according to your needs: 

   * `-d`, `--dcares` (list of numbers): **list of dont't cares (default=[ ])**
   * `-v`, `--variables` (list of chars): **list of characters for representing result (default = [ ])**
   * `-s`, `--show_steps` (yes|no): **show steps leading to solution (default=yes)**
   * `-p`, `--show_step` (sum of products): **sum of products are used to be reduce the function**
   * `-m`, `--show_step` (minterms): **sum of minterms are used to be reduce the function**
   
Example
```bash
    python -m qmccluskey -m 0,1,3,7,8,9,11,15 -d 12  -v a,b,c,d
    python -m qmccluskey -p a'b'c'+b'cd'+a'bcd'+ab'c' -v a,b,c,d
```
## Demo :movie_camera:
   Solution for the the Example above
   
   ![](assets/images/grouping.png)
   ![](assets/images/combining.png)
   ![](assets/images/coverage.png)
   ![](assets/images/solution.png)

MIT &copy; Smarak Patra
