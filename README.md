# data_512_hw_2

The project investigates data bias in Wikipedia articles, focusing on U.S. cities and towns. It examines the quality and quantity of Wikipedia articles for these locations. The analysis includes assessing predicted article quality and exploring state-level patterns in article coverage and high-quality content. The goal is to gain insights into regional disparities in Wikipedia content, particularly how well different U.S. states are represented and the quality of the articles about their cities and towns.

# Datasets

A csv file us_cities_by_state_SEPT.2023.csv, containing the state, page title (city_state) and url. Data is to be acquired for these titles. Has been crawled from https://en.wikipedia.org/wiki/Category:Lists_of_cities_in_the_United_States_by_state.
https://drive.google.com/file/d/1XAydF2Cqjr5u1zs-B9p09JVliqtFYv15/view?usp=drive_link

An excel file NST-EST2022.xlsx, reworked from the original census data (https://www.census.gov/data/tables/time-series/demo/popest/2020s-state-total.html). This file contains the list of states and the 2022 population estimates for each state.

A csv file US States by Region - US Census Bureau - Sheet1.csv, containing regions (Northeast, Midwest etc.), divisions (New England, Middle Atlantic etc.) and states (Connecticut, Vermont etc.)

# API documentation sample document
The below sample codes were referenced for the following tasks and have been provided under the Creative Commons CC-BY license.

Making a page info request
Making an ORES request

# Reproducing the analysis

Open notebooks in Google colab, create a google drive folder with all the input datasets and run the notebooks DATA512_HW_2_DataAcquistion.ipynb, DATA512_HW_2_DataAnalysis.ipynb. 


# Research Implications

This project delved into the qualitative analysis of biases in Wikipedia data, particularly in the quality and quantity of articles across U.S. states. Surprisingly, states with smaller populations like Vermont had a higher number of quality articles per capita than populous ones like California. A significant bias was the focus on English articles, neglecting the linguistic diversity of states like California where many speak other languages. Relying solely on English articles skews the results, as does the use of ORES, which rates articles based on structure rather than content quality. One must be cautious when using biased data for data science research, as it can lead to misleading results. For instance, OpenAI's GPT-3 model, trained on biased data, has shown to generate biased content, underscoring the dangers of deploying such models in real-world scenarios. To address these biases, researchers could supplement the dataset with missing regions or transform it to include non-English articles. The project highlights the need for careful consideration and correction of biases in data science research, emphasizing the importance of a holistic approach to data analysis.
