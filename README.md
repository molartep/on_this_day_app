# "On This Day": Informational R Shiny App

Martin Olarte, Enzo Mescall, Miles King, and Christina Liang

This project was created to showcase information from a variety of public APIs integreated through a Shiny app in R. App users are prompted to input a date and are subsequently presented with an assortment of information about that date in time. The app aims to inform users on what may have happened that day in a casual and visually appealing way. A live version of the application (as well as further information on the APIs used and app-building process) can be found [here](https://milesfking.shinyapps.io/the-app/) or in the associated R-markdown.

## Featured APIs
This information is pulled from APIs and is categorized based on its content (Astrology, News, Sports, etc.). The APIs that are utilized are as follows:
  - The NASA API
  - The New York Times API
  - The NBA API
  - The Numbers API

### NASA API
Using the free NASA API, we focused specifically on the "Astronomy Picture of the Day" that can be accessed through the APOD section of the API. We were able to retrieve historical images and explanations for a user-inputted date. Returns a JSON with the image, the title of the image, an explanation, copyright, and more.

### New York Times API
Using the NYT API, we were able to return a formatted list of front page NY Times headlines for the specified date. These queried headlines are returned in a JSON along with the first paragraph of the article, author(s), image(s), word count, and a link to the article on www.nytimes.com, among other information.

### The Ball Don't Lie NBA API
The "Ball Don't Lie" NBA API returns NBA box scores for a particular date. This is an unofficial NBA API, but we opted to use it as it is a free API that doesn't require a key to authorize requests. The JSON list returned includes game scores, who the home team was, and who the away team was.

### The Numbers API
The Numbers API is an API that has the capcility, among other things, to return an assortment of random fact about a specified day. We queried the API and retrieved one fact each time an app user searched using a specific date.
