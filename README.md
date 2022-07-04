# IMDB_quest

This application scrapes data from IMDB and adjusts IMDB ratings based on the number of ratings recieved and the number of Oscar award won by each movie. With the base settings it is limited to the top 20 movies.

## How to use

You can run the application by calling the individual functions:

-scraper() - Scrapes the top 20 movies from IMDB and returns a pandas DataFrame containing their data.

-review_penalizer() - Subtracts from the ratings of the movies based on the number of reviews they received. The less reviews a movie has, the bigger penalty it gets. Takes a DataFrame as an input and modifies it.

-oscar_calculator() - Increases the rating of a movie for the Oscar awards it received. The more Oscar a movie has won, the bigger bonus it gets. Takes a DataFrame as an input and returns the modified DataFrame

-save_data() - Sorts and saves a DataFrame to a file. Supports .csv, .json and .xlsx file formats. Takes a DataFrame, the desired name and the format of the file, both as strings.
