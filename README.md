**# IITM_Tds_Project1**

1. Scraping mechanism: I scraped the data from the Github site using the github API with a personal access token.
          GITHUB_TOKEN =  '<personal-token>'
          HEADERS = {'Authorization': f"token {GITHUB_TOKEN}",
                     "Accept": "application/vnd.github.v3+json"
          }
   
USERS: "https://api.github.com/search/users?q=location:Hyderabad+followers:>50&per_page=100&page={cur_page}"

REPOSITORIES: "https://api.github.com/users/{cur_user}/repos?per_page=100&page={current_page}"

   
4.  Most interesting and surprising fact: No repos in Google
5.  An actionable recommendation for developers based on your analysis
