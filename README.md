# Predicting-Energy-Loads-of-Buildings

The basic principle of building energy efficiency is to use less energy for operations including heating, cooling, lighting and other appliances, without affecting the health and comfort of its occupants. 
Improving the energy efficiency of functional buildings brings many environmental and economic benefits such as reduced greenhouse gas emissions and operational cost savings.

## Overview

Given various building features (8 variables), goal is to predict heating load and cooling load. This is a multi-target regression problem, a Multi Layer Perceptron (MLP) layer with two output nodes can solve this problem. 
Tried with various MLP architectures and many hyper parameters and find best hyper parameters to reduce R^2.
Performed exploratory data analysis and find insights of the data.

## Description

<ul>
  <li>A modular geometry system was derived based on an elementary cube (3.5 × 3.5 × 3.5m). In order to generate different building shapes, eighteen such elements were used according to Figure</li>


<p><img src="dataset.png" width="300" height="300" /> </p>

  <li> Then generated 12 structures with different shapes and Relative Compactness as shown in figure.</li>

<p><img src="dataset1.png" width="300" height="300" /> </p>
  <li>
    <ul>
      <li> X1 - Relative Compactness </li>
      <li> X2 - Surface Area</li>
      <li> X3 - Wall Area  </li>
      <li> X4 - Roof Area </li>
      <li> X5 - Overall Height </li>
      <li> X6 - Orientation </li>
      <li> X7 - Glazing Area  </li>
      <li> X8 - Glazing Area Distribution </li>
    </ul>
  </li>

<br>  Each feature is described in the figure:
  
<p><img src="dataset3.png" width="300" height="300" /> </p>
  
</ul>

### Dataset
The raw data contains 768 rows each row represent a structure of the building. 8 Input Variables. Heating Load and Cooling load are our output variables.
<br>
<p>Dataset reference: https://people.maths.ox.ac.uk/tsanas/Preprints/ENB2012.pdf <p>

### Splitting Dataset
Since the dataset is a bit small to tain a MLP, splitted dataset into 5 fold CV. Where 4 folds are for training and one fold for testing. <br>
Detailed explaination of 5 fold CV shown in image:
<p><img src="5folcv.png" width="300" height="300" /> </p>

