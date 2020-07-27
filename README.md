# Objective

- Verify the understanding skill of the candidate
- How well the code is written and organised
- What all modern libraries, standards and guidelines was used during coding

# Task

Create a Restful API in Node JS using Express package which should read data from [HackerNews](https://news.ycombinator.com/) and should return as Json
The api should have following features -
1. API1 (public)-> Register -> Register new user using username & password field. Store password as hashed
1. API2 (public)-> Login -> Login using username & password and return access token & refresh token. Access token should have expiry time of 1 minute while refresh token should have expiry time of 30 minutes. 
1. API3 (public) -> seed api - This api should call official site of [HackerNews](https://news.ycombinator.com/), should parse its HTML table and should store them in database. It should store title, website, author, points, timestamp, comments.
1. API4 (protected) -> List api -> It should return all the news with pagination option
1. API5 (protected) -> Create -> It should allow creating new news with fields title, website, author (logged in username), timestamp (created date time)
1. API6 (protected) -> RenewToken -> Renew token should take accessToken & refreshToken as an input and return new accessToken
1. API7 (protected) -> Upvote -> Whenever a user upvotes a news the point value of it should get increased by 1. A user can upvote only once. There is no downvote.
  
## Things to keep in mind
1. Strict naming convention to be followed for defining REST api endpoints
1. API should return correc HTTP status code as defined by REST standards & HTTP protocol for unauthorised access, invalid input params etc.
1. All validation needs to be taken care properly
1. Code needs to be organised properly so one can identify routers, middleware, helper, envs, services easily.
1. Code should be capable to run on multiple environment and must be production ready
1. Database can be used of any choice. No restriction on that.
1. Use ES syntax is suggested
1. Maintain proper readme file with instruction how api works, how it could be deployed and how it could be run locally
1. Logging should be maintained meaningful

# Earn more scores by

- Use of Swagger for API document
- Create Docker container for easy run of project
- Share cloud formation template for easy creation of Infrastructure on AWS
- Use typescript throughout the code structure
- Use of dedicated logger
