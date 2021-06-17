Repo front M (front api movie Angular):
https://github.com/matthcol/movie_angular 

Repo api M (api rest java spring on movies)
https://github.com/matthcol/movieapijava2021

Repo DB (scripts SQL mysql/mariadb/postgresql for a db movie)
https://github.com/matthcol/dbmovie

-------------  timeline dev -------------------

front M branch devf1 : 
	
	list movies + form to add new movie

DB branch dev1 : table movies

api M branch master : 

	- GET /api/movies
	
	- GET /api/movies/1
	
	- GET /api/movies/byTitle?t=Spectre
	
	- POST /api/movies

api M branches devm2a (4 tests NOK), devm2b (1 test nok), devm2c (ok) :
	
	- GET /api/movies/byTitleYear?t=Spectre&y=2015
	
	- GET	/api/movies/byYearRange?mi=1950&ma=1980
	
	- GET /api/movies/byYearRange?mi=1950
	
	- GET /api/movies/byYearRange?ma=1980
	
	- PUT /api/movies
	
	- DELETE /api/movies/1
	
DB branch dev2 : table stars

api M branch dev3a (tests nok), dev3b (tests ok) : new features /api/stars

	- GET /api/artists
	
	- GET /api/artists/1
	
	- GET /api/artists?n=Eastwood
	
	- POST /api/artists

DB branch dev3 : column id_director

api M branch ? : new features to handle director (no push here)

DB branch dev4 : table play

api M branch devm4a : new features to handle actors
	- GET /api/artists/1  (now give actors and directors)
	- PUT /api/movies/director?mid=1&did=3
	- PUT /api/movies/actors?mid=1
