## Overview

Homeowners lean on real estate agents to show them the tricks of the trade and point out things that they otherwise wouldn't consider when buying or selling a home. With a such a large transaction at stake, the agent's expertise and information can make a 5 figure difference in what people pay. 

## Problem

Our goal is to give real estate agents in King County, Oregon some hard data that allows them to turn around and give recommendations to homeowners about how they can increase the value of their home before they put it on the market.

## Data

For this analysis, we had access to infromation about 21,597 homes in King County, Oregon that were sold in 2014 and 2015. Information for each home included items such as size, bedrooms, bathrooms, basements, the size of the 15 nearest homes around them, the quality of the building materials, location, whether or not it's waterfront, and the view from the home.

## Methods

Data cleaning involved turning qualitative data into numerical information, replacing null values with assumed values, and altering some data that was believed to be a result of input error.

Once data was prepared, the StatsModels library was used to create Ordinary Least Squares regressions. This is a form of linear regression modeling that utilizes more than one x variable and aims to minimize the area between the line of best fit and the actual data points. It was a inferential model used to determine the value of the inputs.

The final model ultimately utilized 12 features after removing ones that were deemed unreliable, combined into engineered features, or removed due to having too high of multicolinearity scores.

Once the final model was created, the features were standardized to determine the relative impact they had on home price.

## Results

The model ended up explaining 70.2% of the variance in the data, which gives us reasonable confidence to provide recommendations based on this model.

The most impactful variables were grade, livable area (an engineered feature that included bedrooms, bathrooms, and livable square footage), and latitude. 

More importantly, however are the factors that homeowners have control over. The most important variables that homeowners could control were grade, livable area, condition, and year renovated. 

![price%20factors.png](https://github.com/acollins28/dsc-phase-2-project-v2-3/blob/main/Images/drivers%20of%20price%20most%20to%20least%20impact.png?raw=true)

## Conclusions

The homeowners ability to inrease the value of their home can come in three different methods: improving the grade of the home with some form of renovation, expanding the living square feet, and improving the condition.

Items to improve the grade of a home include: updating plumbing systems, adding wood finishes, upgrading counter tops to something like marble or quartz, adding/redoing insulation, etc. 

Items to improve the living squate feet include: turning on office space into a bedroom, turning a closet into a bathroom, and enclosing a patio.

Items to improve the condition of a home include: cleaning the house, touching up paint, fixing a leaky faucet, and making small repairs to base boards or other damaged areas. 

## Next Steps

While the data set for homes was large enough to make good recommendations on, I would like to rerun this analysis with more updated data. Our data set was only from 2014 and 2015; it would be valuable to see what factors would impact more recent home sales, if there is any difference at all. 

I would also like to run an analysis that included more detailed information about differences between types of views and waterfronts, as well as how lots are laid out. Do lakes have more or less impact than oceans? What about being near a forest area? What constitutes a good view vs a bad view? Does having a larger front yard or back yard matter? Answering these kinds of questions would give us insight into the details of a home that aren't quantified but space or size.

## For more information

For a more detailed breakdown, you can review the notebook [here](https://github.com/acollins28/dsc-phase-2-project-v2-3/blob/main/Notebook.ipynb).

You can also view the presentation slides [here](https://github.com/acollins28/dsc-phase-2-project-v2-3/blob/main/Presentation.pdf).

## Repository Structure

[Images](https://github.com/acollins28/dsc-phase-2-project-v2-3/tree/main/Images) <br>
[Data](https://github.com/acollins28/dsc-phase-2-project-v2-3/tree/main/data) <br>
[Notebook](https://github.com/acollins28/dsc-phase-2-project-v2-3/blob/main/Notebook.ipynb) <br>
[Presentation](https://github.com/acollins28/dsc-phase-2-project-v2-3/blob/main/Presentation.pdf)



```python

```
