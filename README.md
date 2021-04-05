# HW 1: Superoptimizer

### 1. Read through papers:
  * [_Dimensions in program synthesis_ (Gulwani 2010)](https://dl.acm.org/doi/10.1145/1836089.1836091)
  * [_Superoptimizer: a look at the smallest program_ (Massalin 1987)](https://dl.acm.org/doi/10.1145/36177.36194)
  * [_A Hacker's Assistant_ (Warren 2008)](https://github.com/dpt/Aha/blob/distrib/aha.pdf)


### 2. Aha experimentation
* Using provided functions (abs, avg), experimented with the following:
  * different numbers of instructions
  * different immediate operand sets
  * more extensive trial input-output pairs

### Average
| Operations | Solutions | Total Instructions  | Process Time (seconds) |
|------------|-----------|---------------------|------------------------|
| 1-3        | 0         | 133, 36200, 8220022 | ~0, 0.001, 0.154       |
| 4          | 3         | 31221243            | 75.880                 |
| 5          |           |                     |                        |


### Absolute Value
| Operations | Solutions | Total Instructions  | Process Time (seconds) |
|------------|-----------|---------------------|------------------------|
| 1-2        |  0        | 103, 11695          | ~0, ~0                 |
| 3          |  4        | 1857560             | 0.041                  |
| 4          |  951      | 571410152           | 11.962                 |
| 5          |           |                     |                        |



### 3. Experementation with Jeremy Berchtold's GPU Google Colab
* Experimentation with `multBy7` functions
  * Tested `(x<<3) - x` implementation vs other fast and traditional implementation
  * Tested differences in inline functions
