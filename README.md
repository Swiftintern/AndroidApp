# Internhip AndroidApp
Apply to various Internship through app.

## Pages/Views ##
- Register/Login Page for Students(preferebly through linkedin)
- Home page to show and search internship.
- Internship Opportunity details page to apply to internhsip, show info and company profile.
- Student Profile Page to show its profile info and update info
- Student Applications status
- Student Messages received
 
## API Request URL ##
### Fetching and searching Opportunity ###
GET Request parameter
- query (text, the keyword to search)
- location (text, the place to search eg. delhi)
- limit (number, the number of results per page)
- page (number. pagination based on limit per page)
```
http://swiftintern.com/home.json
```
For fetching top 10 internship just make an empty get request to above URL

### Fetching Photo ###
```
http://swiftintern.com/thumbnails/{opportunity_id}
```

### Fetching Internship Details ###
```
http://swiftintern.com/internship/opportunity/{opportunity_id}.json
```
