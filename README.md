# Analysis on RAWG Dataset
###### By Rajkumar K

RAWG is the **largest video game dataset** and game discovery service with 500,000+ games data

## Problem statement
1. Which is the top most rated game for each platform?
2. Which game developer has released most games?
3. Which game genre has most games?
4. Number of  games released per year?
5. Games with longest update time?

## Tech Stack USed
* Pyspark[3.1.2]
* Python[3.8]
* Spark[1.3.2]
* Spark SQL[]
* Git/Github[]

## PySpark Connection
    * Install pyspark, findspark.
    * Download spark and set environmentl variables.
    * Import pyspark,findspark.
    * Create SparkSession.
    * Load data into spark.


## Data Definations
* For all problems we used RAWG games dataset
    eg: 1,dgeneration-hd,D/Generation HD,,2015-10-23,False,2019-09-17T11:58:57,<br>
    http://dgeneration.net,0.0,0,1,80,2,292,0,4,PC||macOS||Xbox One||PlayStation 4||Nintendo Switch,<br>
    West Coast Software,Adventure||Puzzle,West Coast Software,Everyone 10+,4,88,2,2,0,0

#### Column definitions
* id: An unique ID identifying this Game in RAWG Database
* slug: An unique slug identifying this Game in RAWG Database
* name: Name of the game
* metacritic: Rating of the game on Metacritic
* released: The date the game was released
* tba: To be announced state
* updated: The date the game was last updated
* website: Game Website
* rating: Rating rated by RAWG user
* rating_top: Maximum rating
* playtime: Hours needed to complete the game
* achievements_count: Number of achievements in game
* ratings_count: Number of RAWG users who rated the game
* suggestions_count: Number of RAWG users who suggested the game
* game_series_count: Number of games in the series
* reviews_count: Number of RAWG users who reviewed the game
* platforms: Platforms game was released on. Separated by ||
* developers: Game developers. Separated by ||
* genres: Game genres. Separated by ||
* publishers: Game publishers. Separated by ||
* esrb_rating: ESRB ratings
* added_status_yet: Number of RAWG users had the game as "Not played"
* added_status_owned: Number of RAWG users had the game as "Owned"
* added_status_beaten: Number of RAWG users had the game as "Completed"
* added_status_toplay: Number of RAWG users had the game as "To play"
* added_status_dropped: Number of RAWG users had the game as "Played but not beaten"
* added_status_playing: Number of RAWG users had the game as "Playing"

# Data Set Used
* [Data Set](https://api.rawg.io/docs/)
