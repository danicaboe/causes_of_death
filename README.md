# Causes of Death
<h3>33 causes of death. 206 countries. 29 years.</h3>
<break>
<p>Death is universal and draws immense fear, pain, curiosity and facination. When I first came across this dataset, questions were easy to come by.</p>
<ul>
  <li>How did the number of deaths change over time? Did they decline, as expected with more advanced health care, or did they increase? Did any remain the same throughout the years? If so, was it the same everywhere or just certain countries/regions?</li>
  <li>Are there countries that have higher death counts for most of the causes? In other words, a vast majority over others?</li>
  <li>Where did each cause of death originate? Did it travel? Did it remain in one place? Did any of them get to near extinction in all countries?</li>
  <li>What proportion of the population did each cause account for in each country? **I am merging a dataset with population data in order to calculate this.**</li>
  <li>Which causes are contagious and which are not? Of those that are not contagious, do the numbers remain relatively stable across all countries? Are they more common in some and less common in others?</li>
  <li>What cause resulted in the most deaths over all countries and years? Which resulted in the least?</li>
</ul>

  
<p>There are so many hypotheses that can be gleaned from this dataset for further exploration. I will be using pandas and python to explore my data. I believe one of the best ways to understand this data is through an interactive map. I will be creating a map with Tableau to share when completed. As I continue to explore the data, I hope to find better questions. Seeking out more data to layer on top of the baseline I have set in order to add context and humanity to the numbers. There is only so much we can ask of this data set. There are so many other variables to look at to glean further understanding. I have questions that can't be answered with this data set because significantly more information is needed.</p>

<ul> My underlying questions are:
  <li>Why are some causes of death more common in specific countries? What other factors are at play? Poverty? Lack of clean water? Lack of health care and medication? Etc.</li>
  <li>What role did the governments of these countries play in mitigating or exacerbating the cause of death? Or did they play no role?</li>
  <li>Was the cause of death a result of a basic human right being unavailable?</li>
  <li>What could change in each country to reduce the impact of their greatest cause of death?</li>
</ul>

<p>I originally found this data set on <a target="_blank" rel="noopener noreferrer" href="https://www.kaggle.com/datasets/ivanchvez/causes-of-death-our-world-in-data">Kaggle</a>. The cleaned data in my ipynb file is downloaded from Kaggle. The uncleaned data originated from <a target="_blank" rel="noopener noreferrer" href="https://ourworldindata.org/causes-of-death#data-sources">Our World in Data.</a> I began with the cleaned data with the intention of connecting to an AWS database and use SQL queries and python to analyze the data. Instead of using AWS, I set up a local postgresql server database and copied the data in the uncleaned csv file into a table in my database. I will now go through the uncleaned data to explore and clean it using PostgreSQL. I found another dataset on <a target="_blank" rel="noopener noreferrer" href="https://www.kaggle.com/datasets/themlphdstudent/countries-population-from-1955-to-2020">Kaggle</a> that provides the population per country from 1955 to 2020. I created a postgresql table and will join the population data with the causes of death data to explore what proportion of each countries population was affected by each cause of death.</p>
