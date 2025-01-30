# Next Track Recommender System

This project aims to develop a **Next Track Recommender System** for music streaming platforms, with a focus on predicting the next track in a playlist. By leveraging machine learning models, we aim to enhance the user experience by providing personalized recommendations based on user behavior, track sequences, and genre preferences. The project uses Spotify’s **Million Playlist Dataset**, which includes track names, artist names, album names, and playlist metadata, to train and evaluate multiple models including **K-Nearest Neighbors (KNN)**, **BERT**, **XGBoost**, and **Recurrent Neural Networks (RNN)**.

## Approach

The data preprocessing pipeline involves cleaning text columns like track and artist names, followed by feature engineering to generate embeddings using **TF-IDF**, **BERT**, and **DistilBERT**. Sentiment analysis is applied to capture the emotional tone of the playlists. Models are developed to predict the next track based on various features: **KNN** uses content-based filtering, **BERT** captures semantic context in track names, and **XGBoost** handles numerical and categorical features. The performance is evaluated through **AUC** and cosine similarity scores.

## Key Insights

Exploratory Data Analysis (EDA) reveals trends such as the average number of tracks in popular playlists and dominant genres like Hip-Hop. These insights help refine the models and their predictions. **KNN** was found to work well for smaller datasets, while **BERT** effectively captured the contextual meaning of playlist titles, and **XGBoost** excelled in handling high-dimensional data. The **RNN** model, particularly the **LSTM** variant, showed potential for improving sequence-based predictions, leveraging the dependencies between consecutive tracks in playlists.

## Future Directions

The project demonstrates promising results, but further work can improve the system's accuracy. Incorporating user feedback loops, real-time predictions, and audio features like tempo and rhythm could enhance recommendations. Additionally, analyzing mood-based playlists will provide insights into the connection between music and emotional well-being. This work sets the foundation for more personalized and engaging music recommendation systems on platforms like Spotify.

