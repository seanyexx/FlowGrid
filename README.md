# Ultrafast clustering of single-cell flow cytometry data using FlowGrid
    Authors: Xiaoxin Ye and Joshua W. K. Ho
    Contact: j.ho@victorchang.edu.au
    Copyright © 2018, Victor Chang Cardiac Research Institute
## Input data format
Our FlowGrid algorithm only csv format and each columns is seperated by `,`.

## Install
Before using the package, we need to install the dependent package sklearn and numpy.
``` python
sudo pip install -r requirements.txt
```
or
``` python
sudo pip install sklearn numpy
```
## Usage
A summary of the argument of sample code is included in the table below.
 

|argument | usage| Require |
| :----: | :----: | :----: |
|--f | the input file name| True|
|--n | number of bins | True |
|--eps | maximun distance between two bins| True |
|--t | threshold for high density bin| False(default:40) |
|--o | the output file name| False(default: out.csv) |
|--l | the true label file name| False|

## Sample
After installing the dependent packages, you could try to use the sample code to run FlowGrid on sample data.
``` bash
python sample_code.py --f sample_data.csv --n 4  --eps 1.1 --l sample_label.csv
```
The result is saved at out.csv.