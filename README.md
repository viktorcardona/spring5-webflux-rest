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
    Update One Category: (However if not exist then the category is created)
        curl -v -X PUT \
          http://localhost:8080/api/v1/categories/Id-X \
          -H 'Content-Type: application/json' \
          -d '{
            "description": "Fruits Id-X"
        }'
        
    List All Vendors:
        curl -X GET --header 'Accept: application/json' 'http://localhost:8080/api/v1/vendors'
    List One Vendor:
        curl -X GET --header 'Accept: application/json' 'http://localhost:8080/api/v1/vendors/{id}'
    Create Vendor:
        curl -v -X POST \
          http://localhost:8080/api/v1/vendors \
          -H 'Content-Type: application/json' \
          -d '{
            "firstName": "Michael",
            "lastName": "Jackson"
        }'
    
    Update Vendor:
        curl -v -X PUT \
          http://localhost:8080/api/v1/vendors/5b02bcfcc30f180a1d55a37f \
          -H 'Content-Type: application/json' \
          -d '{
            "firstName": "Michael",
            "lastName": "Jackson 5"
        }'
     
        
    