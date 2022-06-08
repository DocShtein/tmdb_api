## Project overview
A set of scripts ```search_in_db.py```, ```find_similar.py```, ```make_own_db.py```, ```tmdb_helpers.py```,
```own_db_helpers.py```, ```hello_api_TMDB.py``` is designed to create your own movie database, search for movies, search for similar movies.
The [The Movie Database](https://developers.themoviedb.org/3/getting-started/introduction) service is used to execute the above scripts.

## How to install
* [Register on the TMDB website](https://www.themoviedb.org/signup)
* [Get the TMDB api key](https://www.themoviedb.org/settings/api/request)
* Python3 should be already installed. Then use pip (or pip3, if there is a conflict with Python2) to install dependencies:
```
pip install -r requirements.txt
```

### Script run order
Run the scripts in the following order and follow the instructions on the screen:

1. ```hello_api_TMDB.py```
2. ```make_own_db.py```
3. ```search_in_db.py``` or ```find_similar.py```


## Scripts overview

* ### ```search_in_db.py```
The script searches for movies by keyword in the user database created with the script ```make_own_db.py```

### How to use
Using the terminal, go to the project directory and run the command ```python .\search_in_db.py```


* ### ```find_similar.py```
The script searches the user database created via ```make_own_db.py``` for movies similar to the movie specified by the user.
Search parameters: **genre**, **budget**, **original film language**, **belonging to a specific collection**.
Displays up to eight similar movies.

### How to use
Using the terminal, go to the project directory and run the command ```python .\find_similar.py```.


* ### ```make_own_db.py```
The script creates a custom movie database using The Movie Database service.
Downloads information about films in the amount of one thousand films.

### How to use
Go to the project directory and run the command ```python .\make_own_db.py```.


* ### ```tmdb_helpers.py```
The script makes requests to TMDB service and saves the responses with movies data to a file. 

### How to use
The script does not require a separate launch. Required for scripts to work: ```hello_api_TMDB.py```,  ```make_own_db.py```.


* ### ```own_db_helpers.py```
Opens a file with movie data parsed from the TMDB service for reading.
Does not require a separate launch. Required for scripts: ```search_in_db.py```, ```find_similar.py```.


* ### ```hello_api_TMDB.py```
This is a test script. Allows you to check if your API key is correct, request data (budget) about a particular movie.

### How to use
Run the command ```python .\hello_api_TMDB.py```
