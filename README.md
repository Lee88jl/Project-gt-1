# Project-gt-1

Sound Data: The Pursuit of the Ideal Song

Miodrag Radovic, Sea Gun Lee, Ershad Ziaei, Priscila Briggs

------------------------------------------------------------------------------------------

Overview:

With this project, we set out to answer three questions:
    (1) What makes a popular song a popular song?
    (2) How have the characteristics of songs changed over time?
    (3) Which artists exemplify each decade?*

*We were able to successfully answer the first two questions, but the search for the third one proved fruitless. With this question, we wanted to further understand how certain characteristics translated over to song popularity, but we ended up being able to gain this insight by delving deeper into the correlation between a song's popularity and its characteristics. Further analysis of this sort over time periods gave us an even firmer understanding of the importance of certain characteristics in songs.

We used a dataset of more than 175,000 songs taken from the Spotify Web API by Baptiste Mansire. The dataset was clean and composed of 19 columns, of which 13 were musical characteristics of songs. We decided not to analyze Key and Mode because of insufficient info from the author on which number correlated to which musical key, thus making that analysis difficult.

Our analysis begins with "Song Popularity Analysis," tasked with answering the first question. First, we placed each song into a "popularity bin" between 1 - 10. Since each song has a popularity score between 0 - 100, this binning would make it possible for us to effectively group each song by popularity. After that, we looked at the average score of each variable tested by popularity bin. For example, while testing Tempo, we found the average tempo score for each of the ten popularity bins and then analyzed any trends. The creation of line graphs for each variable helped us to analyze trends more effectively. We found that seven variables had noticeable trends that affected popularity: Tempo, Loudness, Instrumentalness, Acousticness, Danceability, Energy, and Liveness. We also found that whether a song was explicit or not seemed to have somewhat of an impact on song popularity. For that variable, we figured out the percentage of explicit songs per popularity bin and saw a positive correlation between the two.

Then we go to "Decade Analysis" where we analyze our second question. Similar to our binning in "Song Popularity Analysis," we categorize songs into decade bins according to when a song is from. Next, we looked at the average score of each variable tested by decade bin, just as we did in "Song Popularity Analysis." After graphing each variable over time, we were able to see trends for certain characteristics. Instrumentalness, Liveness, Loudness, Acousticness, Energy, and Tempo had noticeable correlations, while Speechiness, Duration, Danceability, and Explicitness had polynomial trends. Furthermore, we compared trend lines for each variable based on song popularity and decade. We were able to see for a couple of them that the decade trend line almost mimicked the popularity trend line. This begs to ask the question: do we dislike music that sounds old, or do the current trends dictate what we listen to?

As we discovered the variable trend versus the popularity of songs, we wanted to dive deeper into discovering what the critical factors are that could affect the popularity of songs or are visible characteristics of popular songs.  To find the correlation and depth between variables and popularity, we chose to use a heat map chart. We ran the analysis on four different aspects: the entire song list, 10% of each decade (following 10% sample rule, not exceeding 1,000 for each category), top three songs of the decade, and song popularity with a score over 30. The last category was chosen as songs with a popularity of over 30 are more likely to be recommended to playlists and charts, giving it access to more visibility and popularity. After running these analyses, we have found that there are five variables that showed strong correlations with popularity of songs, stated in parenthesis: Acousticness (-), Energy (+), Instrumentalness (-), Loudness (+), and Explicitness (+).  To confirm this finding, we have categorized all the songs by popularity range and calculated the means, getting the same result. With the popular songs variables verified, we matched it to the popular genres of the recent decade. Based on research, popular genres recently are Hip-Hop/Rap, Techno, R&B, Punk, and Alternative Rock (ranked in order from highest to lowest). This result correlates with our findings of what kind of songs catch people’s ears: electronic, energetic, more vocal, louder, and somewhat explicit and catchy lyrics.

------------------------------------------------------------------------------------------

Dataset used:
https://data.world/babarory/spotify-dataset-1921-2020 (containing more than 175,000 songs, from 1921-2020, collected by Baptiste Mansire from Spotify Web API)


Additional Resources:
https://www.tutorialspoint.com/how-to-add-a-second-x-axis-in-matplotlib (for plotting double line graphs with dual x-axes)

https://stackoverflow.com/questions/5484922/secondary-axis-with-twinx-how-to-add-to-legend (for adding legends to line graphs with dual x-axes)

https://towardsdatascience.com/is-my-spotify-music-boring-an-analysis-involving-music-data-and-machine-learning-47550ae931de (for help with music definitions)

https://blog.prosoundeffects.com/understanding-loudness-and-why-it-matters#:~:text=Loudness%20is%20a%20subjective%20term,%E2%80%9D%20(Merriam%2DWebster). (for help with "loudness" definition)
