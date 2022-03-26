## Goal of the project
The goal of this project is to classify according to 3 classes : 
1) Galaxies
2) Quasars
3) Stars

Based on several physical characteristics reported. The dataset used contains 100 thousand samples of classes that are unbalanced and distributed as follows: 
| Class | Number of elements |
|---    |:-:    |
|  Galaxies     |  59445 | 
|  Quasars  |   18961    |   
|  Stars   |   21594  | 
|  TOTAL   |   100000  | 
## Software requirements 
To use this code you will need : 
- Python 3.8 or higher
- Scikit-learn
- Pandas
- Matplotlib
- Numpy
- Seaborn
## Content of the project
This project has 3 parts 
1) **Analysis and visualization of the data:** During this step we analyze globally the variables and their distributions in order to extract the variables of interest and which could efficiently help the classification
2) **Pre-processing of the data:** During this step we prepare the data for the classification, and therefore we remove the columns that we consider useless or not very interesting for the classification and in our case it was : 
    - Rerun ID
    - U
    - G 
    - Z
which were removed. And then a normalization step was done on the data to put them on the same range of values. 
3) **Classification:** During this step we use several classification algorithms allowing us to solve the given problem
## Performance achieved 
### Without data normalization
| Algorithms (%) | Accuracy (%) | F1 score (%) |
|---    |:-:    |:-:    |
|   KNN     |  70.94  |   61.31   |
|   Random Forest   |   97.41   |    96.89   |
|   Extremely randomized tree   |   96.49  |  95.91   |
### With data normalization
| Algorithms (%) | Accuracy (%) | F1 score (%) |
|---    |:-:    |:-:    |
|   KNN     |  90.25  |   88.63   |
|   Random Forest   |   97.41   |    96.95   |
|   Extremely randomized tree   |   96.51  |  95.93   |