- key
    - **GOOD**: Teachable with practial and theoretical experince
    - **THEORY-ONLY**: Would be difficult to demo/incorpate into projects in a pratical way. 
    - **ADVANCED-CONCEPT**: Something I think is difficult. Doable but requires signicant time.
    - **RABBIT-HOLE**: A topic that could be huge if not narrowed to specfics. Needs a key objective 
    - **HAVE-NOT-USED**: A topic that I do not have practical experience using
    - **CLARIFICATION**: Needs more information for me to make a decision

1. Java ( all java basics )
    - GOOD
2. OOP
    - GOOD
3. Design Patterns – Gang of 4, SOLID
    - RABBIT-HOLE
4. Spring
    - GOOD
5. Spring boot
    - GOOD
6. Gradle and maven build tools
    - GOOD
    - I think it would be confusing to use both. They do they same thing.
    - I personally prefer Gradle.
7. Intelij idea
    - GOOD
8. How to use conduct good code quality practices using Intelij such as code formatting, SONAR, Refactoring, etc.
    - CLARIFICATION
        - If they just want proper naming conventions and shortcuts in intelliJ that should come naturally
9. Mysql and mongo – Basics and capable to write basic to medium complex queries
    - GOOD
10. Data JPA
    - GOOD
11. Unit Testing / Integration testing using - junit, **spock** and spring framework
    - GOOD
    - Spock and JUnit are both testing frameworks. Using both is a bit redundant. I think we should push to drop spock. 
12. Swagger/OpenAPI – Handwritting Swagger contracts
    - GOOD
13. TDD and BDD Testing concepts
    1. TDD
        - GOOD
    2. BDD
        - THEORY-ONLY
14. Git & Trunk based development
    - GOOD
15. Java streams - advanced knowledge
    - GOOD
16. Introduction to Redis & Caching
    - HAVE-NOT-USED
    - THEORY-ONLY
17. Oauth and JWT
    1. jwt 
        - GOOD
    2. Oauth
        - THEORY-ONLY
18. Rest / HTTP concepts
    - GOOD
19. Servlets
    - replace with Javalin please
    - Or even directly into spring boot
    - Servlets is a massive pain point in many curricula
20. MVC
    - CLARIFICATION: without html there is no "view" in this design pattern
        - I feel like teaching it would just be confusing
21. Multithreading
    - THEORY-ONLY
        - I feel I would have a hard tim incorporating multithreading in a useful way
        - Most frameworks do that per request under the hood
22. Rx Java
    - HAVE-NOT-USED
    - RABBIT-HOLE
        - The basics could be shown off and probably incorparated in a project
        - But this topic can get very advanced
23. Kafka foundation – Good amount of Kafka knowledge so that they can get into advance concepts like Kafka streams at later stage
Hands on how to produce and consume from KAFKA 
    - HAVE-NOT-USED
    - I have been told it is not too difficult
24. AWS cloud basics
    - GOOD
    - RABBIT-HOLE
        - does this include EC2?
        - Security groups?
        - S3?
25. Introduction to serverless computing
    - THEORY-ONLY
    - Can use AWS Lambda for practical
26. Introduction to API Gateway concept
    - THEORY-ONLY
27. Introduction to AWS Lambda
    - GOOD
28. Introduction to Microservices
    - GOOD
29. Docker and kubernetes - basic guide for build and deployment – good understanding of commands to build application using docker and deploy into Kubernetes
    - ADVANCED-CONCEPT
        - It took my node GCP 2 weeks to get decent pratical usage of kubernetes
30. Tooling: Postman
    - GOOD
31. Handson for building a pipeline using Jenkins
    - If this could be replaced with GitHub actions they can get hands on CI and it would save time and be a better experience for them
32. Basics of Agile / as part of project
    - GOOD

## Week Breakdown
rough idea what a curriculum might look like and what I think an acceptable time would be.
### Week 1
- Java
- OOP
- TDD

### Week 2
- SQL
- AWS RDS
- AWS basics

### Week 3
- API Design with OpenAPI
- HTTP
- Functional programming
- Streams
- Javalin, please Javalin not servlets

### Week 4
- RxJava
- Kafka

### Week 5
- NoSQL/Mongo
- AWS lambda
- Microservices

### Week 6
- Jenkins/GitHub Actions
- Agile
- Spring

### Week 7
- Docker
- Kubernetes