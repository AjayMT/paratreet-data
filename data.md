
### jobscript-2

SMP on 10 stampede2 KNL nodes with batch resumes:

| Stage                             | 16 processes (48 PEs, 3 ppn) | 12 processes (36 PEs, 3 ppn) | 8 processes (24 PEs, 3 ppn) | 4 processes (12 PEs, 3 ppn) |
|-----------------------------------|------------------------------|------------------------------|-----------------------------|-----------------------------|
| Initialization                    | 18125.38ms                   | 18598.471ms                  | 21251.92ms                  | 26797.702ms                 |
| Iteration 0: Tree build           | 5783.440ms                   | 7095.227 ms                  | 10471.693 ms                | 20927.711 ms                |
| Iteration 0: Cache loading        | 207.137ms                    | 213.538 ms                   | 210.622 ms                  | 213.061 ms                  |
| Iteration 0: Tree traversal       | 96780.389ms                  | 128460.209 ms                | 184251.735 ms               | 344143.495 ms               |
| Iteration 0: Interactions         | 6055.636 ms                  | 7106.375 ms                  | 10339.393 ms                | 19808.942 ms                |
| Iteration 0: Perturbations        | 573.990 ms                   | 598.659 ms                   | 869.501 ms                  | 1664.991 ms                 |
| Iteration 0: Rebuilding universe  | 263.849 ms                   | 296.934 ms                   | 448.155 ms                  | 1101.849 ms                 |
| Iteration 0: Assigning keys       | 827.422 ms                   | 908.029 ms                   | 1370.126 ms                 | 2725.884 ms                 |
| Iteration 0: Setting up splitters | 2510.423 ms                  | 2527.363 ms                  | 2585.492 ms                 | 2651.774 ms                 |
| Iteration 0: Creating TreePieces  | 2426.733 ms                  | 2438.943 ms                  | 2677.013 ms                 | 3182.338 ms                 |
| Iteration 0: Flushing particles   | 637.729 ms                   | 668.310 ms                   | 813.539 ms                  | 1283.220 ms                 |
| Iteration 1: Tree build           | 5082.949ms                   | 6639.339 ms                  | 10137.153 ms                | 20485.006 ms                |
| Iteration 1: Cache loading        | 238.700ms                    | 215.895 ms                   | 207.997 ms                  | 232.083 ms                  |
| Iteration 1: Tree traversal       | 98770.732ms                  | 130656.217 ms                | 189015.760 ms               | 352277.477 ms               |
| Iteration 1: Interactions         | 6523.150ms                   | 8311.002 ms                  | 12349.273 ms                | 23255.547 ms                |
| Iteration 1: Perturbations        | 510.400ms                    | 676.756 ms                   | 855.834 ms                  | 1648.697 ms                 |
| Iteration 1: Rebuilding universe  | 271.405 ms                   | 342.849 ms                   | 540.124 ms                  | 1070.588 ms                 |
| Iteration 1: Assigning keys       | 776.541 ms                   | 1083.685 ms                  | 1513.204 ms                 | 2678.155 ms                 |
| Iteration 1: Setting up splitters | 2597.501 ms                  | 2691.454 ms                  | 2886.993 ms                 | 2679.617 ms                 |
| Iteration 1: Creating TreePieces  | 1275.151 ms                  | 1470.202 ms                  | 1865.254 ms                 | 2071.775 ms                 |
| Iteration 1: Flushing particles   | 670.919 ms                   | 716.740 ms                   | 821.257 ms                  | 1417.179 ms                 |
| Iteration 2: Tree build           | 5290.199ms                   | 6582.071 ms                  | 10163.556 ms                | 20185.194 ms                |
| Iteration 2: Cache loading        | 223.271ms                    | 224.563 ms                   | 221.827 ms                  | 219.073 ms                  |
| Iteration 2: Tree traversal       | 100882.504ms                 | 131414.039 ms                | 200854.332 ms               | 366317.288 ms               |
| Iteration 2: Interactions         | 7526.034ms                   | 9803.349 ms                  | 13758.656 ms                | 24971.683 ms                |
| Iteration 2: Perturbations        | 710.948ms                    | 631.694 ms                   | 849.286 ms                  | 1752.744 ms                 |
| Iteration 2: Rebuilding universe  | 268.971 ms                   | 345.890 ms                   | 505.978 ms                  | 1246.430 ms                 |
| Iteration 2: Assigning keys       | 982.235 ms                   | 1154.337 ms                  | 1525.665 ms                 | 2770.568 ms                 |
| Iteration 2: Setting up splitters | 2547.630 ms                  | 2615.023 ms                  | 2653.024 ms                 | 2566.340 ms                 |
| Iteration 2: Creating TreePieces  | 1272.177 ms                  | 1654.807 ms                  | 2054.862 ms                 | 2188.125 ms                 |
| Iteration 2: Flushing particles   | 706.183 ms                   | 723.382 ms                   | 854.797 ms                  | 1678.418 ms                 |
|-----------------------------------|------------------------------|------------------------------|-----------------------------|-----------------------------|
| Total runtime                     | 371319.73 ms                 | 476865.35 ms                 | 688924.02 ms                | 1256213.0 ms                |

