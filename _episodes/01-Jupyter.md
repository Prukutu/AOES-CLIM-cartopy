---
title: "Using JupyterLab"
teaching: 0
exercises: 0
questions:
- "How can I use JupyterLab for Climate Data Analysis"
objectives:
- "Learn key features of JupyterLab to use for Climate Data Analysis"
keypoints:
- "JupyterLab can be used as a Python programming environment"
- "You can create notebooks with codes, figures, links, text, and equations"
- "You can run your codes in JupyterLab cell by cell"
---

### JupyterLab (Jupyter Notebook)

JupyterLab allows us to create Jupyter Notebooks which can contain a combination of code, figures, links, formatted text, and LaTex equations.   

It is also a web-based programming interface for mutiple languages (e.g. Python, R, Matlab).  We will use it as our Python programming interface.

Because it also allows figures, links, text, and equations in addition to code, it is very useful for use in research allowing all your information related to your research to be kept together rather than in separate documents. 

### Creating and working with a Jupyter Notebook

First, let's create a new Jupyter Notebook by clicking `File`->`New`->`Notebook` or clicking on `Python 3`
This creates a new notebook with a default title `Untitled.ipynb` or `Untitled#.ipynb`. Note that Jupyter Notebooks end in `.ipynb`

Change the name of your notebook to `PracticeNotebook.ipynb` by clicking `File`->`Save Notebook As`  

The rectangular box in your notebook is called a `cell` it contains a block of `code`, `Markdown`, or `Raw` text.  What a `cell` contains is indicated in the menu above. 

To determine what kind of `Code` a cell contains for a given notebook, the `kernel` is shown in the upper right.  This notebook contains `Python 3` code.

## What is Markdown?

Markdown is a formatting language that allows you to provide formatted text (e.g. bold, italics, links, different sized font, and LaTeX equations)

As an example, let's type the following in a cell and change the cell to Markdown:
> # CLIM 680 Practice Notebook
> ## by Kathy Pegion
> #### for class
>
> ### We can insert `LaTeX` equations
> The equation for the mean is given by: 
> \begin{equation} \mu_n=\sum_{i=1}^{N}X \end{equation}
> 
> #### We can link to papers
> The analysis in this notebook follows, [Pegion et al. 2019](https://doi.org/10.1175/BAMS-D-18-0270.1)
> 
> #### We can make a numbered list; This notebook will:
> 1. First thing
> 2. Second thing
> 3. Third thing
> 
> #### We can make a bulleted list. Important things for this notebook are:
> * something important
> * something else important
{: .source}

{% include links.md %}
