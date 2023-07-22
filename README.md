# amazon-review-data-analysis

## Overview
This program is designed to be a data analysis script for analyzing merchandise on the e-commerce platform Amazon. Instead of using existing datasets as we usually do, the data used here is fetched from Amazon by applying the techniques of web scraping. Expect Amazon, this project is also applicable to other online shopping websites like Macy’s or BestBuy with necessary modification.

<img width="441" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/7caa6ed4-331c-42c6-8730-149ff2919ca6">


With flexiblity and power of Pandas, it is used as one of the primary tool in this project for data explorable analysis / manipulation. Beside simple summative data like sales or count of ratings, review could be more valuable as it contains more information, like personal preference or explanation, but it is impossible to read thousands of reviews. Therefore, NLTK does a good job filtering and tokenizing words and extracting the common characteristics of the tokens. Plotly is selected here for data visualization. There are of course more tools out there that could do visualization, like Matplotlib and Seaborn. But Plotly is favored here because it is better at creating web-based data visualizations that can be displayed in Jupyter notebooks especially or web applications using Dash or saved as individual HTML files.


## Usage

**Python Script for web scrapper** 
check scrapper subfolder 

**Jupyter Notebooks for data analytics**
Open Jupyter Notebook: IST_652_final_project_Han_Mo.ipynb
Follow the instructions in the notebook to execute the analysis.



## Results

**Question one, what are the key words favored by distributors in naming the product**

In the cat data list, 8519 tokenized words with 795 unique words, and the top 20 tokens are ['cat', 'food', 'wet', 'dry', 'chicken', 'adult', 'oz', 'pack', 'free', 'grain', 'natural', 'purina', 'lb', 'recipe', 'bag', 'cans', 'variety', 'diet', 'gravy', 'salmon']. 

<img width="326" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/bf25c854-6485-40a7-ac2c-0892587068ed">

Similarly, for dog food list, 791 unique words out of 8602 total words. The top 20 keywords are ['dog', 'food', 'dry', 'adult', 'chicken', 'lb', 'natural', 'recipe', 'bag', 'free', 'wet', 'grain', 'diet', 'rice', 'protein', 'breed', 'small', 'pack', 'oz', 'high']. 

<img width="326" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/75719bda-6cc3-4d14-9aaa-6263d9346ea8">



**Question two, market share of each pet brands in terms of their occurrence**

Using plotly to chart the cat food brand by market occurrence. Besides Others, the top 3 places go to Purina, Blue Buffalo and Hill’s. The percentage of the pie chart represent the total number of a brand’s product over all the product in cat food product data list. For example, 24.3% for Purina means that 24.3 percentage of cat food product selling on Amazon comes from Purina. Surprised to see, the top 4 brands take almost half of the market on Amazon.

<img width="399" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/5b6847fa-3ade-412b-8f0b-22136261e9b6">


In the same way, for dog food product, ranking list by total rating count and pie chart for the market occurrence.

<img width="398" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/8d803d1f-39f1-44a4-833b-d163299f3f73">



**Question three, User Review Key Words analysis**

Look at the review for cat product. the code read 3158 tokenized words with 787 of them are unique. The top 20 words are 'food', 'cat', 'cats', 'gravy', 'loves', 'like', 'eat', 'fancy', 'feast', 'box', 'love', 'price', 'great', 'cans', 'amazon', 'get', 'find', 'little', 'one', 'wet'. 

<img width="325" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/5381836e-f6ec-49bc-9c11-f510aac0c797">

For bigram analysis, I have the top 10 paired word for the reviews of Purina can food.  

<img width="327" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/c061854e-4374-4a03-8cb1-aefd56af7c53">

From the keyword, it is not hard to guess one of the reason this product so popular is because its reasonable price.




For dog product, 2177 tokenized word with 243 of them are unique. The top 20 words are 'dog', 'like', 'dogs', 'refused', 'small', 'bought', 'case', 'eat', 'heat', 'wave', 'issues', 'food', 'cans', 'flavors', 'loves', 'sensitive', 'one', 'buying', 'chicken', 'duck'.

<img width="319" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/714ac39b-e920-4099-be51-3c4fc7360d07">

For bigram analysis, the top 10 paired word for the reviews of Purina ONE SmartBlend True Instinct Adult Canned Wet Dog Food.

<img width="328" alt="Picture1" src="https://github.com/rosalynmo/amazon-review-data-analysis/assets/139208167/c03c7722-2f33-4600-9acf-e15f88a05cd1">

From the key words analysis for this product, we can see consumers are happy about the recipe, since they are talking a lot for the ingredients like ‘chicken’, ‘duck’ and ‘beef’.