non-SMP on 10 stampede2 KNL nodes with batch resumes:

| Stage                             | 48 processes | 36 processes  | 24 processes  | 12 processes  |
|-----------------------------------|--------------|---------------|---------------|---------------|
| Initialization                    | 15352.883ms  | 17397.185ms   | 18850.077 ms  | 22921.349ms   |
| Iteration 0: Tree build           | 4770.628 ms  | 5975.260 ms   | 8579.117 ms   | 15981.447 ms  |
| Iteration 0: Cache loading        | 213.237 ms   | 215.693 ms    | 217.186 ms    | 215.216 ms    |
| Iteration 0: Tree traversal       | 88717.042 ms | 108364.893 ms | 162029.570 ms | 289287.570 ms |
| Iteration 0: Interactions         | 6047.660 ms  | 7279.841 ms   | 10641.190 ms  | 20224.378 ms  |
| Iteration 0: Perturbations        | 530.387 ms   | 612.519 ms    | 924.156 ms    | 1694.044 ms   |
| Iteration 0: Rebuilding universe  | 264.264 ms   | 370.466 ms    | 699.359 ms    | 898.355 ms    |
| Iteration 0: Assigning keys       | 833.573 ms   | 924.627 ms    | 1403.807 ms   | 2608.101 ms   |
| Iteration 0: Setting up splitters | 3503.261 ms  | 3678.196 ms   | 4145.255 ms   | 4180.166 ms   |
| Iteration 0: Creating TreePieces  | 2060.153 ms  | 2424.105 ms   | 2623.145 ms   | 3637.131 ms   |
| Iteration 0: Flushing particles   | 820.147 ms   | 1035.441 ms   | 1323.536 ms   | 1549.522 ms   |
| Iteration 1: Tree build           | 4342.938 ms  | 6528.474 ms   | 11058.213 ms  | 25375.521 ms  |
| Iteration 1: Cache loading        | 217.893 ms   | 216.575 ms    | 214.630 ms    | 215.001 ms    |
| Iteration 1: Tree traversal       | 84016.559 ms | 114570.780 ms | 164862.955 ms | 295954.835 ms |
| Iteration 1: Interactions         | 6501.265 ms  | 8305.143 ms   | 12727.332 ms  | 24052.050 ms  |
| Iteration 1: Perturbations        | 465.722 ms   | 614.753 ms    | 863.530 ms    | 1546.247 ms   |
| Iteration 1: Rebuilding universe  | 273.582 ms   | 363.925 ms    | 632.232 ms    | 1055.919 ms   |
| Iteration 1: Assigning keys       | 783.637 ms   | 1129.716 ms   | 1548.566 ms   | 2693.940 ms   |
| Iteration 1: Setting up splitters | 3545.958 ms  | 3873.964 ms   | 3920.563 ms   | 3815.954 ms   |
| Iteration 1: Creating TreePieces  | 1261.987 ms  | 1262.613 ms   | 1765.087 ms   | 2930.149 ms   |
| Iteration 1: Flushing particles   | 796.986 ms   | 991.956 ms    | 1090.596 ms   | 1887.569 ms   |
| Iteration 2: Tree build           | 4335.968 ms  | 7109.698 ms   | 11396.585 ms  | 26039.367 ms  |
| Iteration 2: Cache loading        | 220.643 ms   | 219.632 ms    | 221.173 ms    | 207.259 ms    |
| Iteration 2: Tree traversal       | 96685.432 ms | 119465.247 ms | 165267.000 ms | 298924.181 ms |
| Iteration 2: Interactions         | 7496.802 ms  | 9784.366 ms   | 13786.165 ms  | 25618.673 ms  |
| Iteration 2: Perturbations        | 553.976 ms   | 643.021 ms    | 881.164 ms    | 1572.616 ms   |
| Iteration 2: Rebuilding universe  | 309.048 ms   | 385.426 ms    | 645.521 ms    | 1125.224 ms   |
| Iteration 2: Assigning keys       | 989.418 ms   | 1173.494 ms   | 1569.975 ms   | 2652.992 ms   |
| Iteration 2: Setting up splitters | 3450.453 ms  | 3669.275 ms   | 4028.519 ms   | 3634.326 ms   |
| Iteration 2: Creating TreePieces  | 1158.758 ms  | 1427.733 ms   | 1815.471 ms   | 3293.966 ms   |
| Iteration 2: Flushing particles   | 813.945 ms   | 938.869 ms    | 1157.823 ms   | 1629.236 ms   |
|-----------------------------------|--------------|---------------|---------------|---------------|
| Total runtime                     | 341334.21 ms | 430952.89 ms  | 610889.50 ms  | 1087422.3 ms  |


