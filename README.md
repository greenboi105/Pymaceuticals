# Pymaceuticals Plotting

The Jupyter notebook containing the analysis is named plotting.ipynb.

We want to utilize the different tools in the Anaconda Data Science toolset to analyze the effectiveness of different drugs on the tumor volume of various mice over the course of a number of days.

We can utilize visualization techniques to extract general trends and insights.

## Overall Process

1. We begin by cleaning the prescribed data and filtering out duplicate and invalid rows. We discover that the entries for mouse with ID g989 is invalid (likely due to the hypothetical timepoint measurements). Knowing that there is a single invalid mouse ID, we remove all entries of that mouse from the DataFrame.

2. The second step is to comute summary statistics of the mice treated with each drug regimen. To do so, we utilize a groupby with the 'Drug Regimen' and focus on the 'Tumor Volume (mm3)' characteristic. We compute the mean, median, variance, standard deviation and standard error of the mean group.

3. We want to know more about the aspects of the hypothetical study, and so we plot the number of mice treated with each drug along with the gender distribution of the mice.

4. Lastly, we want to focus on the treatments Capomulin, Ramicane, Infubinol and Ceftamin. We can compute the quartiles and associated outliers, then utilize a boxplot to visualize the spread of the data.

5. Our final point of interest is the relationship between weight and the average tumor volume. As expected, there is a positive correlation between the two features. We can plot the scatter relationship and compute a line of best fit between the two features.
