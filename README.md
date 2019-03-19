# WeRateDogs
Wrangle and Analyze the data from the Twitter WeRateDogs

## Wrangle Report 
 
I separated this project into 4 different parts: In the first part I gathered the required data. Due to the fact, that I conducted this project in China, I normally have to use a Virtual Private Network (VPN) in order to access web sites from the US or Europe. This VPN could not be used because of political conferences conducted by the Chinese government, so I had to ask friends in Germany to download the data and send it via email to me. Anyway, I prepared a cell what should make it possible to download the file image-predictions.tsv with a request library. 
 
In the second part, I assessed the data visually and programmatically. For the programmatic assessment, I mainly used the info(), sort_values() and  value_counts() functions. In the last section of this part, I listed several data quality and tidiness issues of the data. Before that, I also listed four key points from the documents ‘Project Motivation’ and ‘Project Details’. 
 
The third part includes the cleaning work. Before I started with the cleaning process, I made copies from the three gathered data frames. Each cleaning step starts with the description of the issues and includes three sub steps: Within Define, I use words to describe how I plan to solve the respective data quality or tidiness issue. The second sub step is called Coding, here I use python code to conduct the cleaning of the data. In Testing, the third sub step, I check if the code produced the expected result.  
 
During the cleaning process, I merged the three different data frames to a master data frame, what is called df_archive_image_retweet. In the fourth part, I saved that data frame to a new csv file with the name twitter_archive_master.csv. Having the final data frame, it is not too complicated to analyze the data and visualize some of the results.

## Data Analysis Report

In this project, I raised three different data analysis questions and defined one objective to visualize the data. In the following section, I raise the questions and communicate respective insights. Afterwards the data visualization will be conducted. 
 
### Regarding the Neural Network: What are the five most frequent #1 dog breed predictions of the algorithm? 
 
The most frequent dog breed prediction is the Golden Retriever with 139 counts. It is followed by the Labrador Retriever, what was predicted 95 times. The third most frequent predicted dog breed is the Pembroke, this breed was predicted 88. The Chihuahua collected 79 counts, followed by the Pug, that breed got 54 predictions. The data frame has totally 1994 entries but dog breed predictions only sum up to 455. The algorithm predicted numerous other things on the pictures like furniture or cars. That is the reason for the difference between the numbers. 
 
### What is the maximum, average and minimum rating of these five dog breeds? 
 
| Dog breed          | Maximum | Average | Minimum |
|--------------------|---------|---------|---------|
| Golden Retriever   | 14.3    | 1.32    | 0.5     |
| Labrador Retriever | 16.5    | 1.39    | 0.7     |
| Pembroke           | 1.4     | 1.14    | 0.4     |
| Chihuahua          | 1.4     | 1.07    | 0.3     |
| Pug                | 1.3     | 1.02    | 0.3     |
 
It is unusual that the maximum ratings of the Golden Retriever and the Labrador Retriever are significantly greater than the maximum values for the three other dog breeds. The five average values don’t show big differences, therefor I assume that the big maximum values are outliers.  
 
### What are the 3 months, during which the most tweeds have been uploaded? 
 
Most of the tweets have been uploaded in January 2016 (169), November 2015 (296) and December 2015 (367). This period is also the starting point for the data collection of the Twitter WeRateDogs. 

### Show the average favorite and retweet count for the dog stages 'doggo', 'floofer', 'pupper', 'puppo' in a bar chart 

![my_image](D:/Udacity/Data_Analyst_ND/Part4-DataWrangling/Project/data/bar-chart-1.png)
