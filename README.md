# HyperMinSketch

A simple implementation of HyperLogLog (LogLog-Beta to be specific) that allows intersections. This is done by increasing the size of the register by 16 bits (will reduce to 10) for a "fingerprint" based on b-Bit Minwise Hashing". 

The work is based on ["HyperMinHash: Jaccard index sketching in LogLog space - Yun William Yu, Griffin M. Weber"](https://arxiv.org/pdf/1710.08436.pdf)

# Results

Intersecting 2 HyperLogLogs

| HLL1 | HLL2 | Exact Intersection | Estimated Intersection |
| [0 - 1000000]  | [50000 - 1950000]| 950000 | 952282 |
| [0 - 1000000]  | [100000 - 1900000]| 900000 | 897511 |
| [0 - 1000000]  | [150000 - 1850000]| 850000 | 848583 |
| [0 - 1000000]  | [200000 - 1800000]| 800000 | 799654 |
| [0 - 1000000]  | [250000 - 1750000]| 750000 | 750482 |
| [0 - 1000000]  | [300000 - 1700000]| 700000 | 704231 |
| [0 - 1000000]  | [350000 - 1650000]| 650000 | 653112 |
| [0 - 1000000]  | [400000 - 1600000]| 600000 | 599558 |
| [0 - 1000000]  | [450000 - 1550000]| 550000 | 549777 |
| [0 - 1000000]  | [500000 - 1500000]| 500000 | 498171 |
| [0 - 1000000]  | [550000 - 1450000]| 450000 | 452529 |
| [0 - 1000000]  | [600000 - 1400000]| 400000 | 404087 |
| [0 - 1000000]  | [650000 - 1350000]| 350000 | 358688 |
| [0 - 1000000]  | [700000 - 1300000]| 300000 | 306473 |
| [0 - 1000000]  | [750000 - 1250000]| 250000 | 251946 |
| [0 - 1000000]  | [800000 - 1200000]| 200000 | 201678 |
| [0 - 1000000]  | [850000 - 1150000]| 150000 | 151776 |
| [0 - 1000000]  | [900000 - 1100000]| 100000 | 103699 |
| [0 - 1000000]  | [950000 - 1050000]| 50000 | 52215 |
| [0 - 1000000]  | [1000000 - 1000000]| 0 | 0 |