#  Effects of Loan Characteristics on Lender Yield
## by Alexandria Thompson


## Dataset

> The dataset investigated in this analysis was loan data from Prosper. The data constited of 113,937 loans with 81 characteristics. I selected 9 variables to focus on. These variables included lender yield, term, estimated loss, estimated return, propser score, loan original amount, listing category, number of investors, and debt to income ratio. 

>The data can be foun here https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv. There is also documentation on the characteristics found here https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0. 

## Summary of Findings

> In my exploration of this dataset I found that four of the numeric variables that I explored are either positively or negatively correlated with lender yield. The estimated return and estimated loss have postive relationships with lender yield, while propser score and loan original amount have negative relationships with lender yield. I also discovered that term has some effect on the lender yield where all loans with 60 month loans terms do not have any lender yields below about 0.07. The lender yield also peaked in the loans with 36 month terms. 

>In my exploration I also found that listing category had less of an effect on lender yield  and more of an effect on estimated loos and estimated return. I found this to be interesting because lender yield is very closely related to these two variables and I thought that the violin plots of these variables would be very similar. 


## Key Insights for Presentation

> For the rpesentation I am going to focus on the bivariate relationships between lender yield and the 4 selected numeric variables, as well as the multivariate relationship of lender yield and these variables with the term variable included. I will start by plotting the distribution of lender yield and then I will go into the bivariate plots of the relationships between lender yield and the 4 numeric variables. Next I will display the multivariate plots with the same relationships with the addition of the term variable. 

>The Bivariate plots will be regplots that show the data points scttered as well as a regression line to show the direction of the relationship between lender yield and the 4 numeric variables. The multivariate plots will be faceted heat maps that shows the relatioship between lender yield and the 4 numeric variables separated by the term so that you can see the difference between the relationships in each term. 

## Resources

> I used the resources available to Udacity students to complete this project. I used two functions similar to the functions I found in the example project for the violin grid and the faceted heat maps, so that I was able to plot many plots at a time and also display the visuals so they would be easier to compare. 

>I found a way to adjust my faceted heat maps so that the title would not overlap with the labels here https://stackoverflow.com/questions/29813694/how-to-add-a-title-to-seaborn-facet-plot. I used this code plt.subplots_adjust(top=0.9)
g.fig.suptitle('Title'). 