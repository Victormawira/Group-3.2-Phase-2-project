
![pr](https://user-images.githubusercontent.com/124495669/233356860-524bd666-5dd6-4404-848d-95244e65f371.jpg)
## Business Overview
Housing has been the long-term focus of urban development and social and economic policies, not only to the medium level economies but also to the high economies.House Price prediction are very stressful work as we have to consider different things while buying a house like the structure and the rooms kitchen parking space ,the period/time of purchase/ sale of the houses,the bedroom number,the house grade,the year it was built and the floors.
It can further be argued that the subject of ‘affordability’ of housing has become unclear because it addresses numerous issues as already explained on the above factors that come to play when determining the prices of houses in various parts of the globe.
To establish how diffrent factors affect housing prices The use of multiple linear regression modelling can easily help identify the house which is to be perfect for the customers and helps to predict the price accurately.It will also enable the house owners while making decisions on which houses to sell and the rate they earn after  the renovations . The renovations done to some houses and others left out will help determine if they do raise the values of the houses or not thus giving quality advice to the home owners.

## PROBLEM STATEMENT

The Northwestern County housing situation is one that is worth investigating as housing pricing within region is something that cannot be ignored since it affects the majority. the industry is also one that is operating in a very competitive market, just like in other parts of the globe.
The real estate agency within the county have contacted a group of data scientists to help inform the homeowners when to buy/or and sell homes. The specific issue in this case will be to help homeowners make appropriate decision, on whether renovation affects the property values, hence pricing or whether other factors like bedroom and areas of both house and compounds can as well influence the pricing.
The specific issues to be established in this case is the factors that affects the pricing of houses and homes in the Northwestern county.

## Data
This project uses the King County House Sales dataset, which can be found in kc_house_data.csv

## Data Understanding

#### Libraries Used
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
from scipy import stats
import warnings
warnings.filterwarnings("ignore")
import statsmodels.api as sm
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression

#### Loading Data

df = pd.read_csv('data/kc_house_data.csv')

#### Desciptive Data

df.shape
len(df)
df.columns
df.info()

## Data Cleaning

cleaned(df)

## Visualizations

![price](https://user-images.githubusercontent.com/124495669/233357684-44b0fa3d-251f-4dda-8b42-b22be7bc6ba5.png)
![BATH](https://user-images.githubusercontent.com/124495669/233357739-6c835755-53ec-478f-a60f-29d107e2ddac.png)
![BEDS](https://user-images.githubusercontent.com/124495669/233357767-47707131-f0d1-463e-b7d6-5e7468333410.png)
![grade](https://user-images.githubusercontent.com/124495669/233357806-a1573820-d9ce-4b7c-82aa-f9adf618cbe4.png)
![water](https://user-images.githubusercontent.com/124495669/233357858-ccc3cdeb-3a7e-4d8e-aae0-9c1d5a44e311.png)
![Screenshot (269)](https://user-images.githubusercontent.com/124572155/233436542-eddcbfcb-10da-4c24-96ad-984a3a14b46f.png)

## Conclusion(s)

The above implies that testing data worked better than the prediction data hence the increase in a value of the r2 parameters. We can conclude that independent variables affects price of houses as  depicted by r2 values showing the significance between bedrooms,bathrooms, sqft_living, floors, waterfronts, veiw, grade, sqft_above etc. affects the price of housing in the area

## Recommedation(s)

1. Homeowners should consider the following when building; bedroom numbers, bathroom numbers, sqft_ living area, sqft lot,quality of the house, sqft basement, vicinity of the house.
2. Housing agency should be aware that timing affect the price and should therefore advice homeowners on when to build and sell.
3. Consider other algorithms beyond multiple linear regression
4. Consider regression methods that can deal with under or over fitting 
