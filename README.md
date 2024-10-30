**# IITM_Tds_Project1**

1. Scraping mechanism: I scraped the data from the Github site using the github API with a personal access token.
          GITHUB_TOKEN =  '<personal-token>'
          HEADERS = {'Authorization': f"token {GITHUB_TOKEN}",
                     "Accept": "application/vnd.github.v3+json"
          }
   
USERS: "https://api.github.com/search/users?q=location:Hyderabad+followers:>50&per_page=100&page={cur_page}"

REPOSITORIES: "https://api.github.com/users/{cur_user}/repos?per_page=100&page={current_page}"

response = requests.get(<above-url>, headers=HEADERS)

   
2.  Some facts from the analysis:
    * Github Users from Hyderabad with more than 50 followers working in Google , did not have a single repository published
    * Top 3 public repo contributors are working for Apple, MMTechSoft &  Stealth Startup
    * They had most of the contributions in Java, Scala and Javascript in this order
      
3. An actionable recommendation for developers based on your analysis: ?
