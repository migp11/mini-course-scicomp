# Scientific Computing Mini-Course: Complex Systems & Large-Scale Data Analysis

A comprehensive mini-course on scientific computing with a focus on understanding complex systems and processing large-scale datasets. This course combines theoretical foundations with practical hands-on programming using Python, covering everything from N-dimensional arrays to parallel computing workflows.

## 📚 Course Overview

This course explores how to model, simulate, and analyze complex systems through the lens of computational science. Topics include:

- **Complex Systems Theory**: Understanding systems with many interacting components (epidemiology, tumor dynamics, urban mobility)
- **N-Dimensional Arrays**: Efficient data structures for scientific computing with NumPy and xarray
- **Large-Scale Data Processing**: Handling massive datasets with memory-efficient techniques
- **Workflow Automation**: EMEWS (Extreme-scale Model Exploration With Sweeps) for large parameter studies
- **Data Analysis & Visualization**: Practical tools for exploratory data analysis

**Instructor**: Miguel Ponce de Leon (miguel.ponce@bsc.es) - Barcelona Supercomputing Center  
**Date**: May 5, 2026

## 📁 Repository Structure

```
mini-course-scicomp/
├── lectures/                    # Lecture materials (reveal.js presentations)
│   ├── L01_intro.qmd           # Course motivation and complex systems overview
│   ├── L02_nd_arrays.qmd       # N-dimensional arrays and scientific computing
│   ├── L03_massive_data.qmd    # Large-scale data processing techniques
│   ├── L05_emews.qmd           # EMEWS workflow automation framework
│   ├── flowmaps_intro.qmd      # Mobility and flow data visualization
│   ├── day1_setup.qmd          # Environment setup and installation
│   ├── css/                    # Custom presentation styles
│   └── img/                    # Course images and diagrams
│
├── practical/                   # Hands-on Jupyter notebooks
│   ├── 00_pandas_basics.ipynb             # Pandas fundamentals
│   ├── 00_plot_basisc.ipynb               # Basic plotting with matplotlib
│   ├── 01_dataframes.ipynb                # Working with DataFrames
│   ├── 02_xarray_in_45_min.ipynb          # Quick introduction to xarray
│   ├── 03_xarray_flowmaps.ipynb           # Practical xarray with real data
│   ├── process_zones.ipynb                # Geographic data processing
│   ├── data/                              # Sample datasets
│   │   ├── covid19/                       # COVID-19 epidemiology data
│   │   ├── extra/                         # Shapefile and district data
│   │   ├── mitma_v1/                      # MITMA mobility data
│   │   └── processed/                     # Processed dataset outputs
│   ├── img/                               # Notebook visualizations
│   └── solutions/                         # Solution notebooks for exercises
│
├── docs/                        # Generated website (output of Quarto build)
├── _quarto.yml                 # Quarto configuration
├── README.md                   # This file
├── references.md               # Course references and bibliography
└── LICENSE                     # CC0 1.0 Universal (Public Domain)
```

## 🎯 Lecture Contents

| Lecture | Topic | Key Concepts |
|---------|-------|--------------|
| **Day 1 Setup** | Environment configuration | Installation, virtual environments, dependencies |
| **L01** | Complex Systems Introduction | Motivation, complex systems definition, real-world examples |
| **L02** | N-Dimensional Arrays | NumPy, xarray, scientific data structures |
| **L03** | Massive Data Processing | Memory-efficient techniques, out-of-core computing |
| **L05** | EMEWS Framework | Workflow automation, parameter sweeps, HPC |
| **Flowmaps** | Mobility Data Visualization | Geographic flows, mobility patterns, visualization techniques |

## 🛠️ Getting Started

### Prerequisites

- Python 3.8+
- Git
- A code editor (VS Code, Jupyter, etc.)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/mini-course-scicomp.git
   cd mini-course-scicomp
   ```

2. **Create a virtual environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
   
   Key packages include:
   - `numpy` - Numerical computing
   - `pandas` - Data manipulation
   - `xarray` - N-dimensional labeled arrays
   - `matplotlib` - Plotting and visualization
   - `jupyter` - Interactive notebooks
   - `quarto` - Document generation (for building presentations)

### Viewing Materials

**Online**: Access the built course website at the GitHub Pages deployment (if enabled)

**Locally - View Lectures**:
```bash
quarto preview lectures/
```

**Locally - Run Practical Notebooks**:
```bash
jupyter notebook practical/
```

**Build the website**:
```bash
quarto render
```

## 📖 Practical Notebooks Guide

The `practical/` folder contains Jupyter notebooks for hands-on learning:

- **`00_pandas_basics.ipynb`** - Start here for DataFrame fundamentals
- **`00_plot_basisc.ipynb`** - Basic visualization with matplotlib
- **`01_dataframes.ipynb`** - Intermediate pandas operations
- **`02_xarray_in_45_min.ipynb`** - Quick xarray introduction
- **`03_xarray_flowmaps.ipynb`** - Real-world example with mobility data
- **`process_zones.ipynb`** - Geographic data (shapefiles, geospatial analysis)

Each notebook includes exercises with solutions available in `practical/solutions/`.

## 📊 Sample Datasets

The course includes several real-world datasets:

- **COVID-19 Data** (`practical/data/covid19/`): Spanish provincial epidemiology data
- **Mobility Data** (`practical/data/mitma_v1/`): Spanish mobility patterns from MITMA
- **Geographic Data** (`practical/data/extra/`): District shapefiles and boundaries

## 🔗 References

For a complete bibliography and reference materials, see [references.md](references.md).

## 💡 How to Use This Repository

### For Students
1. Start with **`day1_setup.qmd`** for environment configuration
2. Watch/read lectures in order: L01 → L02 → L03 → L05
3. Complete corresponding practical notebooks after each lecture
4. Check `practical/solutions/` to compare your work

### For Instructors
- Modify lecture content in `lectures/*.qmd`
- Update data in `practical/data/` as needed
- Customize styles in `lectures/css/styles.css`
- Rebuild with `quarto render` after changes

## 📝 Course Workflow

```
Day 1: Setup & Introduction
  └─ day1_setup.qmd
  └─ L01_intro.qmd
  └─ practical: 00_pandas_basics.ipynb, 00_plot_basisc.ipynb

Day 2-3: Data Structures & Processing
  └─ L02_nd_arrays.qmd
  └─ L03_massive_data.qmd
  └─ practical: 01_dataframes.ipynb, 02_xarray_in_45_min.ipynb, 03_xarray_flowmaps.ipynb

Day 4: Advanced Topics
  └─ L05_emews.qmd
  └─ flowmaps_intro.qmd
  └─ practical: process_zones.ipynb
```

## 🤝 Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Submit a pull request with a clear description

For bug reports or suggestions, open an issue on GitHub.

## 📄 License

This project is released under the **CC0 1.0 Universal** license (Public Domain). You are free to:
- Use, modify, and distribute the materials
- Use them for commercial and private purposes
- No attribution is required

See [LICENSE](LICENSE) for full details.

## 🔗 External Resources

- [Quarto Documentation](https://quarto.org)
- [NumPy Guide](https://numpy.org/doc/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [xarray Documentation](https://docs.xarray.dev/)
- [EMEWS Project](https://emews.org)
- [Complex Systems Research at BSC](https://www.bsc.es/)

## 📧 Support

For questions or issues:
- Email: miguel.ponce@bsc.es
- Open an issue on GitHub
- Check the [references.md](references.md) for additional learning resources

---

**Last Updated**: May 5, 2026  
**Institution**: Barcelona Supercomputing Center (BSC)