## IITM Tools in Data Science Project 1 - Hyderabad 50

### 1. Scraping mechanism <a href="https://github.com/Rajalakshmi12/IITM_Tds_Project1/blob/main/TDS-Project1.ipynb">(Colab)</a>

I scraped the data from the Github site using the github API with a personal access token <br>
             GITHUB_TOKEN =  'personal-token' <br>
             HEADERS = {'Authorization': f"token {GITHUB_TOKEN}", <br>
                        "Accept": "application/vnd.github.v3+json" <br>
             } <br>
      
USERS: https://api.github.com/search/users?q=location:Hyderabad+followers:>50&per_page=100&page={cur_page}

REPOSITORIES: https://api.github.com/users/{cur_user}/repos?per_page=100&page={current_page}

response = requests.get(<above-url>, headers=HEADERS)

   <p align="left">
<ul>

### 2. Some facts discovered from the analysis:

  <li>   Top 3 public repo contributors are working for <a href="https://github.com/Rajalakshmi12/IITM_Tds_Project1/blob/main/users.csv">
              Apple, MMTechSoft & Stealth Startup   </a>

</li>
          <li>    They had most of the contributions in Javascript, Java, Scala and HTML in this order
</li>
          <li>    Github Users from Hyderabad working in Google, did not have a single repository published
</li>
</ul>
</p>
      
![Logo](Project-1-Findings.jpg)

### 3. An actionable recommendation for developers based on your analysis:
#### Importance of README

#### Quick summary of the Analysis:
1. Connected to the Github API to get the README.md content using the repository name
2. The resultant JSON has a field called 'content' to fetch the readme content from the respective repository
3. Added two new fields called as 'Images' and 'Word count of the readme'
4. Finding correlation between the presence of images/links vs the stargazers count



