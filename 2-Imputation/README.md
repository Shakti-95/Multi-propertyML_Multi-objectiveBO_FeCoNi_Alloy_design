# Imputation

The strategy for imputation used in this work is as follows:
1. Best ML model mapping from *Compostion* to *M<sub>s</sub>* with lowest **MAE** is used to fill up the gaps in *M<sub>s</sub>* column (**Extra Trees**)
2. Best ML model mapping from *Compostion* to *log<sub>10</sub> H<sub>c</sub>* with lowest **MAE** is used to fill up the gaps in *log<sub>10</sub> H<sub>c</sub>* column (**Extra Trees**)
3. Best ML model mapping from *Compostion* to *log<sub>10</sub> T<sub>c</sub>* with lowest **MAE** is used to fill up the gaps in *log<sub>10</sub> T<sub>c</sub>* column (**Extra Trees**)
4. Best ML model mapping from *Compostion* to *log<sub>10</sub> ρ* with lowest **MAE** is used to fill up the gaps in *log<sub>10</sub> ρ* column (**Extra Trees**)
5. Best ML model mapping from *Compostion* to *log<sub>10</sub> δ* with lowest **MAE** is used to fill up the gaps in *log<sub>10</sub> δ* column (**Decision Tree**)
6. Best ML model mapping from *log<sub>10</sub> σ* to *log<sub>10</sub> H<sub>V</sub>* with lowest **MAE** is used to fill up the gaps in *log<sub>10</sub> H<sub>V</sub>* with column respect to filled column of *log<sub>10</sub> σ* (**Linear**)
7. Best ML model mapping from *log<sub>10</sub> σ<sub>y</sub>* to *log<sub>10</sub> H<sub>V</sub>* with lowest **MAE** is used to fill up the gaps in*log<sub>10</sub> H<sub>V</sub>* with column respect to filled column of *log<sub>10</sub> σ<sub>y</sub>* (**Decision Tree**)
8. Best ML model mapping from *Compostion* to *log<sub>10</sub> H<sub>V</sub>* with lowest **MAE** is used to fill up the gaps in *log<sub>10</sub> H<sub>V</sub>* column (**Support Vector**)

The notebooks for all these steps are labeled with their respective step numbers.

For each step, the values of performance metrics for each model are compiled and stored in excel files.

``9-Results.ipnyb``: This jupyter notebook is used for comparing all the performance metrics' values of 12 different models used for the 8 different steps and generating the heat map (shown below).

![Figure-4-rev_300dpi](https://github.com/Shakti-95/Multi-propertyML_Multi-objectiveBO_FeCoNi_Alloy_design/assets/12556692/91dbf5f0-c4d7-4e41-844a-b6550e3dea64)
