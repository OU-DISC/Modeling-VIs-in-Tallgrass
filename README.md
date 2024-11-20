# Modeling-VIs-in-Tallgrass

This project investigates the feasability of several machine learning and deep learning techniques for modeling Vegetation Indices (VIs) in Tallgrass prairies using readily available weather attributes. The goal is to develop predictive models that can accurately estimate the remote sensing VIs such as MODIS-EVI and LSWI.

## Documentation
The code is written using python notebooks and completely implemented using Google Colab Workspace.

## Contents
- data: contains both raw and processed datasets.
- models: contains pretrained models for easily loading results without training step.
- src: contains notebooks for data preparation and modeling of both VIs (EVI and LSWI) broken down into three stages.
    - src/data preparation.ipynb: Load invididual data sources from weathe and remote sensing data, perform preprocessing, save processed clean data.
    - src/**_train_models1.ipnb: Train and save six initial models (linear regression, XGBoost, random forest, decision tree, SVR, KNN).
    - src/**_train_models2.ipnb: Train and save six additional models (bayesian ridge, elastic net, ANN, CNN, RNN, LSTM).
    - src/**_final_eval_plots.ipnb: Load pre-trained models, perform train/test/val, plot and save results.
    - src/**_train_models2_eval.ipynb: Additional train/test/val analysis.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## How to Run
- Clone directly in Google Colab 
(or)
- Clone locally, adjust file paths, install dependencies.