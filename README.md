# MICROSOFT NEW MOVIE STUDIO PROJECT

### OVERVIEW

#### BACKGROUND OF THE BUSINESS

Microsoft is an American multinational technology corporation with the headquarter in Redmond, Washington. Microsoft was founded by Bill Gates and Paul Allen on April 4, 1975. It is the leading developer of personal-computer software systems and applications. Microsoft's best-known software products are the Windows line of operating systems, the Microsoft 365 suite of productivity applications, and the Internet Explorer and Edge web browsers.

#### DOMAIN OF THE BUSINESS

Microsoft generates revenue by developing, licensing, and supporting a wide range of software products and services, by designing and selling hardware, and by delivering relevant online advertising to a global customer audience. In addition to selling individual products and services, they offer suites of products and services. Their products include operating systems for personal computers ("PCs"), servers, phones, and other intelligent devices; server applications for distributed computing environments; productivity applications; business solution applications; desktop and server management tools; software development tools and many more.

#### BUSINESS CASE

Microsoft aims to leverage data-driven insights to understand the current trends and preferences in the film industry.

### BUSINESS UNDERSTANDING

In today's entertainment industry, original video content creation has become a lucrative endeavour for tech giants like Netflix, Apple with Apple TV and others alike. Original content creation involves the following steps:

* Market Research
* Content Development
* Production
* Post Production
* Distribution
* Market Promotion

This project seeks to cover the first step **Market Research**. When thinking about starting up a studio or production company, to be successful, it is important to know which films are most viewed, to keep up with the trend and always sell your product (in this case, films). This is what my analysis aims to investigate.  

#### Objectives  

* Analyze Box Office Performance: Conduct an EDA on box office performance data to identify the most successful films in recent years.  

* Studio Performance: Examine highest performing studio and figure out why.  

* Genre Analysis: Examine the relationship between movie genres and success to determine which combinations resonate best with audiences.  

## DATA UNDERSTANDING

### The Data


* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMDB](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [The Numbers](https://www.the-numbers.com/)

Because it was collected from various locations, the different files have different formats. Some are compressed CSV (comma-separated values) or TSV (tab-separated values) files that can be opened using spreadsheet software or `pd.read_csv`, while the data from IMDB is located in a SQLite database.

Box Office Mojo Data contains about the title of the movie, the studio that made the movie, the gross income from the movie both domestic and foreign and the year the movie was made. The latest data is from 2018.  

Rotten Tomatoes Page Data provided two files one contained data on synopsis of the movie, rating of the movie, genre, writer, director, theatre date- the date it was in theatres, DVD date- the date it came out as a DVD, currency-the currency the box office column is in, box office- amount of money it sold for, run time- how long the movie takes and studio that produced the movie. The other had reviews of some movies, with the critics and publisher and date published.  

The MovieDB Page provided data that contained data on the genre ids, language the movie is in, title of the movie, popularity, release date, vote count and vote average of the movie, the genre ids are a bit ambiguous.  

The Numbers Page provided data that contained release date, movie, production budget, domestic gross and worldwide combined gross for each movie.   

Finally, the SQL data base shown below from IMBD Page

![movie data erd](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-1-project-v2-4/master/movie_data_erd.jpeg)

The above diagram shows ONLY the IMDB data.

### VISUALIZATIONS 

These visualizations seek to explain the conclusions of each objective

From the first objective there is a chart representing the top 5 movies in general and the top 10 most succesful films from 2015:

![Top 5 movies](C:\Users\Crystal\Documents\Course-Materials\Section-1\Projectimages\Top five movies.png)

![Top 10 most succesful films](C:\Users\Crystal\Documents\Course-Materials\Section-1\Projectimages\Top succesful films from 2015.png) 


From the second objective there is a scatter plot showing the relationship between profit and production budget:

![Profit Vs Production Budget](C:\Users\Crystal\Documents\Course-Materials\Section-1\Projectimages\Production budget Vs Profit.png)  

From the third and last objective there are other bar charts representing the genres count and the genres with highest votes respectively:

![Genre Counts](C:\Users\Crystal\Documents\Course-Materials\Section-1\Projectimages\Genre Counts.png)

![Genre Number Of Votes](C:\Users\Crystal\Documents\Course-Materials\Section-1\Projectimages\Genre Number Of votes.png)


## CONCLUSION  

As you start the new movie studio from the analysis of the most successful film, The Avengers film is a good example of film to look at, with a bit of research I found that the storyline was what captivated the audience, and also after that the movies from that one, were also successful which we also saw in the Star Wars film. I would suggest once a film you produce is successful, consider producing another film related to the first one if possible.  

From the analysis of the most successful studio and why it was successful I recommend producing as many movies as possible but also on the production budget, allocate enough money for the production of the film. As seen the production budget correlates highly with the profit made more than the number of movies made correlates with the total gross income. Focus on what is more important and here it is the production.  

From the analysis of genre, focus on movies with the genre type Drama, Action, Comedy as seen these were the best three genres and also the most produced

To conclude I leave a quote, “TO BE A FILMMAKER, YOU HAVE TO LEAD. YOU HAVE TO BE PSYCHOTIC IN YOUR DESIRE TO DO SOMETHING. PEOPLE ALWAYS LIKE THE EASY ROUTE. YOU HAVE TO PUSH VERY HARD TO GET SOMETHING UNUSUAL, SOMETHING DIFFERENT.”
- Danny Boyle