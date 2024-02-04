# OpenAI Driven Review Intelligence of the Beauty Industry with Spark
[Final Deliverable Dashboard](https://public.tableau.com/views/Productoverview_17070828986800/TopicModeling?:language=zh-TW&:display_count=n&:origin=viz_share_link)

# Executive Summary

Every year, the consumer product goods industry witnesses the introduction of around 30,000 new products, yet less than 10% of them manage to achieve true success, as revealed by the McKinsey Consumer Trend Study in 2019. Understanding customers precisely and timely for product development becomes one of the key strengths of consumer packaged goods (CPG) companies.

Our project's primary objective is to establish a big-data-driven review intelligence and sentiment analysis pipeline, harnessing the capabilities of OpenAI, specifically tailored for the beauty industry. By leveraging LLM, we can think naturally again, effortlessly grasping the key information hidden in the data and conveying business insights efficiently.

# What is in the pipeline?

We leverage Databricks, PySpark, and OpenAI APIs to scalably conduct unsupervised analysis of product reviews to extract topics and classify sentiments. By setting up 4 steps of prompts, we process the review data by batches and merge the resulting topics to get a bag of topics on the full scale of data. By labeling each review with topic and sentiment, we are able to generate a comprehensive dashboard of hierarchical visualizations that is of great use in business settings.

![image](https://github.com/clairetsao/OpenAI-Driven-Review-Intelligence-of-the-Beauty-Industry-with-Spark/assets/145289997/14150031-796f-46b7-bb59-016984a9d53c)

# What are the values?

1. Resolves the token limit of OpenAI prompt input and can handle large contents and generate topics on a full scale of data.
2. Generates nearly completely unsupervised topics results with no number of topics specified.
3. Distinguished from traditional LDA by identifying topics based on its LLM training experience, not on the current dataset alone.
4. Provides a more flexible sentiment analysis option, in which specific customized interest in sentiments can be analyzed easily (e.g. label the reviews that favor the color of this product as "positive in color")
5. Can be easily extended and transformed to many industries, as long as there is available review data
6. Leads to a comprehensive dashboard that provides analysis on different levels (category/subcategory/product)
- Link to the dataset: https://www.kaggle.com/datasets/jithinanievarghese/cosmetics-and-beauty-products-reviews-top-brands
- Link to the project video: https://youtu.be/yFQWXn-usTs

