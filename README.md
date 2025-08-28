# YouTube_Video_Suggestion_Engine_04 CaseCraft Analytics Project 4

## 📺 Overview  
This project simulates a YouTube-style video recommendation engine using metadata and engagement metrics. It builds a synthetic dataset of 500 videos and applies cosine similarity to suggest content with similar performance profiles.

## 🎯 Objective  
To recommend videos based on metadata and viewer engagement—mimicking YouTube’s “Up Next” or “Related Videos” feature without relying on watch history.

## 📊 Dataset & Features  
- 500 synthetic videos  
- Metadata: title, category, tags  
- Metrics: views, likes, duration (sec), engagement score (likes/views × 100)

## 🧪 Feature Engineering  
- Selected features: views, likes, duration, engagement  
- Scaled using `StandardScaler` for cosine similarity  
- Tags combined into string format for display (not embedded)

## 📈 Visual Explorations  
- Histogram: Views distribution  
- Scatterplot: Likes vs Views by category  
- Bar chart: Category frequency  
- Dual-axis chart: Engagement score vs video count by category  
- Histogram: Duration distribution  
- Heatmap: Feature correlations

## 🤖 Recommender Logic  
- Cosine similarity computed across scaled features  
- For a given video, top 5 most similar videos are returned  
- Recommendations span categories, focusing on performance metrics

## 🧠 Key Insights  
1. **Engagement Patterns**: Education and Tech videos show higher average engagement  
2. **Popularity vs Interaction**: Views and likes are strongly correlated; engagement is not  
3. **Duration Trends**: Longer videos are common in Gaming, but don’t guarantee higher engagement  
4. **Recommendation Utility**: Suggests similar-performing videos across categories—useful for creators and platforms  
5. **Limitations**: Tags and titles not semantically embedded; no modeling of time-based engagement or virality

## ✅ Final Conclusion  
This project demonstrates how performance-based features can drive content recommendations in a YouTube-like ecosystem. By leveraging cosine similarity on scaled metrics, it offers a scalable, interpretable engine for surfacing similar videos—ideal for enhancing discovery and creator strategy.

