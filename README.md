
# Assignment 04

# Project Proposal

![http://www.pratt.edu/tiny_mce/plugins/imagemanager/files/Light_brown_blue22.jpg](http://www.pratt.edu/tiny_mce/plugins/imagemanager/files/Light_brown_blue22.jpg)

The **purpose of this project** is to have some **well-written** and **well-documented code** in a GitHub repository that illustrates you can write some Python code. This project is for **your** Portfolio, so pick something you are **interested in** or that's **useful** (either in some professional work or automating some task). [Learn how the project is evaluated (rubric)](https://github.com/pratt-savi-810/pratt-savi-810-2020-03-project).


#### Project Routes

There's a couple of routes you can go;

1. **Creating a Tool to Automate a Task** - usually for some task automation, less an analysis, more data engineering. 
2. **Performing Data Analysis to Answer a Research Question** - this type of project requires plots and data insights. 

Since writing the code is the challenging part. Do not think about this in scope of a normal project. **Keep your scope focused!** Keep it limited in functionality and if you finish early, you can add more features. I've seen students go down some pretty deep rabbit holes and emerge with some very disorganized projects. You could have only 30 lines of code or so, and still have a great project so long as the code is well written and the doc's are informative and it has some functionality that's useful in some capacity. Most likely someone such as a hiring manager will only glance at your Repository, so you want it to be organized and clean and very clear as to its purpose. 

## Assignment 04 Submission
You will **Fork** and **Clone this Repo** and **edit this README.md Markdown file**. This is your submission, just the link to your forked Repo and edited README.md file. This project should be the edited version of this README.md (**Markdown**) file. 

#### Learn more about [Markdown](https://www.markdownguide.org/). 

Most code editors allow editing of Markdown files, some recommended editors are;

* [Atom](https://atom.io/)
* [MacDown](https://macdown.uranusjr.com/)
* [Visual Studio Code (VS Code)](https://code.visualstudio.com/)
* [StackEdit (edit in-browser)](https://stackedit.io/)
* [Dillinger (edit in-browser)](https://dillinger.io/)
* You can even edit inside of [GitHub](https://github.com/). 

Your Assignment 04 Deliverables are listed below:

# Deliverables

You should edit the following items in-line and substitute any of the provided text with your response below for your README.md Assignment 04 submission. 


---

## Executive Summary

A _brief description_ of your final project idea. 

- **Why** are you doing this project? 
- **How** do you imagine you'll accomplish this project? 
- Is this a project **Creating a Tool to Automate a Task** or **Performing Data Analysis to Answer a Research Questio**? 

** Create a tool to automate map and chart creation and some data analysis for those maps and charts**
I have been working with the NY NJ Harbor Estuary Program for the last two years creating reports about the work they do in the Hudson River Estuary. Much of the data visualization for these reports involves a lot of exploration of the datasets that come to us in a variety of forms. Some are cleaned up and organized, some data is raw and most of it needs to be cleaned and organized before we can start experimenting. I would like to create a couple of tools; one for charts and one for maps that would help streamline the process of exploring the data patterns and possible ways to highlight findings, and then to export cleanly styled charts and maps with clear, well designed legends. I want be able to apply these tools to multiple datasets.

## Background

A more **detailed background** of your project, please include any information that would be useful for understanding the context of the project. This can be as long or short as you'd like. 

I have designed (with help from partners at Pratt) 5 different reports for the NY-NJ Harbor Estuary Program using a variety of tools. The data visualization is a huge part of these reports and we were hired to explore the data and the analysis and to come up with the best ways to tell the stories behind the data. Most of the work I've done for this has been manual; I've approached each visualization separately and though some related datasets follow a set formats, I've created each individually. I want to make this process faster to not only save time exploring the data but also create a tool that would allow broader experimentation than I'm able to do with excel and more manual processes. I'd like to do this for spatial and non-spatial data but will start with map plots because my colleague (can Sucuoglu) has already written python code that we're using for charts. If I can automate the map plots, I may be able to apply some of that functionality to plotting non spatial data by adding to and working from Can's python code. 

Any scripts I can develop will be things I can modify and reuse in the future, so even if I don't create complex functions, any plots meeting the goals below will be useful. Automating some of the tasks would be ideal. 

Examples of the data visualizations done for HEP over the last two years can be seen [here](https://sara-eichner-xbkp.squarespace.com/nynj-harbor-estuary-program).

Specific goals: 
- get specific data from excel sheets, by row or column name and numbers, not necessarily the whole sheet
- create different plot types quickly 
- create plots that pull data subsets apart into small multiples and also plot them together in various chart styles (line, scatter plots, bar charts, etc.)
- cycle through layers of map data to look at one layer at a time
- set arguments that can be changed to alter the specific design elements that often need modification
- set plot parameter variables to address style experimentation to control the visual emphasis to best tell a particular story.
- export charts that are close to presentation ready to save time on clean up in Illustrator 
- produce chart variations to present visualization strategy and style options to clients in the design development stage.

I plan to use sample datasets from the Harbor Estuary Water Quality Report, currently in progress. I will first work to create exploratory and presentation plots and maps from this data individually. Then I will attempt to create a function from that code so that the process can be applied to additional datasets. 

## Resources
List any possible articles, resources or analysis or anything useful and include links and perhaps annotate a sentence as to the key findings of this resource. Or if you cannot find any resources please mention. 

#### Resources List

* [Spyder](https://www.spyder-ide.org/), mainly because it's already in use for the water quality report. 
* SAVI 810 lessons -- I plan to go through the lessons and do some follow up reading on resoure sites 
* [Flowing Data](https://flowingdata.com/) -- more focused on R but I like the tutorials and discussions about data visualization on that site for inspiration and guidance.
* I'm open to suggestions!
 
 
## Input Data 

#### Data Sources List 
List any possible data including links with any input data sources you'll be using. 

* /Users/saraeichner/Documents/GitHub/HEP_data
* Data comes from the [NY-NJ Harbor Estuary Program](https://www.hudsonriver.org/estuary-program), which is part of the Hudson River Foundation.
	* spatial (point and polygon), such as sampling locations, sources of contaminants, watershed polygons and a study area polygon
	 * non-spatial data that includes water quality measurements in the Hudson such as pathogens, dissolved oxygen, and pH. Non spatial data is collected from the same sampling locations and is all formatted and processed in the same way in terms of annual geomeans and monthly samples. 
* IUS state datasets for NJ and CT boundaries, still to find

#### Data Wish List
List and describe any type of data you'd like to include but had difficulty tracking down. 



## Technical Requirements

#### Python Libraries
List any Python libraries you think you may need. Desribe what you may use them for. 

* Matplotlib: for plotting, bounding box
* Seaborn: for its data viz and plotting library, color palettes 
* Shapely: to look at point and polygon data as points and polygons
* numpy: to query tabular data in shapefiles and look at subset statistics if relevant
* spyder: a notebook to save final code blocks in -- I also like the variable explorer, options for viewing data and plots, etc. and might find it useful to use this. If it takes too much time though, I'll stick with Jupyter. 
* Fiona: for reading in spatial data
(I could use advice about this -- how to focus on the most relevant parts of these libraries)

#### Library Wish List
Also note any libraries or functionality that you may need that you're not sure exists. Try your best to articulate this in words. This will be helpful if I can provide any libraries to suggest for use in the project. 

* Python Library Wish List Item A - to create color ramps and specific color palettes. 
* Python Library Wish List Item B -  Legend parameters that go beyond what I've been able to do so far


## Measuring Success: 
	 
Success will involve scripts that allow me to quickly explore data in shapefiles and Excel sheets, apply plotting parameters (such as legend styles, font styling, categorical and quantifiable data styling, plot composition and sizing, bounding boxes / extents, single and graduated marker sizes, use of custom color palettes and color ramps, etc.), and export near presentation-ready plots to a vector format. Ideally this scripts will be worked into functions so they are easily applied to multiple datasets.
- Even if I'm not able to create functions for all my goals, any scripts I can develop can be modified and useful in the future.
- I'm not sure which tasks I'll be able to fully automate. I'd like to build some plots and chose what can be automated and work on 1 at a time from those code blocks.

## Project Execution Plan Outline
Please include a short outline describing the steps you'd imagine going through. 

```
This week, 4/21: 
- Research tools, libraries and strategies (from lesson resources)
- find contextual state boundary data 
- Clean and prep data
- Explore spatial datasets in map plots (build from assignment 3)
	- revise that map to include the larger region, add NJ data and utilize the bounding box option in maplotlib
- Learn how to use categorical data in point and polygon format
- Learn how to add other elements to legends like polygon data
- create color palette and color ramp and try to use them
- Establish a set of plots from this experimentation that could be used for data exploration in the future

Next week, 4/27: 
- Explore non spatial datasets 
(build from HEP charting code and from map plots: ie. color, fonts, styles, etc.)
- establish a set of chart styles as an exploratory chart set 

End of week (4/27) through May 6: 
- begin trying to build functions out of chart and map code. 
- Automate to apply code to multiple datasets.
- trouble shoot
- I don't know how long this will take or if I'll be able to do it ...
- prepare code and results for presentation
- show notebook and sample plots in pdf format

```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTI0NTU3ODE5LC0xODY2NTY4NDExLDEzMj
IzNjI1NTksMTMyODY5NjQ5NCw5NjcwNTQyODksLTM4NzEyODI1
LC0yMDYyMzM1NTg4LC0xNTc0NDI2OTEyLDE5Nzk1NzgzMzQsOT
E1NDIzMDQwLDE1MzI0MTY4ODAsMjU1NzA4NDgyLC0yMDAwODY4
NTA4XX0=
-->