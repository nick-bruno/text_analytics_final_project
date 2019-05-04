# text_analytics_final_project
### Nick Bruno (nhb3zf), Karan Kant (kk4ze)
The purpose of our project was to take a corpus of 57,650 songs and try to find similarities between songs and artists, as well as compare the sentiment of different artists. We did this in 5 main steps:

1) Created an Ordered Hierarchy of Content Objects (OHCO) that included artist_id, song_id, verse_id, and line_id. So, each artist had songs, each song contained verses, and each verse contained lines. This can be found in "Song_Corpus_OHCO.ipynb".

2) We ran a MALLET analysis on the entire corpus of songs, finding the most frequent song topics. This can be found in "MALLET_Analysis.ipynb", and the subsequent documents that result from this analysis can be found in the "MALLET_Analysis_Files" folder.

3) We compared the cosine similarity of songs between 3 artists. This can be found in "Cosine_Similarity_Comparison_By_Song.ipynb".

4) We compared the cosine similarity of artists. We did this by combining each of the songs into one large text row, and ran our analysis from there to compare the similarity of overall lyrics between artists. This can be found in "Cosine_Similarity_Comparison_By_Artist.ipynb".

5) Lastly, we ran sentiment analysis on our corpus to find the most positive and negative songs, as well as the most positive and negative artists. This can be found in "Sentiment_Analysis.ipynb".


## Folder Structure

The final_code folder includes all our work. The 5 Jupyter notebooks numbered accordingly comprises of our code and analysis. The data folder includes all our original and intermediary CSV files, including the original data (songdata.csv), tokens table ( artist_song_verse_line_OHCO_df_FULL.csv), our artists and song key files named as such and our subset csvs used for Sentiment Analysis. 

The supplemental_code folder includes a notebook that analyzes similarity for songs for for 40 artists. We decided to perform this analysis to show song similarity over a larger corpus, but it is not a part of our main data product as the code is redundant with our other artist and song comparisons.
