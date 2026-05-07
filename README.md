# Generalized Boundary FDR Control under Arbitrary Dependence: An Approach on Closure Principle
This repository implements Domino methods proposed in our paper: Generalized Boundary FDR Control under Arbitrary Dependence: An Approach on Closure Principle
## Repository Structure

```text
.
├── functions/
│   └── utils.py             # Contains all utility functions used in the project
│
├── simulation/
│   └── simulation.py        # Code for simulation experiments (Section 5.1)
│
├── RealData/
│   ├── CEGv2.txt            # True positive labels used in genedata.py
│   ├── NEGv1.txt            # True negative labels used in genedata.py
│   ├── datasource.txt       # The source of the three real data experiments
│   ├── genedata.py          # Real data analysis for gene expression (Section 5.2)
│   ├── stockdata.py         # Real data analysis for stock market (Section 5.3)
│   └── enrichment.py        # Real data experiment for the Appendix
│
├── README.md
│
└── LICENSE                  # MIT License
```

## 🚀 Usage

### 1. Functions (Core Utilities)

The `functions/utils.py` script serves as the backbone of the project, containing all core algorithms and utility functions. Key components include:

- **Domino Implementations:** Functions executing the Domino framework across different types of local tests.
- **Evaluation Metrics:** Functions designed to evaluate the performance and validity of the final rejection sets.
- **Data Helpers:** Additional utility functions required for data preprocessing and supporting the real data analyses.

### 2. Simulation

The simulation experiments from Section 5.1 of the paper are orchestrated in the `simulation/simulation.py` script. It primarily evaluates the performance of different methods as the target alpha level varies.

To run the main simulation:

```bash
python simulation/simulation.py
```

### 3. Real Data Analysis
The `RealData/` directory contains scripts to reproduce the three real-world applications discussed in the paper (Sections 5.2 & 5.3) and the appendix.

- **`genedata.py`**: Reproduces the gene expression analysis (Section 5.2). This script utilizes the true positive and true negative labels provided in `CEGv2.txt` and `NEGv1.txt`, respectively.
- **`stockdata.py`**: Reproduces the stock market data analysis (Section 5.3).
- **`enrichment.py`**: Executes the supplementary real data experiment detailed in the appendix.

**Data Source:** Detailed information regarding the origins and acquisition of the raw datasets for these three experiments can be found in `RealData/datasource.txt`.

## 📖 References

* **Paper**: [Generalized Boundary FDR Control under Arbitrary Dependence: An Approach on Closure Principle] (pdf available soon)
* **Supplementary**: See algorithms described in `utiles/` for technical details.

## 📝 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
