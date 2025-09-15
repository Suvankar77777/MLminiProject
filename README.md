Hobby & Club Recommendation System for University Students
This project presents a data-driven recommendation system designed to suggest new hobbies and clubs to students at SNU based on their existing interests and lifestyle choices. The primary goal is to enrich student life and boost participation in campus clubs by offering personalized recommendations.



📝 Project Overview
SNU's student clubs often face difficulties in attracting and retaining members, which can impact overall student engagement. This project addresses this challenge by utilizing a data-driven approach to connect students with activities that align with their preferences. By analyzing student data, the system generates personalized suggestions, aiming to foster a more vibrant and active campus community.




✨ Key Features

Data-Driven Recommendations: Leverages a student lifestyle dataset to generate relevant suggestions.




Personalized Suggestions: Provides tailored recommendations for each student, moving beyond generic advice.

Co-occurrence Analysis: Identifies relationships between different hobbies, club memberships, music genres, and gaming preferences to inform the recommendations.


Interest Scoring: Each recommendation is assigned a numerical score, indicating the strength of the match for the student's profile.

Data Visualization: Includes visual representations of the most popular interests and their co-occurrence frequencies.

🛠️ Methodology
The system is built using Python with the pandas library for data analysis. The core of the recommendation engine is based on a co-occurrence analysis of student interests.

Data Loading & Inspection: The project uses the miniProjectMLdataset.csv dataset, which contains 111 student entries across 73 columns. An initial inspection was performed to understand data types and check for null values.


Feature Selection: The analysis focuses on key columns related to student interests:


Hobby_top1 


Hobby top2 


Club top1 


Club top 2 


Music Genre Top 1 


Game Genre Top1 

Co-occurrence Calculation: The system calculates the frequency of individual interests and the co-occurrence counts for pairs of interests across different categories. This helps identify which activities are frequently enjoyed together.

Recommendation Generation: For each student, the system generates a set of potential new interests. These suggestions are scored based on how frequently they co-occur with the student's existing hobbies and club memberships. A higher score signifies a stronger recommendation.

📊 Results & Insights
The analysis provided several key insights into the interests of the student community:


Most Popular Interests: "Cricket" and "Music" were identified as the most frequent primary hobbies, with "Bollywood" being the most popular music genre.


Strongest Co-occurrence: The strongest association found was between an interest in "Bollywood" music and membership in the "Sports Club".


Most Influential Interests: "Bollywood" music, the "Sports Club," and the "Coding Club" were the most influential interests, indicating their central role in the student community.


Recommendation Potential: The model successfully generated high-scoring recommendations for students, indicating a strong alignment between their existing lifestyles and the suggested activities.

📈 Visualizations
Top 20 Most Recommended Hobbies and Clubs
This chart displays the frequency of the top 20 most recommended items across all students. "Game Genre Top1: FPS" is the most frequently recommended activity.




3D Scatter Plot of Recommendations
A 3D scatter plot was also generated to visualize the relationship between the top three recommendations for each student, providing a deeper look into the recommendation patterns.

🚀 How to Use
To run this project, follow these steps:

Clone the repository:

Bash

git clone <repository-url>
Install dependencies:

Bash

pip install pandas matplotlib

Navigate to the project directory and ensure the dataset miniProjectMLdataset.csv is present.

Run the Jupyter Notebook:

Bash

jupyter notebook miniProjectML.ipynb
🗂️ Dataset

File: miniProjectMLdataset.csv 

Description: Anonymized data detailing the lifestyle, hobbies, and preferences of 111 university students.

Shape: 111 rows × 73 columns.

📂 Project Structure
.
├── miniProjectML.ipynb         # Main Jupyter Notebook with analysis and recommendation logic.
├── miniProjectMLdataset.csv    # The dataset used for the project.
├── Project Report.pdf          # Detailed project report with findings and conclusions.
└── README.md                   # This file.
🔮 Future Development
The framework established in this project can be enhanced by:

Incorporating more complex machine learning models to improve recommendation accuracy.

Integrating real-time data to provide more dynamic and relevant suggestions.

👥 Contributors

Debasis Mahata - B.Tech in CSE (IoT, Cyber Security & BlockChain Technology) 



Suvankar Paria - B.Tech in CSE (Artificial Intelligence and Machine Learning) 


🙏 Acknowledgments
We extend our sincere gratitude to our mentor, 

Bidyut Saha, Assistant Professor at SNU, for his invaluable guidance and support throughout this project. We also thank the CSE Department for providing the necessary resources.
