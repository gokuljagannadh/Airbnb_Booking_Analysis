# Airbnb_Booking_AnalysisAirbnb Booking Analysis


# 1.Abstract

Airbnb, the world leader in accommodations, allows us to find places to stay directly from individuals in thousands of cities around the world. On the other hand, it allows you to rent apartments or even entire houses from people all over the world. In this work, we explore and analyse the Airbnb data set (2019) of New York City and thereby unravel the dynamics of different variables associated it.

# 2. Problem Statement
The company has provided a data set of New York City (2019) comprising 49,000 observations and 16 columns.  It is a combination of categorical and numeric values. The main objective of this project is to identify various insights on how Airbnb listings are distributed across NYC by understanding each column in the data set. Some of our key objectives are
•	What can we learn about different hosts and areas?
•	What can we learn from predictions? 
•	Which hosts are the busiest and why?
•	Is there any noticeable difference of traffic among different areas and what could be the reason for it?

# 3. Introduction  

Airbnb is already a multi-billion dollar company having a presence in 190+ countries across the world; it is now concentrating to further increase the daily transactions on its platform depending on the customer needs. The business model of Airbnb has become stronger as people prefer staying at an Airbnb rather than a hotel. Guests and hosts have used Airbnb to expand on possibilities regarding travel and present a more unique  way of experiencing the world since 2008. Nowadays, Airbnb became one of a kind service that recognized and passed down by the whole world. Data analysis on millions of listings provided on Airbnb is a crucial element for the company. These millions of listings generate a lot of data. Data that can be analysed  and used for security, business decisions, understanding of customers' and providers' (hosts) behaviour and performance on the platform, guiding marketing initiatives, implementation of innovative additional services and much more. The purpose of our team is to explore a publicly open dataset. Here, we make use of the Airbnb dataset of New York City to apply EDA and map the result clearly through visualization tools, and give new insight to the public and other relevant parties.

3.1 What is EDA?

 “Exploratory Data Analysis is a detective work. EDA can never be the whole story, but nothing else can serve as the foundation stone — as the first step”.  This is a quote by the renowned Data Scientist John W. Tukey in 1970. In simple language, exploratory data analysis (EDA), also known as Data Exploration is a step in the Data Analysis process, where several techniques are used to better understand the dataset being used. The key steps involved in EDA are
•	Acquire and loading data
•	Understanding the variables
•	Cleaning dataset
•	Exploring and Visualizing Data
•	Analyzing relationships between variables 

3.2 Understanding the Variables

In this session, we do the basic inspection of our data set and familiarise the columns. In the Airbnb data set of NYC, we have 16 columns in total, which is a combination of numerical and categorical variables. By doing the basic inspection, we can easily figure out which ones are categorical variables and which ones are numerical variables. Some columns are not significant for our analysis which can also be kept off. Now let’s look at some of the useful columns in our data set.

3.2.1 Host Id

•	Host Id is the government approved id for each individuals who rents their properties on Airbnb. 
•	This is one of the numerical variables associated with each host. 
•	There are about 37457 unique values in the data set.
•	There exist multiple listings corresponding to a particular host id.

3.2.2 Host Name

•	Host names are basically the names of the individuals or organisations who rent a rooms/apartment in Airbnb website.
•	In order to protect the privacy of both hosts and guests, they don't share last names until after a booking is confirmed.
•	Also there are three types of hosts.
o	Listing owner: The person who lists the space in their Airbnb account. This is usually the person who owns the property or living in the property.
o	Co-Host: Someone, usually a friend or family member, who helps the Host manage their place. The listing owner decides whether the co-Host appears as the primary Host on the listing or not.
o	Hosting team: A hosting team is a business or team of people that manages places to stay on behalf of the listing owner. 
•	There are about 11453 unique values out of 48895 observations.
•	This variable is categorised as a categorical variable since a particular individual or organisation can own multiple types of rooms.

3.2.3 Neighbourhood

•	When searching for accommodations in a city, guests are able to filter by neighbourhood attributes and explore layers of professional-quality content, including neighbourhood maps, custom local photography and localized editorial, details on public transportation and parking, and tips from Airbnb’s host community.
•	By looking at the neighbourhoods, the guest can match neighbourhood’s personality with their own.
•	In Airbnb dataset, neighbourhood is a categorical variable

	
3.2.4 Neighbourhood groups	

•	Neighbourhood groups are the clusters of neighbourhoods in the area. 
•	In NYC the neighbourhood groups are generally the boroughs. There are about 5 boroughs in the state.
•	Since there are many neighbourhoods in each borough, it is a categorical variable. 

3.2.5 Room type

Airbnb has 3 categories for types of spaces:
•	Entire house/apartment
•	Private room,
•	Shared room.  
Entire house or apartment generally means a full unit with bedroom, bath and kitchen.  Private room generally means you get your own private bedroom where no one has access to (i.e. you are not sharing it with the host or another guest).  Shared room means you are sharing a room with someone who is another guest or your host. You are also supposed to stay on the couch in the host's living room, so it is not really private, it's a living room during the day, and you sleep there at night.

3.2.6 Price

The total price of your Airbnb reservation is based on the rate set by the Host, plus fees or costs determined by either the Host or Airbnb.
  
Types of fees
•	Airbnb service fee:  Guest service fee charged by Airbnb, this provides 24 hours community support and helps everything run and ensure the system runs smoothly.
•	Cleaning fee: Charged by some Hosts to cover the cost of cleaning their space (applicable to all countries except China).
•	Extra guest fee: Charged by some Hosts for each additional guest beyond a set number.
•	Security deposit: Some reservations may require a security deposit requested by the Host or Airbnb—find out more about security deposits.
•	Value Added Tax (VAT, JCT, and GST): Charged to guests who live in certain countries—find out more about VAT.
•	Local taxes: Charged based on the location of the Host's place—find out more about local taxes.
3.2.7 Other relevant variables
•	Reviews per month: insights into frequency of visits of the listing
•	Minimum nights: indicator of minimum stay length, to be used with the number of monthly reviews
•	Availability 365: It is an indicator of the total number of days the listing is available for during the year.
# 4. Null Value treatment

Our dataset contains a large number of null values which might tend to disturb our accuracy hence we dropped them at the beginning of our project in order to get a better result.

# 5. Data Visualisation
Data visualization is the graphical representation of information using visual elements like charts, graphs, and maps. Data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data. In the world of Big Data, data visualization tools and technologies are essential to analyze massive amounts of information and make data-driven decisions. Here we make use of the tools matplotlib and seaborn to visualize data. The distributed plot, bar plot and scatter plot are the few graphical representations that are included in our work.
# 6. Summary
1. Learning about hosts and areas:-Manhattan has highest number of listing but in
private rooms Brooklyn is leading and Manhattan Is leading because of higher number
of Entire room\apartment.

2. Traffic among different Neighbourhood. Manhattan has highest number of
listings followed by Brooklyn and Staten island has the minimum number of listings
we have seen it after plotting Neighbourhood with total number of listings in
the Neighbourhood.

3. Prediction on different columns of dataset ( exp :-price, availability etc.):-
Manhattan has highest mean price and Bronx is minimum.

4. Which are the busiest host and why :- the busiest host is Sonder(NYC) followed
by Blueground and Kara. These hosts are busiest because they have higher number of
listing and availability is less.
