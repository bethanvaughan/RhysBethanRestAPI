# RhysBethanRestAPI
RhysBethanRestAPI

# The Database we will be implementing is a relational database using SQL.

# 3 schemas: 

Person Schema: 

CREATE TABLE person (
    _id serial PRIMARY_KEY,
    name VARCHAR (255),
    age INT
    number_people_household INT
    );
    
House Schema:

CREATE TABLE house (
    _id serial PRIMARY_KEY,
    address VARCHAR (1000),
    owner VARCHAR (255)
    );
      
Address Schema:

CREATE TABLE address (
    _id serial PRIMARY_KEY,
    address VARCHAR (1000),
    postcode VARCHAR (255)
    );
    
    
# REST API requests:

new GET = to send a form to the user so they can then input info. 
create POST = to send the info inputted by the user to create a new Person. 
show GET = to pull the new info and show it for the user. 

# Route list:

app.get('/person/new')= brings back the form for the user to input into. 
app.post('/person/new') = sends the new inputted info to the backend. 
app.get('/house/id') = brings back a house, it's owner and address. 

app.get('/person?address=something&age=something&householdsize=something') = sends specific results to user using queries. 

# Responses returned
A record of the data depending on the query

app.get('/person/new') = 




