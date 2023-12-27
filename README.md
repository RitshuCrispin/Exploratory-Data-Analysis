# Exploratory-Data-Analysis
To study the data collected over the past few years and to determine what factors influence the price of a vehicle's ad. To do so, i'm going to do the exploratory data analysis and then get conclusions about it.

# Overview
This dataset contains hundreds of free vehicle ads posted on one website every day.

## Objective
 
To study the data collected over the past few years and to determine what factors influence the price of a vehicle. To do so, i'm going to do the exploratory data analysis and then get conclusions about it.

## Language
- Python | It was worked in Jupyter Notebook.

## Libraries
- Pandas
- Matplotlib
- Seaborn

## Conclusion

1. During the data exploration, problems were found with the data in some columns, from presenting missing values to having an inappropriate typology. It is presumed that in the case of the `is_4wd` columns the missing values must have been `0` and that is why they were omitted from the record; For the other columns with missing values, it is believed that there were human errors when recording the data since they did not show any pattern that can be related.
2. To treat the missing data, the relationships of the columns had to be conceptually analyzed to identify which characteristic is related to or has greater dependence on the columns that present null values. In this way, `model_year` was completed with the median based on `model`, `cylinders` with the median of `type`, `odometer` with the median of `condition` and in the case of `paint_color` it was completed with the value `unknown`.
3. Next was the enrichment of the dataframe with new data such as the year of the date the advertisement was placed and the age of the vehicle. This allowed us to study and treat the main parameters, analyzing, with the help of boxplot, whether they have atypical values.
4. Once the atypical data were identified, a clean dataframe was created that served to draw a histogram for each column to be studied and compare them with the previous graphs.
5. Finally, the following is concluded:
- Truck and pickup type vehicles are more popular in terms of the number of ads and cost more than the others.
- The more current the car model, the more it will cost.
- The lower the mileage of the vehicle, the higher the price.
- The better the condition of the car, the greater its value.
- The color of the car and the type of transmission do not influence the price much.
