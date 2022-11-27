# DEVF-MachineLearning
Repository of the challenges &amp; projects from the *Machine Learning* module of the **Master in Data Science & Artificial Intelligence** at [DEV.F](https://www.devf.la/master/data/mx).

## Final Project's Module: **Localization of a Vegetarian Restaurant in Mexico**

### **1. Goal**

To define the appropriate location of a Vegetarian Restaurant in Mexico through the use of Machine Learning techniques.

### **2. Data Collection**
Data was collected from the **National Institute of Statistics and Geography** (INEGI, in Spanish) through its API and some static files. In particular, the *National Statistical Directory of Economic Units* and the *Bank of Indicators* were used along with the *Gross Domestic Product* for each Mexican state.

### **3. Data Wrangling**
The collected datasets were cleaned and joined.

### **4. Feature Engineering**
The cleaned dataset was transformed into new variables more suitable for the later Machine Learning modeling.

### **5. Modeling**
Data was modeled using both supervised and unsupervised learning techniques. In particular, **K-means** modeling was also used to create clusters and profile each of the ZIP Codes. Then, a **Lasso regression** model was used to predict the number of vegetarian restaurants as well as performing variable's selection.

### **6. Conclusions**
According to the results of the clustering analysis, four distinct groups were identified:

Cluster |  Profile 
:---:| :---:
0 | Incipient Veggie Area
1 | Booming Veggie Area
2 | Lagging Veggie Area
3 | No Go Area

In this context, a vegetarian restaurant might be located in any member of the clusters **0** (*Incipient Veggie Area*) and **1** (*Booming Veggie Area*). Thus, from the results of both the clustering and the regression analysis, 10 Mexican States in which the Vegetarian food is becoming trendy are:

1. Ciudad de México
2. Michoacán
3. Chihuahua
4. Aguascalientes
5. Nayarit
6. Yucatán
7. Morelos
8. Baja California Sur
9. Durango
10. Tlaxcala

On the other hand, the features with the highest weight on the Lasso regression model were:

- Gross Domestic Product (PIB2020)
- Comercio al por menor exclusivamente a través de internet, y catálogos impresos, televisión y similares
- Comercio al por menor de automóviles y camionetas
- CP_50040 (Estado de México, a No Go Area)

Of course, before commiting any investment, it is suggested to perform a more accurate study. In this sense, other economic, demographic and social variables as well as further ZIP codes could be selected and included in the model.

Furthermore, other clustering and regression techniques could be explored in order to grasp other insights regarding the decision of open a new vegetarian restaurant and where it should be open.
