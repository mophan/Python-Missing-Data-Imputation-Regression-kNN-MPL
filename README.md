
<!-- PROJECT LOGO -->
<br />

  <h1 align="center">Using Python to Indentify What Factors Influence Life Expectancy</h1>

<p align="center">
  <br /> 
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Download Dataset</a>
    ·
    <a href="https://github.com/mophan/Python-What-Factors-Influence-Life-Expectancy/issues">Report Bug</a>
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

1. Life expectancy:           _Average life expectancy (age) for a country in a particular year_
2. Year
3. Status:                    _The status of country (Developed or Developing)_ 
4. Adult Mortality:           _Probability of dying between 15 and 60 years per 1000 population_
5. Infant deaths:             _Number of Infant Deaths per 1000 population_
6. Alcohol:                   _Alcohol, recorded per capita (15+) consumption (in litres)_
7. Percentage Expenditure:    _Expenditure on health as a percentage of Gross Domestic Product per capita(%)_
8. Hepatitis B:               _Hepatitis B immunization coverage among 1-year-olds (%)_
9. Measles:                   _Measles - number of reported cases per 1000 population_
10. BMI:                      _Average Body Mass Index of entire population_
11. Under-five deaths:        _Number of under-five deaths per 1000 population_
12. Polio:                    _Polio immunization coverage among 1-year-olds (%)_
13. Total expenditure:        _Government expenditure on health as a percentage of total government expenditure (%)_
14. Diphtheria:               _Diphtheria tetanus toxoid and pertussis immunization coverage among 1-year-olds_
15. HIV/AIDS:                 _Deaths per 1000 live births HIV/AIDS (0-4 years)_
16. GDP:                      _Gross Domestic Product per capita (in USD)_
17. Population:               _Population of the country_
18. Thinness 10-19 years:     _Prevalence of thinness among children and adolescents for Age 10-19_ 
19. Thinness 5-9 year:        _Prevalence of thinness among children for Age 5-9_
20. Income composition:       _Human Development Index in terms of income of resources composition (from 0 to 1)_
21. Schooling:                _Number of years of Schooling_

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

Replacing null values in adult mortality, alcohol with 0; in BMI, income composition of resources, schooling with the respective mean by the status of a country.

### Impute the life expectancy variable
Using 3 different following methods
1. Linear Regression Model
2. Neural Network Regression Model
3. kNN Regression Model

Then compare the mean-squared error (MSE) of 3 methods to find the most accurate results.

_For more details, please refer to the [Project Notebook Document](https://example.com)_



<!-- CONTACT -->
## Contact

Mo Phan - helen.dreamsbigdreams@gmail.com

Project Link: [https://github.com/mophan/Python-What-Factors-Influence-Life-Expectancy](https://github.com/mophan/Python-What-Factors-Influence-Life-Expectancy)


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
