# Car-go - Backend
**Project By:** Isaac Santacruz


## Descripton
"Album" is a website that will help you store where are the places you've travel before so you can send it to your friends and they can see where you've been.
</br>

## Link
[**Github**]()
[**Deployment**]()
</br>

## Technologies Used
- Django
- Postman
- Python
- flask
- neon
</br>

## Backend Endpoints

| ENDPOINT | METHOD | PURPOSE |
|----------|--------|---------|
| /shift | GET | return list of trips|
| /shift/:id | DELETE | delete a trip from database |
| /shift/:id | PUT | receive info & update of  a trip in database |
| /shift | POST | receive info from new form & create new trip in database |
| /shift/:id | GET | render page with trip|
</br>

## ERD

``` 
Diagram
    USER {
        id primaryKey
        username string 
        password string
    }
    USER ||--|{ SHIFTS : Create
    SHIFTS {
        country foreignKey
        city string
        spot  string 
        picture string 
    }
    }
```