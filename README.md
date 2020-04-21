# Bokeh
Practicing with bokeh
-----------------------------------------------------------------------
#Line
#Making a basic bokeh line graph

#importing Bokeh
from bokeh.plotting import figure
from bokeh.io import output_file, show

#prepare some data
x = [1,2,3,4,5]
y = [6,7,8,9,10]

#prepare the output file
output_file("Line.html")

#create figure object
f = figure()

#create line plot
f.line(x,y)

#write the plot in the figure object
show(f)

------------------------------------------------------
#Triangle
from bokeh.plotting import figure
from bokeh.io import output_file, show

x = [1,2,3]
y = [4,5,6]

output_file("Triangle.html")

f = figure()

f.triangle(x,y)

show(f)

---------------------------------------------------
