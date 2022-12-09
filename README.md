# Introduction
In order to texture a 3d model, a common practice is to map the 3d shape onto a 2D surface and add the texture to the surface, which is known as parametrization. There are many algorithms in this field with a large number of classical techniques. 

In our project, we have implemented the Least Squares Conformal Maps(lscm) algorithm, mainly based on conformal maps to preserve the information for the original 3d shape. Our work is mainly based on the article \emph{Least Squares Conformal Maps
for Automatic Texture Atlas Generation} (Lévy B et al.).

# Data
Several meshes saved folder meshes are utilised in the project. Most of them are downloaded from Internet. 


# Loading
There are several npy files containing pretrained lists of features edges. You can either apply the feature extraction algorithm or load the corresponding files.  
```python
feature_rabbit,feature_neighbor_rabbit=read_features(mesh_rabbit,features_rabbit,neighbors_rabbit)
```


# Environment:
In the project, sevral modules are used. Their requirements are listed as follow:
* numpy==1.23.1
* pandas==1.5.1
* scipy==1.9.3
* pywavefront==1.3.3
* openmesh==1.2.1
* rectangle-packing-solver==0.0.5
* rectpack==0.2.2
* matplotlib==3.5.2
* matplotlib-inline==0.1.6

The environment is also saved in the environment.yaml, which can be directly imported by using anaconda.

# How to run the file 
There are two jupyter notebooks, different meshes are applied in each of them

new.ipynb: Algorithm applied on the rabbit mesh

fish.ipynb: Algorithm applied on the fish mesh

You can simply run the notebooks from top to bottom. For the feature extraction, you cai either train a model on your own or load the existing results as said above.

You can also find the projet on github: https://github.com/xiajunkai328/inf574 where the files all already placed in the right places. 