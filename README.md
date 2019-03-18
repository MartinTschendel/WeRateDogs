# WeRateDogs
Wrangle and Analyze the data from the Twitter WeRateDogs

## Wrangle Report 
 
I separated this project into 4 different parts: In the first part I gathered the required data. Due to the fact, that I conducted this project in China, I normally have to use a Virtual Private Network (VPN) in order to access web sites from the US or Europe. This VPN could not be used because of political conferences conducted by the Chinese government, so I had to ask friends in Germany to download the data and send it via email to me. Anyway, I prepared a cell what should make it possible to download the file image-predictions.tsv with a request library. 
 
In the second part, I assessed the data visually and programmatically. For the programmatic assessment, I mainly used the info(), sort_values() and  value_counts() functions. In the last section of this part, I listed several data quality and tidiness issues of the data. Before that, I also listed four key points from the documents ‘Project Motivation’ and ‘Project Details’. 
 
The third part includes the cleaning work. Before I started with the cleaning process, I made copies from the three gathered data frames. Each cleaning step starts with the description of the issues and includes three sub steps: Within Define, I use words to describe how I plan to solve the respective data quality or tidiness issue. The second sub step is called Coding, here I use python code to conduct the cleaning of the data. In Testing, the third sub step, I check if the code produced the expected result.  
 
During the cleaning process, I merged the three different data frames to a master data frame, what is called df_archive_image_retweet. In the fourth part, I saved that data frame to a new csv file with the name twitter_archive_master.csv. Having the final data frame, it is not too complicated to analyze the data and visualize some of the results.