### jobscript-1

4 KNL stampede2 nodes, SMP mode, 68 processors, 3ppn (204 PEs):

| Stage                             | TRAM + batch resumes | TRAM         | batch resumes |
|-----------------------------------|----------------------|--------------|---------------|
| Initialization                    | 10297.789 ms         | 11043.095ms  | 11560.01ms    |
| Iteration 0: Tree build           | 2153.558 ms          | 1874.245 ms  | 1854.999 ms   |
| Iteration 0: Cache loading        | 222.892 ms           | 217.015 ms   | 214.341 ms    |
| Iteration 0: Tree traversal       | 36964.525 ms         | 42659.156 ms | 37824.924 ms  |
| Iteration 0: Interactions         | 2199.055 ms          | 2184.553 ms  | 2200.725 ms   |
| Iteration 0: Perturbations        | 218.550 ms           | 203.900 ms   | 202.359 ms    |
| Iteration 0: Rebuilding universe  | 73.208 ms            | 67.904 ms    | 72.470 ms     |
| Iteration 0: Assigning keys       | 322.485 ms           | 321.762 ms   | 321.116 ms    |
| Iteration 0: Setting up splitters | 2597.609 ms          | 2481.707 ms  | 2559.911 ms   |
| Iteration 0: Creating TreePieces  | 3968.616 ms          | 4077.139 ms  | 4302.249 ms   |
| Iteration 0: Flushing particles   | 541.872 ms           | 499.473 ms   | 519.540 ms    |
| Iteration 1: Tree build           | 1543.829 ms          | 2233.940 ms  | 1542.314 ms   |
| Iteration 1: Cache loading        | 220.994 ms           | 317.255 ms   | 227.663 ms    |
| Iteration 1: Tree traversal       | 38411.235 ms         | 46877.380 ms | 37423.335 ms  |
| Iteration 1: Interactions         | 2203.075 ms          | 2270.751 ms  | 2342.935 ms   |
| Iteration 1: Perturbations        | 180.752 ms           | 435.361 ms   | 206.735 ms    |
| Iteration 1: Rebuilding universe  | 92.497 ms            | 91.162 ms    | 91.410 ms     |
| Iteration 1: Assigning keys       | 272.794 ms           | 337.235 ms   | 317.240 ms    |
| Iteration 1: Setting up splitters | 2514.269 ms          | 3015.943 ms  | 2451.563 ms   |
| Iteration 1: Creating TreePieces  | 430.148 ms           | 439.973 ms   | 454.669 ms    |
| Iteration 1: Flushing particles   | 524.602 ms           | 513.776 ms   | 533.648 ms    |
| Iteration 2: Tree build           | 1576.079 ms          | 2281.130 ms  | 1673.560 ms   |
| Iteration 2: Cache loading        | 228.009 ms           | 311.953 ms   | 226.565 ms    |
| Iteration 2: Tree traversal       | 34400.195 ms         | 46446.800 ms | 35782.659 ms  |
| Iteration 2: Interactions         | 2693.615 ms          | 2701.589 ms  | 3265.248 ms   |
| Iteration 2: Perturbations        | 213.881 ms           | 499.618 ms   | 211.047 ms    |
| Iteration 2: Rebuilding universe  | 92.863 ms            | 102.177 ms   | 100.768 ms    |
| Iteration 2: Assigning keys       | 261.164 ms           | 343.633 ms   | 342.070 ms    |
| Iteration 2: Setting up splitters | 2436.313 ms          | 2927.513 ms  | 2360.388 ms   |
| Iteration 2: Creating TreePieces  | 461.337 ms           | 432.484 ms   | 450.603 ms    |
| Iteration 2: Flushing particles   | 522.155 ms           | 522.811 ms   | 538.103 ms    |
|-----------------------------------|----------------------|--------------|---------------|
| Total runtime                     | 148839.97 ms         | 178732.43 ms | 152175.17 ms  |
