qcon
====

notes from QCon


What makes a great API
----------------------

### Keys
  A valuable service
  A plan and a business model
  Simple flexible, easily adopted
  Managed and measured
  Great developer support

Each point above has two key sides: Business & Technology

#### Valuable
One of the top three searches on programmable web : weather

- Over half of data written into Salesforce is through api
- Over half of placements in ebay is through their api

#### Planned
Being RESTful is not enough

Blog on Programmableweb - Netflix - "How REST keeps me awake at night"

more than 2/3 of apis support json. 1/2 of those apis support only json

http://groups.google.com/group/api-craft

#### flexible

provides choices
- data format, protocol, version
- control
  - partial queries, updates and batch operations

TTFHW - Time to First Hello World
- Be clear at what you do
- Offer a free/trial version
- Fast/Automated sign up
- Clear/accurate documentation
- Copious code samples. Most developers don't want to write code from scratch.
  - A whole working app. And. A whole working mobile app.
- Provide Tools

#### Manage and Measure

##### Manage
People underestimate the scale of an API project.
One important aspect in managing an api
Versioning
* Path segment - Date /2010-04-01/
* Path segment - Number /1/
* Path segment - v+number /v1/ 
* Query parameter - ?v=2 [Google]
* Custom HTTP header - String - GData-version:2 [Google]
* HTTP accept header - applicaiton/vnd.github[version]
note Google provides support for both query param and header

Security Baseline

Today
- SSL
- OAuth 2

Future:
- SSL [Many apis are moving ssl only]
- Openid Connect [Still early today]

##### Measured
Metrics that matter
- Traffic
  - total calls, top apis, call chains, quota faults
- Developers
  - Total Developers, active, top, trending apps, retention
- Service
  - Performance, Availability, Error rates, Code defects
TODO Missed a couple here
- Business
  - revenue
    - Direct, Indirect

#### Supported
Great developer experience
- Signup, guides, reference, SDK, prociing, clear ToS
Communication and Community
- forum, blog, social media, email, app gallery

References
[developerexperience.org](developerexperience.org)
[developersupport-handbook.appsport.com](developersupport-handbook.appsport.com)

An example of a great api: Stripe [hearing this again and again]


Top 10 worst practices
- refer the slide share
