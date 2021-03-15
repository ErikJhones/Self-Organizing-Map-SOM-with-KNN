# FUZZY to classifie hotspot
Classification of hotspot in photovoltaic module using fuzzy logic.

## Dataset

![Alt text](./images/fuzzy-datas.png?raw=true "Title")

This is a dataset supervised. The dataset has 600 samples of module with hotspot, where is splited in 6 classes. Each sample has 3 features: Ppl: The percentage of power less; Voc: the percentagem of voltage less; and Isc: the percentage of current less.

## Model FUZZY
![Alt text](./images/fuzzy-universe1.png?raw=true "Title")

Universe of discourse of the Voc feature. The 'L' means 'LOWER', and mean a lower less of voltage at modules. Respectively, 'M' is 'Mean' and 'H' is 'HIGH'.

![Alt text](./images/fuzzy-universe2.png?raw=true "Title")

This image is for Isc feature.

![Alt text](./images/fuzzy-universe3.png?raw=true "Title")

This is the consequence of FUZZY. It means if Voc and Isc were L, so the module has a L OMF, thus it got 1 or 2 hotspots.

## Results
This FUZZY was used to classifie hotspot fault, so the result is show in the image below.

![Alt text](./images/fuzzy-result1.png?raw=true "Title")

![Alt text](./images/fuzzy-result2.png?raw=true "Title")

Can be seen in the figures that the FUZZY was better to classifie the class 1 and 2, but for class 3 and 4 this dont happens. 

**The accuracy was 79%**.

# Self-Organizing-Map-SOM-with-KNN
A SOM network build to classify one photovoltaic failure dataset 

## DETAILS FOR LIBRARIES INSTALL (ubuntu)
1. Create a virtual env: virtualenv -p python3 .env
2. enter in your terminal venv: source .env/bin/activate
3. install the libraries: pip install requirements.txt 

## The model
Map: 100x100  
neighboor: 3  
learn rate: 0.5  
weighs: random from dataset  
epoch: 1000  

## DATASET DETAILS 
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


## RESULTS
with a 100x100 nodes matrix (just 10000 instead of 500.00 samples), was obtained a F1-score higher than 91%.  
![Alt text](./images/wdataset.png?raw=true "Title")

comparation with W choised randomly, where the KNN got just 41%.  
![Alt text](./images/wramdon.png?raw=true "Title")

Anf for all dataset, the result was 96% acc.  
![Alt text](./images/allds.png?raw=true "Title")

## graph comparative som output vs real output
![Alt text](./images/somVSreal.png?raw=true "Title")

# MLP FOR SHADOW FAULT CLASSIFICATION IN PHOTOVOLTAIC MODULE 

## Multi Layer Perceptron
Number layers: 4  
Neurons per layers: 128, 100, 100, 64  
solver: adam  
activation: tanh  
epoch: 100  

## Results
### For all dataset
![Alt text](./images/mlp-result1.png?raw=true "Title")

### For SOM dataset
![Alt text](./images/mlp-result2.png?raw=true "Title")

https://colab.research.google.com/drive/1E5u5mEaI7d9idc7lDHqyg0oeVx2t0YHi#scrollTo=nRMZvdTxrT5g
