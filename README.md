# Amazon-Prime-Power-BI-Dashboard


**Background:**

Amazon Prime Video is a subscription-based streaming service offered by Amazon, boasts a vast library of movies and TV shows across various genres and categories. Due to the millions of titles and TV shows readily available to its subscribers, Amazon Prime Video aims to deliver high-quality content, personalised recommendations and an exceptional viewing experience to its users.



![image](https://github.com/user-attachments/assets/7850e2d5-7971-4a4b-b1a0-e31eedaa8c43)


**Problem Definition:**

Despite the extensive content library available on Amazon Prime Video, the platform faces challenges in optimising content selection, understanding user preferences and retaining subscribers. Due to its increasing competition in the streaming industries with the likes of Netflix and Disney + , it is crucial for Amazon Prime Video to leverage data-driven insights to curate compelling content to improve recommendation algorithms and enhance user satisfaction.

**Purpose of Analysis:**

The purpose of this analysis is to leverage Amazon Prime Movies and TV shows data to gain actionable insights that can inform strategic decision-making and drive user engagement and subscriber growth. By analysing aims to address the following objectives:

1.	Content Analysis: Identify the trends in the type of content either Movie or Tv Show available on Amazon Prime including the distribution of movies, series and the frequency of additions to the platform
2.	Director & Cast Analysis: Explore the most prominent directors and cast members featured in Amazon Prime Movies or TV shows.
3.	Release Year Analysis:  Examine the distribution of release years to identify trends in the age of content available on Amazon Prime.
4.	Rating Distributions: Analyse the distribution of release years to understand the types of content available on Amazon Prime.
5.	Genre Analysis: Explore the categories in which titles are listed to understand the diversity of content available.
6.	Description Analysis: Gain insights into the themes and topics covered by either Movies or TV shows on Amazon Prime.

**Data Description:**

The data used for this analysis was taken from the website Kaggle.com included 1k + Amazon Product ratings and reviews the following features in the dataset includes:

-	show_id : The unique ID for each title of Movie or Tv series
-	type : Either a Movie or TV show
-	title:  Title of the Movie or TV show
-	director: The director of the Movie or Show
-	 cast: Cast of Movie/ TV Show
-	country: Country the Movie or TV show is produced and filmed
-	date_added: Date the Movie/Show was added on Prime 
-	release_year: Release year for movie, series 
-	rating: Rating of movie/Tv series
-	duration: the timing of particular titled movie/ Tv series
-	listed_in: genre the movie/TV show is listed in 
-	description: Summary of what the movie/TV show is about



**Data Transformation & Data Cleaning:**

Firstly, I transformed the data into Powe Query in Power BI and I checked for errors and null values in the data column by columns,  
replaced the blank values with 0

![image](https://github.com/user-attachments/assets/0fd87bd4-1755-4870-a746-3dfed6eccf37)



I grouped column Director and Cast to analyse the Top Director and Cast Member:
 
 ![image](https://github.com/user-attachments/assets/5db8bbfb-d9a4-4f6d-885e-2cfac85e8655)



![image](https://github.com/user-attachments/assets/be6c7664-6b00-436e-baf0-bd99b27dc9a4)



Data Modelling and Statistical Analysis:

The following Data Modelling and Statistical Analysis was done to analyse the data and create the Dashboard visualisation in Power BI:


![image](https://github.com/user-attachments/assets/9ae7b243-3017-41f0-b9a3-25655b0c1227)


 
Above is the Dataset in the end when cleaned with Added Measure for Movie Count using DAX :
 ![image](https://github.com/user-attachments/assets/78aa3359-b633-478c-8f2b-517ba8a38980)

This formula counts the distinct values of the “type” column where the type is a Movie.

A measure was also created to Calculate the Percentage of Each content Type. Using the DIVIDE Function, the formulas calculates the percentage of movies by dividing the count of movies by the total count of all rows in the dataset.
 ![image](https://github.com/user-attachments/assets/336b1935-876e-4e0b-b780-0b9227918c99)


These were created in the “Modelling” tab in Power BI to perform the statistical analysis.

A new calculated Column was also created named Content Category 
 ![image](https://github.com/user-attachments/assets/9d9ec291-9bed-4686-875d-3c0f1074f3ed)



This formula creates a new column that categorises each row as either Movie or Series based in the value in the Type column

Data Analysis Report: Amazon Prime Content Dashboard & Insights

The subsequent sections of the report will provide detailed analysis and insights derives from the Amazon Sales Dashboard.


 ![image](https://github.com/user-attachments/assets/c8ee00a7-04c6-4e47-ab8e-6ed46b9d1a0e)


<u>**Insights:**</u>

-	The majority of TV shows were 13+ Rating meaning most are suitable for pre-teens to watch on Amazon prime
-	Given the distribution indicated a generally positive reception from viewers

	![image](https://github.com/user-attachments/assets/22c7d826-e494-4e1d-a8db-a88120a7418d)

<u>**Insights:**</u>

-	Drama is the most prevalent genre across both Movies and TV shows, followed Comedy and Drama with Suspense
-	Movies have a higher representation in Drama and Comedy which indicates a preference for these genres in cinematic formats

![image](https://github.com/user-attachments/assets/51295096-778b-410a-b90e-0a5d29ba28c8)


<u>**Insights:**</u>

In the dashboard you can see the US contributes to the largest number of both Movies and TV shows with 253 content. Followed by India with 229 content.


![image](https://github.com/user-attachments/assets/488b2a0b-0c2e-4281-b73f-e7a573a4b275)


The datasets contains a high number of movies with 7.81K compared to TV shows which represents a greater emphasis for cinematic content.
The ratio of Movies and TV shows is approximately 80% to 19% 




![image](https://github.com/user-attachments/assets/9de81595-e47c-4c0c-afbf-f76accef004b)

<u>**Insights:**</u>

-	This graph represents the steady increase in the number of Content either Movie or TV shows over the years based on the release_year . This reflects the growing content available on Amazon Prime Video
-	Recent years show a significance spike in the number of releases indicating the upward trend in content production and traction of users to the  Amazon Prime Video platform


**Conclusion:**

The analysis of the Amazon Prime Video dataset provides valuable insights into the distribution of ratings, genres, countries of origin and trends in content production over time. These insights can inform content acquisition strategies, user engagement initiatives and platform expansion efforts to enhance the overall viewer experience on Amazon Prime Video.

The analysis above identifies opportunities to attract and retain subscribers through targeted marketing campaigns and promotional offers for upcoming Movies and Prime TV shows expected to showcase on the platform.



<u>**Recommendations**</u>
1.	Identify Top performing content: Based on viewership prioritise promoting and featuring top-performing movies and TV shows prominently on the platform.
2.	Invest in acquiring rights to top performing Tv shows and movies to stream on platform.
3.	Personalised recommendations:  Diving deeper with data create machine learning algorithms to personalise content recommendation based on individual user preferences, viewing history etc.
4.	View behaviour analysis of duration sessions it takes for a user to watch a TV show/ movie in its entirety. 
5.	Explore partnerships with content creators, production studios and influencers to create exclusive content and promotional tie-ins that drive subscriber growth
6.	Diversify content library: Cater to a wide range of interests and preferences while including niche genres and international content


References

-	Bansal, S. (2021, October 12). Amazon prime movies and TV shows.
  Data Source- Kaggle( https://www.kaggle.com/datasets/shivamb/amazon-prime-movies-and-tv-shows)


