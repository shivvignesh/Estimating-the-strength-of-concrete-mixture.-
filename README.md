# Concrete Compressive Strength.

Compressive strength or compression strength is the capacity of a material or structure to withstand loads tending to reduce size, as opposed to tensile strength, which withstands loads tending to elongate.

Compressive strength is one of the most important engineering properties of concrete. It is a standard industrial practice that the concrete is classified based on grades. This grade is nothing but the Compressive Strength of the concrete cube or cylinder. Cube or Cylinder samples are usually tested under a compression testing machine to obtain the compressive strength of concrete. The test requisites differ country to country based on the design code.

## Install
This project requires python 3.6 or anyother higher versions of python, along with these libraries :

* NumPy
* Pandas
* matplotlib
* scikit-learn


You also need a software to run this python notebook "Jupyter Notebook".
It is highly recommended that you install the Anaconda distribution of Python, which already has the above packages and moreincluded.

## Description of the repository 

This repository contains 5 notebooks 
1. compressive strength of concrete.ipynb : This notebook contains univariate linear regression implementation of the dataset.  

2. compressive strength 2 features.ipynb :  Multivariate Linear Regression implementation using two features. 

In the above two notebooks features selection was performed using Pearson correlation. The features with highest correlation values were selected. 

3. Compressive Strength using Sklearn.ipynb : Scikit-learn implementation of the dataset using a single feature.Correlation is misleading and not the accurate way of features selection. Features were selected on the basis of knowledge on the dataset, how one feature can affect the overall outcome/target. 

4. Compressive Strength using Sklearn-All features.ipynb : Scikit-learn implementation using all the input variables.

5. NN for Regression-concrete : Neural Networks implementation. 
As the root mean squared error in the above implementations were high, Neural Networks produced a 
much more acceptable error.

## Attribute information

* Cement (component 1) -- quantitative, kg in a m3 mixture :
  The quantity of cement added to the concrete mixture. Cement forms the main ingredient in concrete mixture.

* Blast Furnace Slag (component 2) -- quantitative -- kg in a m3 mixture :
  Blast Furnace Slag is the residue iron mixture component added to increase the strength of the concrete mixture.

* Fly Ash (component 3) -- quantitative -- kg in a m3 mixture :
  Fly Ash is a carbon product(coal)	added to reduce the amount of Cement in the mixture, it increases the workability,strength and durability of the concrete mixture. 

* Water (component 4) -- quantitative -- kg in a m3 mixture  :
  Water component is self descriptive, water is added to mixture which transform into a gel like substance, usually seen in construction work. This substance on drying or exposure to heat yields a solid rock like product.

* Superplasticizer (component 5) -- quantitative -- kg in a m3 mixture :
   Superplasticizer component removes any excess water molecules present in the mixture, excess water in the concrete leads to cracks,breaks and voids inside concrete. 

* Coarse Aggregate (component 6) -- quantitative -- kg in a m3 mixture :
  
* Fine Aggregate (component 7) -- quantitative -- kg in a m3 mixture 
  
  Coarse Aggregate are stones whose sizes is greater than 4.75mm . Fine Aggregate are natural sand or crushed stones whose size is less than 4.75mm.   

* Age -- quantitative -- Day (1~365) :
 The amount of time taken to harden the mixture into concrete. The strength of the concrete  increases as more number of days pass by.
 
## Output Variable (desired Target):
 * Concrete compressive strength -- quantitative -- MPa : Compressive Strength is the maximum amount of load or pressure at which the concrete would break. 

## Models Trained on:
 Training Model | Root Mean Squared error
 ---------------|--------------------------
 Univariate Linear Regression | 0.13738
 Multivariate two features | 0.17730
 Linear Regression using Sklearn | 0.13093
 Neural Networks | 0.073981

## Error graph : 
![Error vs iterations](download(1).png)

