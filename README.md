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

**From the first objective there is a chart representing the top 5 movies in general and the top 10 most succesful films from 2015:**

![Top 5 movies](Top five movies.png)  

The movies are almost at the same level but we can see one with a significant difference The Avengers movie, there could be so many factors that pushed this movie to the top  and was the beginning of a series as can be seen Avengers: Age of Ultron follows, followed by Black Panther. The success of the Avengers might have caused a chain reaction of some sort. 

![Top 10 most succesful films](Top succesful films from 2015.png)  

From this we can conclude that the most successful film was the Avengers whether it was a series or a movie adopted from the series character, this type of film looks to resonate best with the majority and had a high gross income.


**From the second objective there is a scatter plot showing the relationship between profit and production budget:**

![Profit Vs Production Budget](Production budget Vs Profit.png)  

Looks like there is correlation between the two,the average production budget and the average profit. 

**From the third and last objective there are other bar charts representing the genres count and the genres with highest votes respectively:**

![Genre Counts](https://github.com/CrystalW123/dsc-phase-1-project-v2-4/assets/141912458/89da4a4c-42db-4241-992a-7d0dd2d2912a)

It looks like the Drama genre appeared the most whether as a stand alone or with other genres, followed by the comedy, then Documentary and also Action genre is a bit high.

![Genre Number of votes](https://github.com/CrystalW123/dsc-phase-1-project-v2-4/assets/141912458/6774af34-0baa-41e6-af51-710fb6ec150a)

From the above the movies with the genre type Drama, Action as part of the overall genre resonate best with the audience. So, it is a good idea to follow this trend, producing movies in this genre.

## CONCLUSION  

As you start the new movie studio from the analysis of the most successful film, The Avengers film is a good example of film to look at, with a bit of research I found that the storyline was what captivated the audience, and also after that the movies from that one movie (in other words the series) were also successful which we also saw in the Star Wars film. I would suggest once a film you produce is successful, consider producing another film related to the first one if possible. People are bound to watch the second one if they enjoyed the first one. Use characters that are known in the cinematic universe and make the movie your own.This will make people more familiar with the characters, creating a huge audience.  

From the analysis of the most successful studio and why it was successful I recommend producing as many movies as possible but also on the production budget, allocate enough money for the production of the film. As seen the production budget correlates highly with the profit made more than the number of movies made correlates with the total gross income. Focus on what is more important and here it is the production.Spend more money on producing the film, paying your crew than the number of films you produce. It is better to watch a film with great background and scenery, good actors and high quality video than many with none of these attributes.  

From the analysis of genre, focus on movies with the genre type Drama, Action, Comedy as seen these were the best three genres and also the most produced,specifically  the Action, Adventure, Sci-Fi combination seems to appear a lot. 

This analysis can be found on the ![student.ipynb file](student.ipynb) and in the ![presentation.pdf.](presentation.pdf) 
If you need to run the code be sure to unzip the zipped file and also the rest of the data is inside the folder.

To conclude I leave two quotes,

“Too often we forget that genius, too, depends upon the data within its reach, that even Archimedes could not have devised Edison’s inventions.”
~ Ernest Dimnet  

"To be a filmaker, you have to lead, you have to be psychotic in your desire to do something. People always like the easy route. You have to push very hard to get something unusual,something different."
~ Danny Boyle
