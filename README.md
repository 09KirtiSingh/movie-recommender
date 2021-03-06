# MOVIE RECOMMENDER

### Overview
- [About The Project](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#about-the-project)
  - [Salient Features](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#salient-features)
  - [Algorithms Used](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#algorithms-used)
  - [Compatible Platforms](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#compatible-platforms)
  - [Built With](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#built-with)

- [Agile Methodology](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#agile-methodology)
  - [About Agile](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#about-agile)
  - [How I incorporated Agile Methodology during the development cycle](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#how-i-incorporated-agile-methodology-during-the-development-cycle)

- [Getting Started](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#getting-started)
   - [How to get the API key](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#how-to-get-the-api-key)
   - [How to run the project](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#how-to-run-the-project)

- [Navigating Through The App](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#navigating-through-the-app) 
   - [Home Window](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#home-window)
   - [Recommendation Window](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#recommendation-window)

- [Resources Used](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#resources-used)
   - [Datasets](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#datasets)
   - [Tutorials](https://github.com/09KirtiSingh/movie-recommender/edit/main/README.md#tutorials)

### About The Project
- Movie Recommender project is built during Microsoft Engage 2022 program.
- This application provides recommended movies based on the movie entered by the user.
- All the details of the requested movie such as overview, genre, release date, rating, runtime, top cast, reviews, are provided.

#### Salient Features:
- The users' requested movie is searched effectively and the autocomplete feature helps to find the movie easily.
- The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API,
- Reviews are fetched by web scraping in the IMDB site using `beautifulsoup4` and sentiment analysis is performed on those reviews.
- Recommended movies can further be explored.

#### Algorithms Used:
- KNN - Uses K-Nearest Neighbour algorithm and Levenshtein Distances for movie recommendation.
- Content Based Filtering - Uses to recommend movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.
- Searching Algorithm - Uses to search the movie requested by the user.

#### Compatible Platforms:
Laptops, Desktops, Mobiles and Tablet PCs

#### Built With:
![Python](https://img.shields.io/badge/Python-3.8-blueviolet)

![Framework](https://img.shields.io/badge/Framework-Flask-red)

![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)

![API](https://img.shields.io/badge/API-TMDB-fcba03)

### Agile Methodology
#### About Agile:
Agile is a development methodology adopted today in the software industry. Agile promotes teamwork, flexible procedures, and organizing teams.

####  How I incorporated Agile Methodology during the development cycle: 
SCRUM is a subset of Agile, a framework for developing software. SCRUM takes advantage of different techniques to achieve goals in Agile. It promotes an iterative model where the planning is performed on a very short term. The basic time working unit is the sprint. SCRUM teams always reason in sprints and their planning is limited to sprints.

- Sprint 1 (04 May): Project Decision, Sprint Planning, Research - Researching about various movie recommender engines, how famous movie streaming sites use searching, sorting, filtering to recommend movies. After finalizing Python and its framework to execute the project, I searched for tutorials that helped me in the build of my project.

- Sprint 2 (12 May): Software development, design and debugging - Started the development process by taking help from YouTube tutorials. Built a web application using Python and Flask framework for the first time, implemented necessary searching-sorting algorithms, and movie filtering techniques. Worked on the front-end and API calls to make the prototype functioning. Encountered occasional bugs which I debugged timely.

- Sprint 3 (22 May): Adapting the surprise feature, debugging and adding additional features - Decided to implement some surprise and exciting features. Added some additional features - the movie cast details, ratings in the recommended movies, features in the recommended movies.

### Getting Started

####  How to get the API key:
Create an account in https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your `API` sidebar once your request is approved.

####  How to run the project:
1. Clone this repository in your local system.
2. Install all the libraries mentioned in the `requirements.txt` file with the command `pip install -r requirements.txt`.
3. Replace `my_api_key` in the line 22 and 42 in `static/recommend.js` file with the api key generated by you.
4. Open your terminal/command prompt from your project directory and run the `main.py` file by executing the command `python main.py`. 
5. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
6. Voila! You're good to go now.
> Note: If you are unable to run the application, you first need to create and activate a virtual environment, by running:
`py -m venv env`
`.\env\Scripts\activate`

### Navigating Through The App 

#### Home Window:

![](static/home.JPG)
Home window prompts a greeting dialog box.

![](static/home2.JPG)
![](static/search.JPG)
A search bar is displayed to search the movie.

#### Recommendation Window:

![](static/recommend.JPG)
After the movie is searched, it is displayed on the screen. All the details of the movie is also showm.

![](static/cast.png)
The details of the cast of the requested movie is displayed. The user can hover over the cast to know more about them.

![](static/sentiments.JPG)
User reviews and sentiments based on the  movie are displayed.

![](static/recom.png)
After scrolling down, all the recommended movies are layed out based on the searched movie's ratings, genre, etc.
The user can click any of the recommended movie to see all the details, movie-cast, reviews, and more recommended movies.

### Resources Used
####  Datasets:
- [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
- [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
- [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
- [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
- [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

#### Tutorials:
- [Flask](https://youtu.be/4L_xAWDRs7w?list=PLZoTAELRMXVPBaLN3e-uoVRR9hlRFRfUc)
- [Movie Recommendation System](https://youtu.be/A_78fGgQMjM)
- [Python Movie Recommendation System](https://youtu.be/R64Lh1Qwl_0?list=PLZoTAELRMXVN7QGpcuN-Vg35Hgjp3htvi)
