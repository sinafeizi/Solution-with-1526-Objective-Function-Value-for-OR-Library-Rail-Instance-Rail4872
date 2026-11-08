# Solution-with-1526-Objective-Function-Value-for-OR-Library-Rail-Instance-Rail4872
This repository provides selected-column indices supporting a solution of **1526 for the full OR-Library rail4872 set covering instance**, obtained using a reduced-cost-pool large neighborhood search matheuristic. The set covering model minimizes the total cost of selected columns subject to covering every row at least once. **The reported cost and feasibility refer to the full original instance, not merely a restricted core instance.**

In the paper’s original experiments, one of ten seeds reached a recorded objective value of 1526 within an 18,000-second run. However, the selected-column indices were not saved, preventing direct feasibility verification of that particular solution.

To investigate whether this result could be reproduced, ten additional runs were conducted with different random seeds and an 18,000-second time limit per run on a laptop with an **AMD Ryzen 5 5600H processor**. Three of these ten runs reached 1526, each producing a different set of selected columns.

The laptop CPU was faster than the Intel Xeon CPU used in the paper’s experiments. These additional runs therefore serve to verify the reported solution cost; they are not a hardware-controlled comparison of computational performance.

The column indices for all three solutions are publicly available in this repository. Anyone can use them with the **full original rail4872 data** to check that every row is covered and that the selected columns have a total cost of 1526. These additional results support the reproducibility of the reported objective value across multiple seeds and distinct column selections.
| Seed | Selected columns | Cost calculation | Rows covered | Uncovered rows |
|---|---:|---:|---:|---:|
| 24 | 1,038 | \(550 + 2(488)=1526\) | 4,872/4,872 | 0 |
| 28 | 1,046 | \(566 + 2(480)=1526\) | 4,872/4,872 | 0 |
| 29 | 1,028 | \(530 + 2(498)=1526\) | 4,872/4,872 | 0 |
