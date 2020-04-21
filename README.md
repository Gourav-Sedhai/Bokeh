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
#Circle
#importing bokeh
from bokeh.plotting import figure
from bokeh.io import output_file, show

#Entering datas
x = [1,2,3,4]
y = [5,6,7,8]

#creating output file
output_file("Circle.html")

#creating figure object
f = figure()

#creating a circle
f.circle(x,y)

#showing output
show(f)

------
#From pandas
#Making a basic bokeh line graph

#importing bokeh and pandas
from bokeh.plotting import figure
from bokeh.io import output_file, show
import pandas

#prepare some data
df = pandas.read_csv("data.csv.txt")
x = df["x"]
y = df["y"]

#prepare the output file
output_file("Line_from_csv.html")

#create figure object
f = figure()

#create line plot
f.line(x,y)

#write the plot in the figure object
show(f)

