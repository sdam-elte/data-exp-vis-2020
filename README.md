# Course material for Data Exploration and Visualisation 
### 2020 spring semester

This course is part of the [Scientific Data Analytics and Modelling Programme](http://datascience.elte.hu/en/Default.aspx#top).
The aim of the course is that students gain practical skills to **access large databases/datasets**, to handle **data stored in different formats**, **to explore/distill these data** and **present/visualize** the gathered information. During the course students will come across databases of multiple disciples. Completing of the several projects allows students to gain experience on this field that will be a firm foundation for later courses on theoretical datamining and advanced computing laboratories.
In this course we intend to introduce **state of the art tools and methods** for data exploration and visualization. This field evolves rapidly and a year later one might not use the same tool for the same task, but certain notions, languages and packages become the standard for a longer time.

There is a useful tutorial into python http://bokae.web.elte.hu/numerical_methods.html), which gives a wide background knowledge, that comes handy.

During the course every sample code will be shown in **jupyter notebooks**, which can be accessed on the [Kooplex Edu platform](https://kooplex-edu.elte.hu).

Each occasion starts with an hour of introduction into the current topic with examples. After that everyone can work on the worksheets and the lecturers will be available to help with the any related problems and questions. 

  
#### Course info
Neptun code: 	**dsexplorf17vm** <br>
Instructor: 	**Dávid Visontai**<br>
Semester: 	spring <br>
Type: 	Lecture + Practice <br>
Credit points: 	4 <br>
Prerequisites: 	programming in either **python**, **R** or **matlab** <br>

The course is held in the **North Building** in computer lab **5.56** on **Wednesdays**  **14:00 - 17:00**.


### The schedule of the course 
1,  12.02.2020. **[Introduction to Kooplex Edu](https://kooplex-edu.elte.hu/hub)**, **[Jupyter Notebooks](https://jupyter.org/)** and **[Visualization](Interactive_Visualization)** <br>
2,  19.02.2020. **[SQL queries on an NBA database](Basketball_League-SQL) I** <br>
3,  26.02.2020. **[SQL queries on an NBA database](Basketball_League-SQL) II** <br>
4,  04.03.2020. **[USGS water discharge statistics](USGS-waterdata-curl-pandas)** <br>
5,  11.03.2020. **[REST services](REST-services)** <br>
6,  18.03.2020. **[Following John Snow (shapely)](John_Snow-map)** <br>
7,  25.03.2020. **[Following John Snow (geopandas, folium)](John_Snow)** <br>
8,  01.04.2020. **[Network exploration](Networkx)** - This lecture will be given by [**Dániel Ábel**](http://maven7.com/hu/daniel-abel/), who is a developer at Maven7. <br>
9, 15.04.2020. **[Data extraction from images](ImageExploration)** <br>
10, 22.04.2020. **[Natural Language Processing on tweets](NLP_on_tweets)** - This lecture will be given by **Eszter Bokányi**, whose field of interest is how social phenomena can be captured by using various digital fingerprints of individuals. <br>
11, 29.04.2020. **[3D Visualization](3d_Visualization)** <br>
12, 05.05.2020. **Consultation** <br>
13, 12.05.2020. **Consultation**

### Covered topics

 * Datatypes, images, timeseries, tables, graphs, textual data
 * Standards of file- and dataformats ([csv](https://www.computerhope.com/issues/ch001356.htm), [hdf5](https://en.wikipedia.org/wiki/Hierarchical_Data_Format), [netcdf](https://en.wikipedia.org/wiki/NetCDF))
 * Raw and processed data, metadata, cleansing of data
 * Access data locally and through the web ([API](https://restfulapi.net/)s, [HTTP protocol](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol))
 * Access of scientific databases, Usage of relational databases ([SQL](https://www.w3schools.com/sql/))
 * Transforming data, sorting, combining [pandas](https://pandas.pydata.org/)
 * Basics of timeseries analysis
 * Handling datasets with geolocation ([shapely](https://shapely.readthedocs.io/en/stable/manual.html), [folium](https://python-visualization.github.io/folium/), [geoviews](https://geoviews.org/))
 * Basics of image processing ([opencv](https://opencv.org/))
 * Dimension reduction, clustering
 * Processing textual data, logs ([natural language processing](https://www.nltk.org/))
 * Infographics, visualisation (html, css, javascript libraries)
 * Interactive dataexplorative tools ([ipywidgets](https://ipywidgets.readthedocs.io/), [bokeh](https://bokeh.org/), [holoviews](http://holoviews.org/))
 * Developing open source softwares, reproducible research ([OSF](https://osf.io/))



### Where to work on the assignments?
https://kooplex-edu.elte.hu/hub is where the notebooks will be handed out. It is available for all students with a valid **Neptun** or **caesar** account. Once you run your notebook server you will find a folder with the course material. The notebooks will be available in this Github repository as well.
We will explain how to use this portal on the first lecture.
The Kooplex Edu platform is accessible externally as well. In case there is any problem with the portal you can run a notebook server locally on any other computer and upload your work later.

### Requirements
There will be an assignment for each of the 9 topics, which need to be completed individually. The deadlines for the submissions are shown next to the topic and all related information will be in the topics' folder. These are not strict deadlines, however we advise students to keep them in order to be able to complete all tasks.

The **minimum requirement** for this course is to submit all assignments with at least **one** completed task. In all worksheet or assignment the first couple of tasks follow the excercises explained in the given tutorial files.

The result should look like a **report**, which will be generated from the worksheets as it will be explained on the [lecture](1-createreport). All figures should have *labels*, *title*, each exercise should end with a descriptive *conclusion* and the explanatory comments should be inserted into the code. These are **must have features** of a work that is intended for presentation.

### Grading

Each assignment will be corrected after submission and a maximum of 20 points will be given for it. 10 for all the completed tasks, 10 for the quality of the submitted report (look and clarity). 
The final grades will be given according to the following pointsystem:<br>
0 - 60: failed<br>
61 - 79: 2<br>
80 - 101: 3<br>
102 - 129: 4<br>
130 - : 5<br>

### Example Datasets

In the */home/course/Datasets* directory you will find datasets, that you can work with.

### Learning materials
* Python tutorial: http://bokae.web.elte.hu/numerical_methods.html (translated from the BSc course "numerical methods in physics I" by Eszter Bokányi, work in progress )
* SQL tutorial: https://www.w3schools.com/sql/ 
* RESTful service: https://en.wikipedia.org/wiki/Representational_state_transfer
* Networkx: https://networkx.github.io/

#### Recommended readings

* Wes McKinney: Python for Data Analysis, (O’Reilly 2013)
* Joel Grus: Data Science from Scratch (O’Reilly 2015)

