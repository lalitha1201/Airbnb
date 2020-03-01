# Airbnb Project
Airbnb is a global online platform that helps travellers to find accomodation and good experiences across the globe. Not only this, Airbnb also encourages hosts to post their listings for rental business and guests to book their stay.

# Use Case 1:
I love to travel. And what would be better than finding an accomodation that suits our needs and our budget. We feel like it is a good idea to analyze the Airbnb dataset to understand what features drive the price of various listings.

# Use Case 2:
While on our vacation away from home, it might be a good idea to list our home on Airbnb to make some extra income. Also, buying a property that can be listed on Airbnb seems like a good investment. Again, analysis of features that drive the price of various listings is important for this.

# Airbnb Data:
Data Source: http://insideairbnb.com/get-the-data.html

 # Airbnb datasets:
- Listings.csv
- Calender.csv
The above datasets provide detailed Listings data along with availibilty details for each listing. Some of the features that these datasets contain are:

bedrooms: number of bedrooms in a listing

bathrooms: number of bathrooms in a listing

beds: number of beds in a listing

property_type: the type of property (House, Apartment,..., Others)

room_type: the type of room (Entire Apartment or house, Shared room)

amenities: amenities for the listing (Internet, TV, etc.)

price: price per night

availability_30: number of days available in the next 30 days

accomodates: number of people the property can accomodate.

In this data exploration exercise I will precise the analysis on the Airbnb listings to Seatlle, Washington, United States.

# What Are the Busiest Times of the Year to Visit Seattle?
![Screen Shot 2020-03-01 at 12 05 27 AM](https://user-images.githubusercontent.com/22896571/75622018-9267aa00-5b50-11ea-9792-8c437bc13a69.png)

![Screen Shot 2020-03-01 at 12 05 18 AM](https://user-images.githubusercontent.com/22896571/75622019-9267aa00-5b50-11ea-8e93-98b96c64de3b.png)
# Number of Listings in each Neighbourhood
![Screen Shot 2020-03-01 at 12 05 35 AM](https://user-images.githubusercontent.com/22896571/75622017-91cf1380-5b50-11ea-96a1-ba513fdfdd49.png)
# HeatMap
![download](https://user-images.githubusercontent.com/22896571/75622013-8f6cb980-5b50-11ea-8b5a-be8c203b5413.png)
# K-means and GMM clustering for Price vs Accommodates

![Screen Shot 2020-03-01 at 12 13 41 AM](https://user-images.githubusercontent.com/22896571/75622103-99db8300-5b51-11ea-8ade-5f9dcb17f3ff.png)

![Screen Shot 2020-03-01 at 12 13 33 AM](https://user-images.githubusercontent.com/22896571/75622104-9b0cb000-5b51-11ea-913b-8a3088238c3d.png)

# Analysis
I see the distribution for pricing is strongly skewed right. This again makes sense as a majority of the listings on Airbnb are single individual listings. Additionally, Airbnb does strongly cater to travelers who are looking for cheaper places to stay for short durations of time. There are of course listings with a high pricing as well; intuitively this matches with hosts that are listing a high value property such as an entire house. Looking at the heat map, I can see that 'accomodates', 'bedrooms', 'bathrooms', 'beds' have the highest correlation to the price.

To know how these features affect the price of the listings, I have implemented K means and GMM clustering algorithms on these features vs the price of the listing
The number of clusters is determined using the elbow method.

Both the algorithms formed very much similar clusters but K-means seems doing a better clustering job according to "Price vs Bed" plots. From the GMM plot, the darker green dots has been scattered and mixed with the purple cluster. Also, I see that these features have a positive corelation with the price. As the number of bedrooms, accomodates, bathrooms and beds increase, the price also increases.
# Comparisions of different regression algorithms

