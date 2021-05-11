# Final Project: EPA Toxic Spill Analysis

### Statement of Need

The Environmental Protection Agency has been keeping track of the release of toxic chemicals into the environment since 1987. 
We know that systemic racism, including redlining and white flight, has meant that Black and brown folks are much more likely to be affected by things like worse air quality, pipelines being built across their lands, and more.  Large power plants and other polluters are also much more likely to be built in and around Black neighborhoods (creating things like cancer alley in Louisiana). 
The EPA would like to work to a) find the extent of these issues as they relate to toxic spills in order to find potential interventions or policy solutions to these issues, and b) help predict where these spills might happen again to prevent it. 
This final project will deliver an interactive dashboard using ESRI Insights that showcases: the extent to which toxic spills affect low income communities of color over others, and where we can predict spills to happen again. 

### Phase 1: Exploratory Data Analysis

First I wanted to do some time series exploration of the data.  

#### Type of Industry 

First, I looked at spills by type of industry. We can see that based on number of spills, the chemicals industry is highest, but there are some industries that have shot up in the past 20 years. In terms of amounts, currently the top spiller industry is metal mining, but it didn't beat out chemicals until 1997. In short, it seems like the chemical industry, plus the mining industry seems to be the biggest culprits. We can also see from this (and the next set of graphs) that the overall number and amount of spills has decreased drastically since 1987. 

![image](https://user-images.githubusercontent.com/59181449/117845330-72507200-b24e-11eb-9d91-adb126a9ca76.png)

#### Type of Chemicals

I did a similar analysis for types of chemicals that are being spilled - sodium hydroxide has the most number of spills while aluminum oxide had the largest amount. Both of these, however, seem to be in the past, since the lines don't extend the full way. It seems like other chemicals are now the top spillers. 

![image](https://user-images.githubusercontent.com/59181449/117845588-b2aff000-b24e-11eb-8045-4bb1e34c1d2d.png)

#### Tribe

One thing I was interested in is whether spills have been happening disproportionately on tribal lands, and it seems like that is not the case. Based on all of the spills, very few have happend on tribal land. 

![image](https://user-images.githubusercontent.com/59181449/117845758-d6733600-b24e-11eb-884c-eb434372c06d.png)

#### Carcinogen

Fewer of the spills were spills of carcinogens than I expected as well. 

![image](https://user-images.githubusercontent.com/59181449/117845839-e559e880-b24e-11eb-9cd1-561e355f3797.png)

### Phase 2: Demographics Analysis

Next, I wanted to find out where the spills were happening and how we might be able to analyze whether they were happening disproportionately in Black and brown communities. 

#### Bin Map 

First, I plotted out the spills in a bin map. We can see that a majority of the spills happen on the eastern side of the country, plus California, and that a good number seem to happen along the coast. 

![image](https://user-images.githubusercontent.com/59181449/117846296-4d103380-b24f-11eb-8e78-ce37a3744035.png)

#### Demographics Map

How does that compare to where people live in the US? This is a side by side of percent white and percent nonwhite across US counties. 

![image](https://user-images.githubusercontent.com/59181449/117846587-96608300-b24f-11eb-983a-c64fb1794e48.png)

Based on the above images, we can see that there does seem to be some correlation between where the spills are happening (especially in the counties in California) and counties with a higher percentage of Black and brown communities, but we can delve deeper with spatial aggregation. 

#### Spatial Aggregation

Using spatial aggregation, we can see that not all counties in the US have had spills, firstly.

![image](https://user-images.githubusercontent.com/59181449/117849995-df660680-b252-11eb-8594-0d6f6184869e.png)

Next, we can see the number of spills per county and total releases per county. 

![image](https://user-images.githubusercontent.com/59181449/117850127-03c1e300-b253-11eb-997b-d512e985e820.png)

This shows us essentially what the bin map showed us, but we can see the specific counties (for example, in Texas) that seem to be hardest hit. 

Finally, we can plot the respective interactive terms (CountXPercentNonwhite and AmountXPercentNonwhite) to see counties that have been hardest hit that are also majority Black and brown. This is essential for policy makers to see where the discrepancies are and how to intervene.

![image](https://user-images.githubusercontent.com/59181449/117850402-41267080-b253-11eb-9045-0b9157257f94.png)

### Phase 3: Prediction

Unfortunately, due to the size of the dataset, I was not able to have enough memory in my computer to finish predicting (I tried both hot spot analysis and kernel density) on the full dataset, so I tried it on just the 2019 dataset. 



### Conclusion & Next Steps

This project is simply the start of analyzing where and how these toxic spills happen and how they affect communities of color. There is much that can be done to improve this project, from other ways to visualize the data to deeper analysis on specific counties. For now, however, this dashboard can act as an important tool that can help the EPA find and intervene in counties where spills are happening. 

