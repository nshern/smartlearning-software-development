# 1. Microservices at a glance

## Definition
> *"A **microservice** is a service with one, and only one, very narrowly focused capability that a remote API exposes to the rest of the system.*"

## Characterictics
- [A microservice is responsible for a single capability.](#responsible-for-a-single-capability)
- A microservice is individually deployable.
- A microservice consists of one or more processes.
- A microservice owns its own data store.
- A small team can maintain a few handfuls of microservices.  A microservice is replaceable.

## Microservices can be different languages
- don't need to be written in the same programming language as the one it collaborates with
  - they just need to know *how* to collaborate with one another e.g.
    - [[queues]]
    - [[service bus]]
    - [[gRPC]]
    - GraphQL
    - HTTP (most often)

## Microservices as an architectural style
  - an entire system consisting of many microservices
  - lightweight form of [[service-oriented architecture]]
  - distributed system with a (probably) large number of collaborating microservices
  - offer a number of potential benefits over both more trad. SOA approaches and [[monolithic]] architectures
  - When done well are
    - malleable
    - scalable
    - robust
  - allow for systems that do well on these four key metrics[^1] 
    - Deployment frequency
    - Lead time for changes
    - Time to restore service
    - Change failure rate

## Responsible for a single capability
- A microservice is responsible for one and only one capability in the overall system e.g.:
  - A microservice has a single responsibility
  - That responsibility is for a capability
- single responsibility principle has been stated in several ways e.g.
  - > "A class should only have one reason to change"




[^1]: __:
- Nicole Forsgren, Gene Kim, and Jez Humble. Accelerate. IT Revolution Press: 2018.
- Nicole Forsgren, Dustin Smith, Jez Humble, and Jessie Frazelle, “Accelerate: State of DevOps 2018,” https://inthecloud.withgoogle.com/state-of-devops-18/dl-cd.html
