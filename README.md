# Pystars-Project-1

## Housing Analysis
---
An Analysis of Housing Sales in El Paso County in 2021
![House](Images/pexels-binyamin-mellish-106399.jpg "House")

## Members
---
|Names             | Profiles                                |Rank        |
|:----------------:|:---------------------------------------:|:----------:|
|Will Serene       |[GitHub](https://github.com/willserene)  |Group Leader|
|Abhi Shrestha     |[GitHub](https://github.com/abhikenobi)  |Group Member|
|Christine Chitechi|[GitHub](https://github.com/cchitech)    |Group Member|
|Alex Merriex      |[GitHub](https://github.com/amerriex24)  |Group Member|
|Rob Thompson      |[GitHub](https://github.com/rob10thhuman)|Group Member|

<a href="http://www.youtube.com/watch?feature=player_embedded&v=IGneD1n75u8
" target="_blank"><img src="http://img.youtube.com/vi/IGneD1n75u8/0.jpg" 
alt="Intro" width="600" height="450" border="10" /></a>

---
### Introduction
---

The Pystars group welcomes you to our project repository/analysis created and submitted to The University of Denver's Data Analytics Bootcamp as our group project.

The goal of this project was to conduct an analysis on housing prices of homes sold in El Paso County in 2021. We were curious as to what affected the price a home sold for. For this, project we narrowed down such an open-ended question to three factors.

### Factor 1
---
The first factor considered was the `**walk score**` of a house. The walk score of an address measures the walkbility of that address by analyzing hundreds of walking routes to nearby amenities. Based on the distance of those amenities, points are awarded towards the score, the maximum limit set at a distance within a 5 min walk/ 0.25 miles and decaying for amenities further outside that radius. The group hypothesized that a higher walk score would result in properties being sold at higher prices.
![Walking](Images/pexels-godisable-jacob-1353029.jpg "Walking")

### Factor 2
---
The second factor we researched was the exitences of a shcool nearby as well as the ranking of that school. The group wanted to research and analyze if the option of `**having a school nearby**` and the `**ranking of the school**` would raise sales prices of homes. It was hypothesized that houses with a school within a 5 mile radius would have higher sales prices than those that don't. Also, houses with higher ranked schools hypothetically would sell for higher prices.
![Schools](Images/pexels-mihai-vlasceanu-1386484.jpg "Schools")


### Factor 3
---
The third factor researched was the installation of `**solar panels**`. As Colorado is dubbed the state with ***"300 Days of Sunshine"***, we wanted to see if people valued having solar panels pre-installed on their homes. Unsure of the actual correlations and the mechanisms of real estate, we treaded lightly with our hypothesis houses with solar panels would be valued more than those without.
![Solar](Images/pexels-pixabay-356036.jpg "Solar")

### Methodology
---
This housing sales data was provided through a group member's `Personal API` used for their work in real life. We had to settle on just 2021 due to time constraints and to prevent server crashes when trying to consolodate the data at once due to the vast size. It was then filtered through the `Google Geocoding API` where the address was used to extrapolate the longitude and latitude for each property. Afterwards, the long,lat values were used to parse the `Walk Score API` and the `School Digger API`, and cross-examine the `Pikes Peak Regional Building's Solar Panel Licensing Data` to extract for each home:
- Walk Score
- Nearest High School
- High School Ranking
- Nearest Middle School
- Middle School Ranking
- Nearest Elementary School
- Elementary School Ranking
- Solar Panels Installed: True/False

> During analysis, it was shown that of the 4400 properties, only one home had solar panels installed. Due to the extremely limited data-set, analysis was deemed moot, as any findings could not be proven significant without additional data.
