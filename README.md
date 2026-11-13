# DL-Onboarding-Project
2026 Onboarding Project for the Deep Learning team (UTAT)

# Usage
Clone entire repo before running any notebooks. Ensure `simpler_data_rwc.csv` exists in a directory labelled `datasets` (one level above `src`). 
## Plotting Data
To plot hyperspectral data, run `plotting.ipynb`. 
## Constructing models
To construct an unmixer, you may run `model1.ipynb` to build a model according to initial specifications (as specified by onboarding instructions). <br><br>
To construct an unmixer with modified architecture, run `model2.ipynb`. Change the `model_name` string at the top of the file and edit the architecture at your discretion (e.g. hidden layer width, count, activation function, etc.)
## Testing models
In either `model1.ipynb` or `model2.ipynb`, a second code block exists for testing. Running it will output a graph and R^2 scores for the model.
## Results
During training and testing, R^2 scores are obtained and outputted as .csv's. During training, this goes into `validation-data`, while testing scores go into `testing-data`. Validation score csv's contain data on each epoch of training, organized in the format [GV R^2, NPV R^2, Soil R^2]. Testing data contains the final GV, NPV, and soil R^2 after testing, as well as an average of the three endmembers.
