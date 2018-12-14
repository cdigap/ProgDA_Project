# ProgDA_Project
Programming for Data Analysis - Project 2018

# Problem statement
For this project you must create a data set by simulating a real-world phenomenon of
your choosing. You may pick any phenomenon you wish – you might pick one that is
of interest to you in your personal or professional life. Then, rather than collect data
related to the phenomenon, you should model and synthesise such data using Python.
We suggest you use the numpy.random package for this purpose.
Specifically, in this project you should:

• Choose a real-world phenomenon that can be measured and for which you could
collect at least one-hundred data points across at least four different variables.

• Investigate the types of variables involved, their likely distributions, and their
relationships with each other.

• Synthesise/simulate a data set as closely matching their properties as possible.

• Detail your research and implement the simulation in a Jupyter notebook – the
data set itself can simply be displayed in an output cell within the notebook.


# Data Preparation
For this project I am using the Life expectancy data and build my own data set from it. 

## Objective

Life expectancy has been increasing in a steady pace from last century till now. Considering the same want to understand what will be our life expectancy in X + N years where x is the current year and n would be the number of years later we want to know. 

During the analysis I found that the life expectancy is dependenct of the income and or Development status of the Country or region the peopple are living. From the analysis I found out that the life expectancy(Lifeexpectancy) of a country is increasing in a steady pace every year (Year). This is also affected by growth status(DevelopmentStatus = Least developed countries / Less developed regions / More developed regions) of the country. Life_expetancy is different for a male and a female.

So Let us use the below 5 different variables for our analysis.

* Year
* Development_status
* Men
* Women
* Life_Expectancy

The Data that we will be createing with an algorithm, is based of the real life scenario of Life expectancy of the different regions depending on the Development status we have categorised into 3.

* More Developed Regions
* Less Developed Regions
* Least Developed Regions

For the purpose of this project I have taken the start year for data collection as 1950 to 2015, so each different Development status region will have 66 entries. The Men and Women life expectancy is calculated used a np.random package. The overall Life Expectancy is calculated as a mean of the both Men and Women life expectancy for each line.

### Data cleanup 
Activities for data cleanup have also been discussed as well, Creating different data sets and appending them to make one Data freame and then updating the values to match the requirement for easy analysis. After this Data indexing has been done so that it would easy to retrieve and easier to work with.

Created a lof of different plots which explains in itself how the data is trending. Plots like Scatter plot, Box plots, graph showing the trends and relationship between the different varialbes.

Created subsets of data using Development status as the criteria, 3 data sets, c_More, c_Less, c_Least.

### Distributions 
Discussed about Distributions. Used the data to explain the *Normal Distribution* and wrote code to perform the related calculations and plotted a few graphs
* Plotting the normal distribution for Life expectancy More developed regions - Men.
* Plotting the normal distribution for Life expectancy More developed regions - Women.

### Data Relationships
Discussed about how the data is related to each other by performing the *t-Test for independent samples* wrote code for calcluation.
* Comparison between Men and Women by Development Status.
* t-Test for Dependent Samples
Also discussed *Chi Square test* wrote code for calculation.
* Chi-Square test with similar proportions

### Correlation
Explained about correlation between between Men's and Women's ages we can clearly see that the if the Men's age increases, we see that the women's age is increasing as well. This will directly increase the Life expectancy of the Region. 
* Average Life expectancy of More  / Less / Least Developed Region
* Graph showing Male and female life expectancy in More / Less / Least Developed Region

Discussed about *Pearson* and *Spearman* Correlations
* Graphed with a color coding.

### Regression
Discussed about Linear Regression for More Developed Regions as the results will be similar for all the three different regions
* Graph for life expectancy of More Developed Regions
Using Linear Regresssion techniques splitted the data and using the train test split method predicted the life expectancy for future.


#  Reference 
1. https://ourworldindata.org/life-expectancy
2. https://stackoverflow.com/
3. https://erikrood.com/Python_References/
4. https://machinelearningmastery.com/how-to-code-the-students-t-test-from-scratch-in-python/
5. https://www.datascience.com/blog/introduction-to-correlation-learn-data-science-tutorials
6. https://ourworldindata.org/ https://plot.ly/python/plot-data-from-csv/ 
7. http://onlinestatbook.com/2/logic_of_hypothesis_testing/steps.html 
8. https://www.khanacademy.org/math/statistics-probability/significance-tests-one-sample/idea-of-significance-tests/v/simple-hypothesis-testing![image.png](attachment:image.png) 
9. https://www.kaggle.com/chrisbow/cleaning-data-with-python-challenge-day-1 
10. https://www.dataquest.io/blog/data-cleaning-with-python/  
11. http://www.statslab.cam.ac.uk/~rrw1/stats/Sa5.pdf![image.png](attachment:image.png)
12. https://researchbasics.education.uconn.edu/t-test/# 
13. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3900058/![image.png](attachment:image.png) 
14. http://pytolearn.csd.auth.gr/d1-hyptest/12/ttest-1sample.html 
15. http://www.learningaboutelectronics.com/Articles/How-to-plot-a-graph-with-matplotlib-from-data-from-a-CSV-file-using-the-CSV-module-in-Python.php![image.png](attachment:image.png)
16. http://pytolearn.csd.auth.gr/d1-hyptest/12/ttest-paired.html![image.png](attachment:image.png) 
17. https://medium.com/@sebastiannorena/finding-correlation-between-many-variables-multidimensional-dataset-with-python-5deb3f39ffb3 
18. https://pythonhealthcare.org/tag/linear_regression/ 
19. http://hamelg.blogspot.com/2015/11/python-for-data-analysis-part-27-linear.html 
