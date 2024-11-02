## DataScraping

This repository contains data about GitHub users in Moscow with over 50 followers and their repositories.

This code scrapes user data from the GitHub API based on location and follower count:
Setup: It uses a GitHub API token for authentication to avoid rate limits on requests.
User Data Collection: The fetch_users function retrieves users in a specified city with a minimum follower count, paginating through results and fetching detailed user info.
Repository Data Collection: The fetch_repositories function collects repository details for each user, stopping when there are no more repositories.
Saving Data: The save_users_to_csv and save_repositories_to_csv functions save the collected data into CSV files.
Execution: The main function coordinates fetching users and their repositories, saving the results into separate CSV files, while including a one-second delay between requests to adhere to API rate limits.

Summary of API Endpoints Used
https://api.github.com/search/users for initial user search by location and followers.
https://api.github.com/users/{username} for fetching individual user details.
https://api.github.com/users/{username}/repos for fetching each user’s repository data.
#Data Collection

- Data collected using GitHub API
- Date of collection: 2024-10-29
- Only included users with 50+ followers


## Files

1. `users.csv`: Contains information about 459 GitHub users in Delhi with over 50 followers
2. `repositories.csv`: Contains information about 25411 public repositories from these users
3. `scr.py`: Python script used to collect this data


## intersingObservation

Consider creating high-quality projects in popular languages like JavaScript or Python, as repositories in these languages tend to attract more stars, increasing visibility and followers.

Interestingly, despite Python’s global popularity and ease of use, it wasn’t the top language among developers in Moscow who joined after 2020—JavaScript took the lead instead. This suggests a regional preference for web development skills among newer developers.

If you're a developer in Moscow, especially new to the field, consider focusing on building your JavaScript skills. Its high popularity, particularly among recent GitHub users, could enhance your job prospects and open up more opportunities for collaboration within the local tech community.

Enable wikis and project boards in your repositories to attract more collaborators. These features highlight project planning and documentation, making it easier for others to contribute.
   
