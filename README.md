
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
I have been working with the NY NJ Harbor Estuary Program for the last two years creating reports about the conservation work they do in the Hudson River Estuary. Much of the data visualization for these reports involves exploration of the datasets that come to us in a variety of forms. Some are cleaned up and organized, some is raw and most of it needs to be cleaned and organized before we can start experimenting. I would like to create a couple of functions or a tool that would help streamline the process of building maps and the associated experimentation. The goal is to be able to find the best ways to highlight findings, and to export styled maps with clear legends. 

## Background

A more **detailed background** of your project, please include any information that would be useful for understanding the context of the project. This can be as long or short as you'd like. 

I have designed (with help from partners at Pratt) 5 different reports for the NY-NJ Harbor Estuary Program using a variety of tools. The data visualization is a huge part of these reports and we were hired to explore the data and the analysis and to come up with the best ways to tell the stories behind the data. Most of the work I've done for this has been manual; I've created each visualization separately. I want to make this process faster for exploring the data and also extend the experimentation. I'd like to do this for spatial and non-spatial data but will focus for this project on map plots. If I'm able to build a function for map plots, I'll be able to apply that process to chart building later. 

Any scripts I can develop will be things I can modify and reuse in the future, so even if I don't create complex functions, any plots meeting the goals below will be useful. Automating some of the tasks would be ideal. 

Examples of the data visualizations already created for HEP [here](https://sara-eichner-xbkp.squarespace.com/nynj-harbor-estuary-program).

Specific goals: 
- get specific data from excel sheets, by row or column name and numbers, not necessarily the whole sheet
- create different plot types quickly 
- create plots that pull data subsets apart into small multiples and also plot them together in various styles (for instance, 5 variations showing different classifcation methods for a chorolpleth map so they can be compared)
- cycle through layers or regions of map data to look at one layer at a time
- set arguments that can be changed to alter the specific design elements that often need modification
- set plot parameter variables to address visual emphasis to best tell a particular story.
- export maps that are close to presentation ready to save time on clean up in Illustrator 
- produce map variations to present visualization strategies to clients in the design development stage.

I will first work to create maps individually. Then I will attempt to create a function from that code so that the process can be applied to additional datasets or a different group of style variations. 

## Resources
List any possible articles, resources or analysis or anything useful and include links and perhaps annotate a sentence as to the key findings of this resource. Or if you cannot find any resources please mention. 

#### Resources List
* [Spyder](https://www.spyder-ide.org/), mainly because it's already in use for the water quality report and I'm interested in exploring it.  
* SAVI 810 lessons -- I plan to go through the lessons and do some follow up reading on resource sites 
* [Flowing Data](https://flowingdata.com/) -- more focused on R but there are a number of articles about data visualization with python, geopandas and maplotlib.
 
## Input Data 

#### Data Sources List 
List any possible data including links with any input data sources you'll be using. 

* /Users/saraeichner/Documents/GitHub/final_project_eichner/HEP_data
* Data comes from the [NY-NJ Harbor Estuary Program](https://www.hudsonriver.org/estuary-program), which is part of the Hudson River Foundation.
	* spatial (point and polygon), such as sampling locations, sources of contaminants, watershed polygons and a study area polygon
	 * non-spatial data that includes water quality measurements in the Hudson such as pathogens, dissolved oxygen, and pH. Non spatial data is collected from the same sampling locations and is all formatted and processed in the same way in terms of annual geomeans and monthly samples. I may join some of this to spatial data for experimentation with categorical and quantitative data 
* US state datasets for NJ and CT boundaries, still to find

#### Data Wish List
List and describe any type of data you'd like to include but had difficulty tracking down. 

## Technical Requirements

#### Python Libraries
List any Python libraries you think you may need. Describe what you may use them for. 

* Matplotlib: for plotting, bounding box
* Seaborn: for its data viz and plotting library, color palettes 
* Shapely: to look at point and polygon data as points and polygons
* numpy: to query tabular data in shapefiles and look at subset statistics if relevant
* spyder: a notebook to save final code blocks in -- I also like the variable explorer, options for viewing data and plots, etc. and might find it useful to use this. If it takes too much time though, I'll stick with Jupyter. 
* Fiona: for reading in spatial data

#### Library Wish List
Also note any libraries or functionality that you may need that you're not sure exists. Try your best to articulate this in words. This will be helpful if I can provide any libraries to suggest for use in the project. 

* Python Library Wish List Item A - to create color ramps and specific color palettes. 
* Python Library Wish List Item B -  Legend parameters that go beyond what I've been able to do so far

## Measuring Success: 
	 
Success will involve scripts that allow me to quickly explore data in shapefiles and Excel sheets, apply plotting parameters (such as legend styles, font styling, categorical and quantifiable data styling, plot composition and sizing, bounding boxes / extents, single and graduated marker sizes, use of custom color palettes and color ramps, etc.), and export near presentation-ready plots to a vector format. Ideally this script will be worked into functions so they are easily applied to multiple datasets.
- Even if I'm not able to create functions, any scripts I can develop can be modified and useful in the future.
- I'm not sure which tasks I'll be able to fully automate. I'd like to build some maps, choose what can be automated and work on 1 at a time from those code blocks.

## Project Execution Plan Outline
Please include a short outline describing the steps you'd imagine going through. 
```
This week, 4/21: 
- Research libraries and strategies
- Find contextual state boundary data 
- Clean and prep data
- Explore spatial datasets in map plots (build from assignment 3)
	- revise that map to include the larger region, add NJ data and utilize the bounding box option in maplotlib 
- Learn how to use categorical data in point and polygon format

Next week, 4/27: 
- Learn how to add other elements to legends like polygon data
- create color palette and color ramp and try to use them
- establish a set of map styles as an exploratory map set 
- evaluate map plot code for tasks that might be automated

End of week (4/27) through May 6: 
- begin trying to build functions out of map code. 
- Automate to apply code to multiple datasets.
- prepare code and results for presentation

```

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ5NzAwNzg0NCwtMjEyMTYxNTcyOCwtNz
E2MTMxODg1LDk5NTA5MTUzOCw1ODcwNDc0ODgsLTI0NTU3ODE5
LC0xODY2NTY4NDExLDEzMjIzNjI1NTksMTMyODY5NjQ5NCw5Nj
cwNTQyODksLTM4NzEyODI1LC0yMDYyMzM1NTg4LC0xNTc0NDI2
OTEyLDE5Nzk1NzgzMzQsOTE1NDIzMDQwLDE1MzI0MTY4ODAsMj
U1NzA4NDgyLC0yMDAwODY4NTA4XX0=
-->