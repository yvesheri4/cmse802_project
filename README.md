Project Title: Application of Machine Learning in Accelerator Physics
===============================

This repository implements machine learning techniques, including non-linear regression and Physics-Informed Neural Networks (PINNs), to solve the inverse problem of the Kapchinsky-Vladimirsky (KV) equation. It includes data preprocessing, model code, Jupyter notebooks, and results, supporting reproducibility in computational research. Here is the repository directory structure tailored for this project:

```
cmse802_project
│
├── data                        # Contains datasets
│   ├── raw                     # Raw, unprocessed data files
│   └── processed               # Preprocessed and cleaned data
│
├── notebooks                   # Jupyter notebooks for analysis and experiments
│   ├── 01_data_generation.ipynb        # Initial data exploration
│   ├── 02_data_exploration.ipynb       # 
│   ├── 03_LSTM_forward_problem.ipynb   # LSTM for forward problem
│
├── src                           # Source code directory
│   ├── __init__.py               # Initialization for the Python module
│   ├── data_preprocessing.py     # Scripts for data cleaning and preprocessing
│   ├── LSTM_model.py             # Model implementation
│   └── utils.py                  # Utility functions
│
├── scripts                     # Helper scripts and commands
│   └── run_training.sh         # Script to train the model
│
├── tests                       # Unit and integration tests for the codebase
│   └── test_LSTM_model.py      # Example test for the PINN implementation
│
├── results                     # Directory for output results
│   ├── figures                 # Generated plots and figures
│   └── logs                    # Logs and performance metrics
│
├── requirements.txt            # Python dependencies
├── README.md                   # Project description, setup instructions, and usage
├── LICENSE                     # Project license
└── .gitignore                  # Files to be ignored in the GitHub repository
```

Description
------

We are working on solving the inverse problem of the Kapchinsky-Vladimirsky (KV) envelope equation in accelerator physics expressed as

$$
r_x'' + kr_x - \frac{2K}{(r_x+r_y)}-\epsilon_x^2/r_x^3= 0 
$$

$$
r_y'' - kr_y - \frac{2K}{(r_x+r_y)}-\epsilon_y^2/r_y^3= 0 
$$

Where $r_x$ and $r_y$ are the horizontal and vertical beam envelope radii as functions of the position  $𝑠$ along the beamline. $\epsilon_x$ and $\epsilon_y$ are the horizontal and vertical emittances, representing the beam's spread in phase space. The parameter $k$ is the external focusing strength (e.g., from magnetic lenses). And last parameter $K$  accounts for the space charge effect, which causes beam expansion due to the repulsive forces between charged particles. In this project, we intend on using: Machine learning, Physics-Informed Neural Networks (PINNs), Non-linear regression. The goal is to infer parameters or conditions of the KV equation from observed or simulated data.

Objectives
---------
In this project we aim specifically to:

1. Write down the KV equations and formalize the inverse problem mathematically. Review the physics of the KV equation and beam dynamics.

2. Simulate data using accelerator simulation tools. Ensure the data is preprocessed and ready for machine learning (clean, normalized, structured).

3. Set up a Git repository for version control.

4. Develop a small-scale prototype of a PINN using TensorFlow or PyTorch. Start with a forward problem, then adapt to the inverse problem by embedding the KV equation into the loss function.

5. Physics-based metrics, such as how well the model satisfies the KV envelope equation.
...

