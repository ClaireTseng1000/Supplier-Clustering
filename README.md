# Supplier Optimization
## Overview
This project applies **clustering** and **linear programming** techniques to analyze supplier performance and optimize supply allocation.
- Identify distinct supplier groups through K-means clustering
- Explore relationships between supplier clusters and characteristics
- Develop a cost-minimization supply plan through linear programming
**Part 1:** Cluster suppliers based on quality, cost, delivery time, and flexibility.
**Part 2:** Use linear programming to minimize transportation and manufacturing costs while satisfying customer demand.

## Part 1 – Supplier Clustering

### Goal
Group suppliers based on performance to uncover meaningful patterns.

### Cluster Interpretations
**cluster 1**: high quality, high cost, fast delivery, low flexibility
**cluster 2**: low quality, low cost, slow delivery, high flexibility
**cluster 3**: high quality, low cost, slow delivery, low flexibility
**cluster 4**: average quality, slightly high cost, fast delivery, high flexibility

## Part 2 – Linear Programming Optimization

### Goal
Minimize total cost while fulfilling customer demand across multiple nodes in a supply chain.


![Supply Chain Network]("E:\BADM 575\Supply Chain Network.png")
### Transportation Cost Table
| From → To         | W1      | W2      | R1      | R2      | R3      |
|------------------|---------|---------|---------|---------|---------|
| **Supplier 1**   | 150     | 200     | 325     | 260     | 390     |
| **Supplier 2**   | 400     | 350     | 585     | 650     | 520     |
| **Warehouse 1**  |         |         | 65      | 65      | 65      |
| **Warehouse 2**  |         |         | 97.5    | 32.5    | 32.5    |

### Results
- **Minimum Total Cost**: \$9,967,500
- **Optimal Plan**: All shipments are fulfilled directly from Supplier S2 to the retailers.
- **Insight**: Warehouses were unused in the optimal plan, indicating that direct shipping was more cost-efficient.

