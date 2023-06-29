![license
status](https://img.shields.io/github/license/johnwslee/injection_molding_analysis)

# Classification of Defective Parts in Injection Molding Using Various Modeling Approaches

**Author:** John W.S. Lee

## 1. Introduction

In this study, efforts were made to classify the defects from the parts produced by injection molding processes. 3 different modeling approaches (i.e. supervised learning models, Mahalanobis Distance model, and Variational AutoEncoder Model) were implemented and their performances were compared.

The dataset used in this study was downloaded from the Korea AI Manufacturing Platform, also known as [KAMP](https://www.kamp-ai.kr/aidataDetail?AI_SEARCH=&page=1&DATASET_SEQ=4&EQUIP_SEL=&GUBUN_SEL=&FILE_TYPE_SEL=&WDATE_SEL=). The website is written in Korean, however, the contents of the dataset were mostly written in English. The dataset contained 7,996 rows with 44 columns. One of the columns was the label for the target, `PassOrFail`.

The followings are the summary of this study, while more detailed codes and notebooks used for this study can be found in [notebook folder](https://github.com/johnwslee/injection_molding_analysis/tree/main/notebooks).

## 2. Summary of Study

### 2.1. Basic Exploratory Data Analysis

The dataset had 4 different injection-molded parts, namely `CN7` and `RG3`, each with Left-Hand and Right-Hand components. The figure below shows the distribution of processing parameters for the parts with 4 different combinations. As shown in the figure, the processing parameters for `CN7` and `RG3` exhibited very different distribution, whereas the difference between the Left-Hand and Right-Hand components were not big. Therefore, it was reasonable to proceed with two separate models for `CN7` and `RG3`.

<img src="https://github.com/johnwslee/injection_molding_analysis/blob/main/img/process_parameter_distribution.png" style="width:800px;height:700px;background-color:white">

### 2.2. Exploratory Data Analysis for `CN7` and `RG3`

For each type of injection-molded parts, the distributions of the processing parameters were compared for passed parts(i.e. good parts) and failed parts (i.e. defective parts). In the case of `CN7`, there seemed to be some difference in the distributions of the processing parameters for passed/failed parts . However, the difference for `RG3` seems to be less obvious than that for `CN7`.

#### Distribution of Processing Parameters for `CN7`

<img src="https://github.com/johnwslee/injection_molding_analysis/blob/main/img/cn7_parameter_distribution.png" style="width:800px;height:2400px;background-color:white">

#### Distribution of Processing Parameters for `RG3`

<img src="https://github.com/johnwslee/injection_molding_analysis/blob/main/img/rg3_parameter_distribution.png" style="width:800px;height:2400px;background-color:white">

### 2.3. Classification of Defective Parts for `CN7`





### 2.4. Classification of Defective Parts for `RG3`






### 2.5. Feature Importances





## 3. Conclusion



## How to Run the Notebooks Locally

To download the contents of this GitHub page on to your local machine, follow these steps:

1. Copy and paste the following link: `git clone https://github.com/johnwslee/injection_molding_analysis.git` to your Terminal.

2. On your terminal, type: `cd injection_molding_analysis`.

3. Create a virtualenv by typing: `conda env create -f env.yml`

4. Activate the virtualenv by typing: `conda activate inj_env`

5. Run the notebooks in notebook folder in order.