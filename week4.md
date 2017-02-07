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
 - dal (data access layout)
 - domain
 - **service** (all your business logics tend to reside) -- in Homework4
 - util (things that don't have the good home tend to go in here)
 - app specifics
 - **client** (something that needs to interact with)
```
## How the World Communicates
```markdown
__Web Service__
Web service is any piece of software that makes itself avaiable over the internet
```
