# Dionex_ICS1500 Ion Chromatography Anion Tracker v_1.1

This notebook allows you to take data from the Dionex ICS1500 and process the data to get some pretty graphs. You need not have any python experience to run this notebook.
Alternatively, as long as your data is formatted the way you see in the example table, you can use this. So don't limit yourself to just data analysis from the Dionex!

## Installing Python Packages

So, if you've just installed python, you probably don't have any of the packages installed. To install packages, you need to go to your command line if you are using a Mac, or open up cmd.exe as an administrator in Windows.
After you've got that nice black screen up and open you want to type the following:

    python -m pip install -U pip

Next, you want to install your packages. For instance, say we want to install matplotlib, you paste in the following:

    python -m pip install -U matplotlib

Great!

## Required Packages
- [Matplotlib](https://matplotlib.org/3.4.3/users/installing.html)
- [Numpy](https://numpy.org/install/)
- [Pandas](https://pandas.pydata.org/docs/getting_started/install.html)
- [Scipy](https://scipy.org/install/)
- [Math](https://pypi.org/project/python-math/)

## Running Cells
When you come across a cell you need to run, press Shift+Enter (or Return if you're on Mac) this runs the cell and spits out stuff. You can use shift+enter on cells that have this kind of text on it, but it won't do anything. Cells with code have the letters `In[ ]` on the left hand side. It will show `In[*}` while it's running and, it will show a number in it when it's done (e.g. `In[1]`). 

## What this notebook does

   1. Takes a formatted sheet from the Dionex and converts it to a format that Python can read. For this sheet, it is important that all the values you have are converted to concentration. 
   2. Averages the samples in triplicate and gets the standard deviation
   3. Plots the samples in a set of graphs 


## Before Starting, Look at the example data!

You should have the data you put into here look a lot like the sample data that is associated with this notebook. The key things that you want in your spreadsheet is:
    
   - A header on row A in the format of "Condition_ion". For example, Condition_1_sulfate. __Be sure to include no spaces__, if you need a space, place an underscore!  
   - Column 1 should!
 have the header "Time". In this column you should have all of samples of the particular time on the same row

See this example:
[Screenshot from 2021-12-06 11-05-14](https://user-images.githubusercontent.com/27031932/144906726-4ae1cd04-bed5-409c-a8b5-92974f484772.png)
   
That's it!

Have fun! And make some pretty graphs
Be sure to make a new copy everytime you run a new experiment, so you're not deleting old data! And let me know if you have any questions.
