# Week 4 (02.06.2017)
## Logging
### Why:
```markdown
- Helps troubleshoot
- Better than system print outs
- Provides a consistent format and layout
```
### How:
```markdown
- Use a common logging framework.
- Logback abd SLF4j for now
- Logback framework provides several nice features
- Logback.xml
 *Template of logback file will be posted
```
## Performance Testing (The DIY Approach)
```markdown
The performance testing is the tesing of how effective and responsive your program is.
 - the speed: how responsive/fast your app is
Testing techniques
  - memory and heap utilization
  - the number of effective app
  - application latency 
      (Note: latency means the delay before a transfer of data begins following an instruction 
      for its transfer)
Some software to use for testing
 - JVisualVM
 - JMeter
 - SoapUI
 - RoadRunner
```
## QA Testing (Quality Testing)
```markdown
All and only thing the QA test cares about is does your application works with the exact 
specifications that your client asked? QA tries to simulate what the user does.
```
## Packages
```markdown
An organization of tools for us.
- /src/main/java/plain.java <-- default for plain class
- /src/test/java <-- default for test unit
  - make sure your testing unit is in the same package as your class
- In java, everything is in the concept of package (Default package -- nothing in the package)
- Packages from the code perspective is just the directory structure.
- Base package for an application is defined by YOU (edu.xaviercsci260.'your name')
**Standard Layout**
- Base package
- Default package
- Sub packages ("." exteneded default packages - e.g. src.main.java = java is a sub package of main)
 - config
 - controller
 - dal (data access layers)
 - domain
 - **service** (all your business logics tend to reside) -- in Homework4
 - util (things that don't have the good home tend to go in here)
 - app specifics
 - **client** (something that needs to interact with)
```
## How the World Communicates - Web Service
```markdown
Web service is any piece of software that makes itself avaiable over the internet
Details:
 - Runs over HTTP
 - REST (Representation State Transfer) vs SOAP (Simple Object Access Protocol 
  - JSON (Javascript Object Notation) vs XML ()
 - Synchronous vs Asynchronous
   - Synchronous real-world example is when a teacher give a stack of papers to the person
     in front of the row and pass on to the people in the back
      - easier for debugging
   - Asynchronous: throw a stack of paper and everyone gets the paper at the same time
 - URL based
```
## Anatomy of a service
```markdown
- Controllers
  - No Business logic
- Service
  - Business logic (business logic would be anything that does something to your project besides transitions)
- Domain
  - POJOs
  - Anything that can be reused goes under this sub package
- DAL (Data Access Layers)
  - holds DAO
- DAO (Data Access Objects)
  - How you access data
  - File system access
  - Database access
  - Web service access
```
## Service Oriented vs. Macro Oriented
```markdown
how you construct your applications.
In the end, it does not matter.
__Single Responsibility__
A service should have only one resposibility
__Web Services in Java__
Easiest Way:
Use Spring Boot
```
## Controllers
```markdown
- Holds request methods
- Request Mappings
 - Goes from Root URL/
- Handles call handoff to service layer (no service/business logic in here)
- Only logic:
 - Formatting Request and Response objects
 __Request/Response__
 - HTTP Protocol/Operations
  - CRUD
 - GET, POST, DELETE
  - create, read, update and delete
 - Request parameters get turned into request objects
 - Results of service calls get turned into response objects 
```
