# VR user identification
==============================

Code for the paper "Movement- and Traffic-based User Identification in Commercial Virtual Reality Applications: Threats and Opportunities," by S. Baldoni, S. Benhamadi, F. Chiariotti, F. Battisti, and M. Zorzi, to be presented at IEEE VR 2025.

## Project Organization
------------
```
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
└── 

```
--------

## Running the Project

To generate statistical features from the VR raw data, including movement and traffic data, execute the following command. This process will compute various statistical measures such as minimum (min), maximum (max), standard deviation (std), 25th percentile, 50th percentile, 75th percentile, and mean.

```python
python ./src/features/build_features.py ./data/raw/Raw_traffic_and_movement_data/ ./data/processed/ 1
```

