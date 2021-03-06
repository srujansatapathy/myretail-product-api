#My Retail
####Service Name: myretail-products-api

---
## GET Product Details
### Description
Build an application that performs the following actions: 
-	Responds to an HTTP GET request at /products/{id} and delivers product data as JSON (where {id} will be a number. 
-	Example product IDs: 15117729, 16483589, 16696652, 16752456, 15643793) 
-	Example response: {"id":13860428,"name":"The Big Lebowski (Blu-ray) (Widescreen)","current_price":{"value": 13.49,"currency_code":"USD"}}
-	Performs an HTTP GET to retrieve the product name from an external API. (For this exercise the data will come from redsky.target.com, but let’s just pretend this is an internal resource hosted by myRetail)  
-	Example: http://redsky.target.com/v2/pdp/tcin/13860428?excludes=taxonomy,price,promotion,bulk_ship,rating_and_review_reviews,rating_and_review_statistics,question_answer_statistics
-	Reads pricing information from a NoSQL data store and combines it with the product id and name from the HTTP request into a single response.  
-	BONUS: Accepts an HTTP PUT request at the same path (/products/{id}), containing a JSON request body similar to the GET response, and updates the product’s price in the data store.  

## HTTP Method
GET

## PUT Product Details
## Description
Updates Product Details in Mongo Database.

## HTTP Method
PUT

## Notes to reviewer

Used BDD and TDD for building the application.
Used lombok framework for builders and models.
used gradle instead of maven as i have been using gradle for while
Used Mongo morphia framework to talk to mongo database


##How to run the application on local
Please check out master branch from github.
Please Right click and run MyretailApplication application.
Please Use any tool like postman or ARC to run the GET and PUT operation
Also Additionally i have created a POST operation which would be useful to create records for GET and PUT operations
Please refer swagger documentation

##Code Quality checks
Ran sonarlint for quality check, could not run veracode due to licesnse issues

##Workspace Setup

-	Please checkout master branch in your favorite editor
-	This code is tested with Java 8 and Intellij
-	set up graddle setting to graddle wrapper if local machiene does not have gradle
-	Right click on MyretailProductApiApplication and click on run to bootstrap the spring boot application

 
 