# data_512_hw_2

The project investigates data bias in Wikipedia articles, focusing on U.S. cities and towns. It examines the quality and quantity of Wikipedia articles for these locations. The analysis includes assessing predicted article quality and exploring state-level patterns in article coverage and high-quality content. The goal is to gain insights into regional disparities in Wikipedia content, particularly how well different U.S. states are represented and the quality of the articles about their cities and towns.

# Datasets

A csv file us_cities_by_state_SEPT.2023.csv, containing the state, page title (city_state) and url. Data is to be acquired for these titles. Has been crawled from https://en.wikipedia.org/wiki/Category:Lists_of_cities_in_the_United_States_by_state.

An excel file NST-EST2022.xlsx, reworked from the original census data (https://www.census.gov/data/tables/time-series/demo/popest/2020s-state-total.html). This file contains the list of states and the 2022 population estimates for each state.

A csv file US States by Region - US Census Bureau - Sheet1.csv, containing regions (Northeast, Midwest etc.), divisions (New England, Middle Atlantic etc.) and states (Connecticut, Vermont etc.)

All three files are located here https://drive.google.com/drive/u/0/folders/1mkQ97wqeDt-HGH7xu4anzKcIYYcpqJJA

# API documentation

ORES Wiki Overview: https://www.mediawiki.org/wiki/ORES

Wikipedia Article Evaluation: https://en.wikipedia.org/wiki/Wikipedia:Content_assessment

Wikimedia API Reference Guide: https://www.mediawiki.org/wiki/API:Info

# Reproducing the analysis

Open notebooks in Google colab, create a google drive folder with all the input datasets and run the notebooks DATA512_HW_2_DataAcquistion.ipynb, DATA512_HW_2_DataAnalysis.ipynb. 


# Research Implications

Reflection
Understanding a data science project requires both quantitative and qualitative analysis. This project highlighted biases in data, influenced by factors like demographics, religion, and culture. It revealed that articles per capita might not be the best measure, with states like Vermont showing higher articles despite a smaller population. This could be due to factors like a stronger community of contributors. Online data inherently has biases stemming from various socio-cultural factors. Recognizing these biases is crucial to ensure accurate interpretations and results, especially when considering the influence of population and linguistic proficiency on the quality of articles.

What biases did you expect to find in the data (before you started working with it), and why?

Data biases were evident, with population centers significantly influencing per capita rankings. Major cities showed varied article quality, likely due to frequent edits. Additionally, cities' naming patterns, often excluding state names, require special handling. Impressively, no data was missing after using the ORES calls, highlighting its scalability and consistency. A deeper exploration into how ORES evaluates articles, its parameter weightage, and its scoring methodology would be insightful.

What might your results suggest about (English) Wikipedia as a data source?

Wikipedia offers vast potential as a data source due to its extensive content. While this project focused on article metadata, there's a wealth of other analyses possible. Though widely regarded as reliable, Wikipedia's open-source nature allows anyone to edit, leading to potential inaccuracies and past "edit wars" that resulted in locked articles. Despite its vulnerabilities, Wikipedia remains a valuable resource for diverse analyses, from page views to article quality, offering numerous opportunities for data analysts.

Can you think of a realistic data science research situation where using these data (to train a model, perform a hypothesis-driven research, or make business decisions) might create biased or misleading results, due to the inherent gaps and limitations of the data?

Using open-source data like Wikipedia for research presents challenges due to inherent biases, including geographical and economic factors. For instance, larger population centers affected article quality in our study. Algorithms trained on such data can produce skewed results, potentially compromising the analysis. Overrepresentation can distort data-driven decisions, emphasizing the need for careful decision-making in data science to avoid real-world repercussions.

How might a researcher supplement or transform this dataset to potentially correct for the limitations/biases you observed?

Wikipedia offers significant value for data science research, especially in time series analytics due to its reliable historical data. Its vast information makes it a primary online resource. The Wikimedia Foundation enhances this potential by offering advanced APIs, giving access to extensive data and tools for better understanding. These resources position Wikipedia as a compelling data source for data science, a sentiment I, as an emerging data scientist, strongly resonate with.

