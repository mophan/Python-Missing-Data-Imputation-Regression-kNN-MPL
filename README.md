
<!-- PROJECT LOGO -->
<br />

  <h1 align="center">Using Python to Impute Missing Data</h1>

<p align="center">
  <br /> 
    <a href="https://github.com/mophan/Python-Missing-Data-Imputation-Regression-kNN-MPL/blob/master/python-mising-data-imputation-regression-knn-mpl.ipynb">View Code</a>
    ·
    <a href="https://www.kaggle.com/kumarajarshi/life-expectancy-who/version/1">Download Dataset</a>
    ·
    <a href="https://github.com/mophan/Python-Missing-Data-Imputation-Regression-kNN-MPL/issues">Report Bug</a>
<br />
<br />  
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#data-description">Data Description</a>
    </li>
    <li><a href="#methodology">Methodology</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

This project performs the imputation of missing values on the life expectancy dataset using the application of linear regression, kNN regression, and neural network regression models in Python with scikit-learn package.   


<!-- DATA DESCRIPTION -->
## Data Description

The dataset is obtained from the website https://www.kaggle.com/kumarajarshi/life-expectancy-who/version/1


There are 20 variables in the dataset which was collected for 193 countries during 16 years from 2000 to 2015. Among those, variables regarding health and life expectancy were collected from the WHO website, while the ecomonic variables were from the United Nation website.

Below are the list of all variables:

   - Life expectancy --           `Average life expectancy (age) for a country in a particular year`
   - Year
   - Status --                    `The status of country (Developed or Developing)` 
   - Adult Mortality --           `Probability of dying between 15 and 60 years per 1000 population`
   - Infant deaths --             `Number of Infant Deaths per 1000 population`
   - Alcohol --                   `Alcohol, recorded per capita (15+) consumption (in litres)`
   - Percentage Expenditure --    `Expenditure on health as a percentage of Gross Domestic Product per capita(%)`
   - Hepatitis B --               `Hepatitis B immunization coverage among 1-year-olds (%)`
   - Measles --                   `Measles - number of reported cases per 1000 population`
   - BMI --                       `Average Body Mass Index of entire population`
   - Under-five deaths --         `Number of under-five deaths per 1000 population`
   - Polio --                     `Polio immunization coverage among 1-year-olds (%)`
   - Total expenditure --         `Government expenditure on health as a percentage of total government expenditure (%)`
   - Diphtheria --                `Diphtheria tetanus toxoid and pertussis immunization coverage among 1-year-olds`
   - HIV/AIDS --                  `Deaths per 1000 live births HIV/AIDS (0-4 years)`
   - GDP --                       `Gross Domestic Product per capita (in USD)`
   - Population --                `Population of the country`
   - Thinness 10-19 years --      `Prevalence of thinness among children and adolescents for Age 10-19` 
   - Thinness 5-9 year --         `Prevalence of thinness among children for Age 5-9`
   - Income composition --        `Human Development Index in terms of income of resources composition (from 0 to 1)`
   - Schooling --                 `Number of years of schooling`

Life expectancy is the output variable, and the rest are the predictors.

<!-- METHODOLOGY -->
## Methodology

### Impute predictors
5 variables have missing values:
- Adult mortality: 10 missing records
- Alcohol: 194 missing records
- BMI: 34 missing records
- Income composition of resources: 167 missing records
- Schooling: 163 missing records

Replacing NULL values in adult mortality, alcohol with 0, and
Substituing NULL values in BMI, income composition of resources, schooling with the respective mean by the status of a country.

### Impute the life expectancy variable
Using 3 different following methods
1. Linear Regression Model
2. Neural Network Regression Model
3. kNN Regression Model

Then compare the mean-squared error (MSE) of 3 methods to find the most accurate results.

_For more details, please refer to the [Project Notebook Document](https://github.com/mophan/Python-Missing-Data-Imputation-Regression-kNN-MPL/blob/master/python-mising-data-imputation-regression-knn-mpl.ipynb)_



<!-- CONTACT -->
## Contact

Mo Phan - helen.dreamsbigdreams@gmail.com

Project Link: [https://github.com/mophan/Python-Missing-Data-Imputation-Regression-kNN-MPL](https://github.com/mophan/Python-Missing-Data-Imputation-Regression-kNN-MPL)


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
