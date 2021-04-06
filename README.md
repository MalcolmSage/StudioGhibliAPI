# Studio Ghibli API

##### Used: 
* express
* javascript
* mongoose
* heroku
* mongo atlas
##### Information source: https://ghibliapi.herokuapp.com/#
### End Point: 
`http://sei41-sgfilms.herokuapp.com/films`
## GET
### This will retrieve every object within the films category.
`$ http get http://sei41-sgfilms.herokuapp.com/films`


## POST
### This will allow you to create a new film.
#### Template: `$ http POST http://sei41-sgfilms.herokuapp.com/films/title="<title>" description="<description>" director="<director>" release_date="release_date"`
#### Example: `$ http POST http://sei41-sgfilms.herokuapp.com/films/ title="The Test" description="A film to test the system" director="Malcolm Sage" release_date=2000`
##### Expected result: 
```
{
    "description": "A film to test the system",
    "director": "Malcolm Sage",
    "release_date": 2000,
    "title": "The Test"
}

```

## PUT
### This will allow you to edit a film.
#### Template: `$ http PUT http://sei41-sgfilms.herokuapp.com/films/<_id> title="<title>" description="<description>" director="<director>" release_date="release_date"`

## DELETE
### This will allow you to delete a film.
#### Template: `$ http DELETE http://sei41-sgfilms.herokuapp.com/films/<_id>`
##### Expected result: 
```
{
    "ok": true
}
```
