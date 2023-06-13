***User: Subscriber***
- As a subscriber I want to sign up/ sign in the website using username and password so that I can subscribe one of the clubs.
- As a subscriber I want to subscribe in horses club/Self defense sport so that I can pay after the confirmation from the club.
- As a subscriber I can see view profile details. 
- As a subscriber I want to view my schedule in the club.
- As a subscriber I want to  check my reviews.
- As a subscriber I can join a tournaments in the club so that I can compete with the others.
- As a subscriber I want to subscribe with a specific package in the club so that I can select from a different packages.
- As a subscriber I want to view the offers in each section.
- As a subscriber I want to make a review in the participating club so that I can evaluate it.

***User:Club***
- As a club I want to sign up/ sign in the website using username and password so that I can add my club to the website.
- As a club owner I can add my club to the website so that the users can join in it.
- As a club I can add trainers to my club.
- As a club I want to check subscribers profiles so that I can ckeck their status.
- As a club I want to arrange a schedule for the subscribers so that they can follow it in their journey.
- As a club I want to publish the tournaments so that the subscribers can join in.
- As a club I want to accept or refuse a join request for the tournaments.

***User:Normal User***
- As a normal user I want to sign up/ sign in the website using username and password so that I can use the feature services in the website.
- As a normal user I want to view the offers in each section.

***

## Project Models:

***

- ***Profile*** 
    - one to one -> User
    - avatar
    - level
    - age
    - city

*- Review* 
    - foreign key -> Club
    - foreign key -> Subscriber
    - title
    - Message content
    - rating

***- Club***
    - Club type
    - Club name
    - description
    - coaches names
    - city 

***- Coach***
 - foreign key -> Club
    - name
    - age
    - expert
    - bio
    - image
    - social accounts

- ***Subscriber***
    - foreign key -> User
    - foreign key -> Club
    - foreign key -> Package 
    - Start date of subscribing
    - End date of subscribing

***- Tournament***
    - foreign key -> Package 
    - foreign key -> Subscriber
    - tournament_name
    - Date
    - winner

***- Package***
    - foreign key -> Club
    - Name
    - Details
    - duration
    - Price

***- Enroll***
    - foreign key -> Club
    - foreign key -> Package
    - is_enrolled
    
***- Payment***
    - foreign key -> Club
    - foreign key -> Subscriber

- ***Contact***
    - foreign key -> User
    - title
    - email
    - message_content

## ***SiteMap***
[SiteMap](https://www.figma.com/file/I2lrDVjZhkQc77MZp7pfAC/Alkhoud?type=design&node-id=0:1&t=rdXVa4vJMcHtjzRR-1)
