# This repository contains Sleep and Psychological Effects using KNN Supervised

# Description

This dataset has downloaded at kaggle in this link (https://www.kaggle.com/datasets/hanaksoy/reading-habits-and-mood-impact-dataset)
which hase these column:


1. User ID: Unique identifier for each participant.
2. Age: Age of the participant.
3. Gender: Gender of the participant (f for female, m for male).
4. Favorite Book Genre: The genre of books most enjoyed by the participant (e.g., Fiction, Fantasy, Science).
5. Weekly Reading Time (hours): Average number of hours spent reading per week.
6. Mood Impact: Reported impact on mood after reading (Positive, Neutral, Negative).

# Summary
1. Im using KNN to make this, first we check the data, check if they have null value, from df.info we can see that many object data type, these mean we need to change it into number (Encode)first before we do KNN.
If you see the result of df.info we can conclude that gender, favorite_book_genre and mood_impact have object dtype... this will be encoded later
![Image](https://github.com/user-attachments/assets/c19d6895-39db-4acd-86ef-af644770f0f1)
2. First im encoding the Favorite_Book Genre, this has 7 different genre so it will make 7 column here i use One Hot Encoding and this methode works by adding more column with 0 and 1 value. Why i use this... well One Hot Encoding is to encode some categories that arent ordinal.. i mean the different is not related, like maybe you ever know categories like low, medium, high, those are ordinal, because they have their own mean.
3. Then for gender and Mood_Impact i use Label Encoder because it is ordinal, if you see Gender column they have 0 and 1 value meaning male and female, same thing with mood impact which have positive, neutral and negative
4. After that we can do the KNN, split the data and make the model... in this time i also learn how try except work... i mean i already knownn these before but i havent used it. The hard one here i think when i goes to mapping Books_Genre i need to always look back to the .csv
5. After that we put the new data and calculate it
6. Then we predict it if the output 2 its mean positive, if 1 is neutral else negative, this number are same from label encoder









