## User Segmentation Project

### Overview
This project focuses on segmenting users based on their engagement and activity on a platform, utilizing various data science techniques and machine learning clustering methods. It leverages a dataset containing metrics such as engagement rates, follower counts, and content statistics to identify distinct user groups and derive insights into their behaviors and characteristics.

### Features
The dataset includes the following features:
- `timestamp`: Date and time of the account data extraction.
- `account_id`: Unique identifier for the user account.
- `nickname`: User's nickname on the platform.
- `biography`: User's biography.
- `awg_engagement_rate`: Average engagement rate per post.
- `comment_engagement_rate`: Engagement rate based on comments.
- `like_engagement_rate`: Engagement rate based on likes.
- `bio_link`: URL provided in the user's biography.
- `is_verified`: Whether the account is verified.
- `followers`: Number of followers.
- `following`: Number of accounts the user follows.
- `likes_received`: Total number of likes received.
- `videos_count`: Number of videos posted.

### Installation

To set up the project environment, run the following commands:
```bash
git clone https://github.com/devanshijoshi08/User-Segmentation.git
cd repository-name
pip install -r requirements.txt
```
### Usage
To run the LSTM model training and evaluation, open and run the `User_Segmentation.ipynb`.

### Clustering Process
- **Data Scaling**: Data features are scaled using `RobustScaler` to handle outliers effectively.
- **K-Means Clustering**: `KMeans` clustering is applied to segment users into groups based on their engagement and activity levels.
- **Elbow Method Visualization**: `KElbowVisualizer` from `yellowbrick.cluster` is used to determine the optimal number of clusters.

### Results
- **Cluster Profiles**:
  - **Cluster 0**: Active and Engaged Users
  - **Cluster 1**: Platform Giants
  - **Cluster 2**: Emerging Influencers
  - **Cluster 3**: Established Content Creators
  - **Cluster 4**: Highly Engaged Niche Creators

Each cluster is analyzed for key characteristics such as engagement rates, follower counts, and content statistics. Strategies and recommendations are provided for each user segment to enhance their engagement and growth on the platform.

### Visualizations
The script generates various plots such as:
- **Engagement Distributions**
- **Correlation Matrix of Features**
- **Cluster Summaries**

These visualizations help in understanding the data distribution and the characteristics of each user segment.