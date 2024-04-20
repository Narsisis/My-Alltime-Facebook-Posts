# My All time Facebook Posts (December 2011 to April 2024)
This report presents the findings of an analysis conducted on my facebook posts data to understand the frequency with which I posts (MoM & YoY). The analysis involves cleaning the data, resampling the data to show frequency, and visualizing the YOY aspects of the post activity.

# Data Cleaning/Processing
The data gotten from facebook was cleaned by extracting relevant information such as date and post and dropping other irrelevant columns.

The date column which was imitially named 'timestamp' was renamed as date and it was saved in datetime format. This two columns are okay for our analysis since the focus here is to understand frequency.

I also checked for NAN values and luckily for me, there were no NAN values.

# Data Analysis
The shape of the data was gotten to reveal the total size of the data. It was revealed that 2601 rows of data was gotten from 2011-12-14 till date of analysis, Apil 20, 2024. This means that I have made 2601 posts since i registered on Facebook till date of this analysis.

The data, being 2601 rows is definitely large and it means I would not be able to get the frequency analysis I needed at a glance, therefore I had to resample the data by Month using the resample method to give us a frequency of how many facebook posts I have made per month for the period of my analysis spanning from December 2011 to April 2024 but before this could be possible, I had to set the index of the data to date and use the datetime64 data type.

After that, I had to get the new shape of the dataset using the shape method to see the length of the resampled data. (149 months)

Once this had been done, I had to use the max function to check the highest number of posts I have made per month and at what month and what year.

The numpy select function was used to create a conditional column indicating on what months I was frequent user of facebook and on what months I wasn't. The threshold for being a frequent user was 30 posts per month; with the rationale that 1 post per day in a 30 day period makes me a frequent user

Also, a line chart was made so I could visualize the trends to spot any patterns or inconsistencies.

# Observations
The analysis revealed constant fluctuations in the number of posts per month, with the highest posting activity observed on 2014-12-01 at 151 ppsts. This particular month I had just gotten a new phone and as usual, i was very active due to the new phone. I also got admission to the university so I guess that could be one of the reasons why.

It also revealed that per year, the months at which I post more frequently were different so no pattern of behaviour could be observed from this.

It also showed that the average number of posts was 17.4

The analysis also showed that out of the 149 grouped data, I was a frequent user 23 times posting more than 30 posts in a month and I was not frequent 146 times

The analysis showed that from janaury 2018 to November 2021, I was a non-frequent user of facebook with my highest number of posts per month within that period as 29 posts. It also showed that during the period of non frequency, in 2019 as a year, I only made 92 posts.

# Conclusion
The analysis of my facebook posts provided valuable insights into the frequency with which I post on facebook. The findings highlight the importance of understanding my posting patterns to see if there was a specific month or year which I made more posts or lesser posts and understand the reasons for these flunctuations.

Ultimately, from my analysis, I can see that I am not addicted to facebook as my posting activity indicates that I am not a frequent user of facebook and as at this year 2024, I have not had a frequent month with my highest posts in 2024 as 13 posts per month.


# Future Directions
Future analysis could explore deeper insights into time stamps to know as at what time of the day I post more. 

