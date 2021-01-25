# New Pizza spot in Franklin County


<b> Introduction:

Columbus, Ohio is the state capital of Ohio and located in Franklin County.  

A pizza place with locations in Columbus Ohio is looking to expand into other nearby cities (suburbs) in Franklin County. They know that their most successful pizza location in Columbus is near a park and in areas without many other pizza restaurants. There seems to be an increase in sales when the pizza store is close to a park. They are now looking for which nearby city in Franklin County does not have a pizza place as their top venue, and has parks in their top 5 venues. The investors in the new pizza location have reached out to a data scientist to help assist them with the decision of where to place the new restaurant.

<b> Data needed:

We are going to need a list of the zip codes in Ohio filtered to those in Franklin County. The latitude and longitude of the other cities in Franklin County will need to be calculated so that a list of venues can be found using the foursquare api.  Next we will need to calculate the percentages of venue types relative to each city in Franklin County.

<b> Methodology:

We will need to look at the frequency of venues in the Franklin County city zip codes and filter out any that have pizza places as their most common venue along with the City of Columbus as the pizza chain already has locations there. Next we will look for locations that have parks as one of their top 5 venues. Clustering will be used to compare the different Franklin County cities and find an ideal location where parks are in the top 5 most common venues and pizza places are not the top venue.

<b> Results:

The result was that Upper Arlington was the best location to build in based on the low frequency of pizza places and high frequency of parks.  Since I was using the free foursquare API, the volume of venues pulled was relatively low.  Upper Arlington had parks as the 3rd most common value and pizza places were not number 1:

<b> Discussion:

Based on the results, and since there was only a single park, I decided to plot the location of the park so that the new pizza place could be built next to the park. That map is displayed in the notebook and suggests where the chain could build their new location.  One observation with the pulled data, was that columbus should have been filtered out prior to pulling the data.  By doing this, we would have received many more non-Columbus locations that would not have been filtered out and would have resulted in a more robust data set.  

<b> Conclusion:

In conclusion, Upper Arlington was the best city for the new pizza place. Building next to Falco Park would be ideal based on the pizza place's history with their previous Columbus locations.  
