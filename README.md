# Internship AndroidApp
Apply to various Internship through app.

## Pages/Views ##
- Register/Login Page for Students(through linkedin)
- Home page to show and search internship.
- Internship Opportunity details page to apply to internhsip, show info and company profile.
- Student Profile Page to show its profile info and update info
- Student Applications status
- Student Messages received
 
## API Request URL ##
### Register/Login ###
POST Request parameter
- email
- name
- phone
- city
```
http://swiftintern.com/app/student.json
```

### Get Complete Profile(after login) ###
```
http://swiftintern.com/students.json
```


### Update Profile ###
POST Request parameter
- name
- phone
- action = saveUser
```
http://swiftintern.com/students/settings.json
```

### Fetching and Searching College/Company ###
GET Request parameter
- name
- type = institute or company
```
http://swiftintern.com/organizations.json
```


### Adding or Editing Qualification ###
POST Request parameter
- institute(College name to be fetched from other url)
- degree
- major
- gpa
- passing_year
- action = saveQual
```
http://swiftintern.com/students/qualification/{qualification_id}.json
```

### Adding or Editing Work ###
POST Request parameter
- institute(Company name to be fetched from other url)
- duration
- designation
- responsibility
- action = saveWork
```
http://swiftintern.com/students/work/{work_id}.json
```

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

### Fetching Students Profile ###
At the starting of app make a call to Register method to create session then the data will be fetched
```
http://swiftintern.com/students.json
```

### Fetching Students Applications ###
```
http://swiftintern.com/students/applications.json
```

### Fetching Students Messages ###
```
http://swiftintern.com/students/messages.json
```
