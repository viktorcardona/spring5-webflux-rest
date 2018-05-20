[![CircleCI](https://circleci.com/gh/viktorcardona/spring5-webflux-rest.svg?style=svg)](https://circleci.com/gh/viktorcardona/spring5-webflux-rest)

# Spring Framework 5 - RESTFul Interfaces with WebFlux

The source code in this repository comes from the course [Spring Framework 5: Beginner to Guru](https://www.udemy.com/spring-framework-5-beginner-to-guru/?couponCode=GITWEBFLUXREST).


Mongo

    Run tre mongodb docker image
    docker run -p 27017:27017 -d mongo

Rest Services Calls:

    List All Categories:
        curl -X GET --header 'Accept: application/json' 'http://localhost:8080/api/v1/categories'
    List One Category:
        curl -X GET --header 'Accept: application/json' 'http://localhost:8080/api/v1/categories/{id}'
    Create One Category:
        curl -v -X POST \
          http://localhost:8080/api/v1/categories/ \
          -H 'Content-Type: application/json' \
          -d '{
        	"description": "Reactive Java"
        }'
    
    List All Vendors:
        curl -X GET --header 'Accept: application/json' 'http://localhost:8080/api/v1/vendors'
    List One Vendor:
        curl -X GET --header 'Accept: application/json' 'http://localhost:8080/api/v1/vendors/{id}'
        
    