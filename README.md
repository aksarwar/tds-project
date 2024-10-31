# GitHub Users in Toronto

1.Data Scraping Process: Used Python’s requests library to interact with the GitHub API, querying /search/users for Toronto-based developers by location and followers:>100, and gathering detailed profile and repository data using /users/{username} and /users/{username}/repos endpoints.

2.Interesting Finding: Analysis revealed that developers with moderate-length bios (10-20 words) and keywords like "AI" or "Data Science" attract more followers, possibly due to algorithmic boosts or increased community interest.

3.Actionable Recommendation: Developers should create concise bios that highlight key skills or trending fields like "machine learning" and maintain active repositories to improve visibility and attract followers.

# files
1.users.csv: Contains information about 693 GitHub users in Toronto with over 100 followers  

2.repositories.csv: Contains information about 55778 public repositories from these users  

3.fetch.py:The fetch.py file contains a GitHub scraper implemented in Python, which uses a GitHub API token to fetch and process data from GitHub, likely to extract repositories or user data, using libraries such as requests and pandas for handling requests and data manipulation.    

4.project1.ipynb: notebook provides solutions to a series of data analysis questions, using Python and pandas to process and analyze user and repository data from CSV files.

# Data Collection Overview  
Method: Data gathered through the GitHub API  
Collection Date: October 28, 2024  
Criteria: Included only users with over 100 followers  
Repository Limit: Captured up to 500 of the most recently updated repositories for each user  

# Usage  
Setup: Ensure you have a valid GitHub API token to handle authenticated requests and install Python’s requests library to  enable API calls.  

Scripts: First, run get_users_csv.py to generate users.csv, which will include user data like login, bio, followers, and company. Then, execute get_repos_csv.py to create repositories.csv with repository-specific details like stars, language, and license type.  

Data Structure: The dataset contains user information, including location, follower count, bio, and public repository stats, as well as repository details like primary language, license, and stargazer count, enabling a detailed analysis of popularity factors.  

# Analysis Overview  
Follower Patterns: Users with medium-length bios (10-20 words) appear to have higher follower counts, suggesting that bios which balance informativeness with brevity might be more appealing.  

Company Influence: Affiliation with well-known companies tends to correlate with higher follower counts, indicating potential brand influence on a developer’s visibility within the GitHub community.  

Licensing Trends: MIT is the most common open-source license used by Toronto-based developers, with other permissive licenses like Apache and BSD also present. This trend suggests a community preference for sharing and collaboration.  

# Insight & Recommendation  
Insight: Developers using relevant, recognizable industry keywords in their bios are more likely to attract attention, likely because such terms align with common search queries or trends. This finding suggests that aligning bios with popular topics can improve profile visibility.  

Recommendation: Developers should thoughtfully curate their bios, incorporating specific, relevant keywords without overloading on details. Regularly updating repositories and using trending tags in project descriptions or names could further improve search ranking, helping developers grow their follower base organically.
