# Baseball Regression Analysis for Runs/Runs Created

## Regression Analysis
`y = dependent variable = runs scored in a season`

Independent (**X**) variables used:
 - BB+HBP
 - Singles
 - Doubles
 - Triples
 - Home runs
 - Stolen bases
 - Caught stealing

`Predicted runs for season = Constant + B1(BB+HBP) + B2(Singles) + B3(Doubles) + B4(Triples) + B5(Home Runs) + B6(Stolen Bases) + B7(Caught Stealing)`

### Meaning of p-values

Any idependent variable with a _small_ p-value (traditionally means <.05, even though this choice has been arbitrary) is considered to be a useful predictor of the dependent variable (after adjusting for the other independent variables).  

**Essentially,** the p-value for an independent variable gives the probability that (in the presense of all other independent variables used to fit the regression) the independent varaible **does not enhance our predictive ability (or equivalently the probability that the value of the weight is obtained purely by chance, and in reality the coefficient is zero).**

## Scrapper
Scrapper will use `https://www.baseball-reference.com/leagues/majors` as the base url to get the yearly team statistics over time. 
