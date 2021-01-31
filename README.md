# Self-Organizing-Map-SOM-with-KNN
A SOM network build to classify one photovoltaic failure dataset 

# DETAILS FOR LIBRARIES INSTALL (ubuntu)
1. Create a virtual env: virtualenv -p python3 .env
2. enter in your terminal venv: source .env/bin/activate
3. install the libraries: pip install requirements.txt 

# DATASET DETAILS 
![Alt text](./images/dataset.png?raw=true "Title")
Irr = irradiance
Icc = current
Vcc = Voltage
Tpm = temperature

Class = 

## DATASET VISUALIZATION
datas process with PCA and get just the 2 best samples. 
datas with yours respectives class by colors.
![Alt text](./images/pca.png?raw=true "Title")

Data plots with the 2 first samples (Irr Icc)
![Alt text](./images/real.png?raw=true "Title")


# RESULTS
with a 40x40 nodes matrix (just 1600 instead of 500.00 samples), was obtained a F1-score higher than 80%.
![Alt text](./images/wdataset.png?raw=true "Title")

comparation with W choised randomly, where the KNN got just 41%.
![Alt text](./images/wramdon.png?raw=true "Title")
