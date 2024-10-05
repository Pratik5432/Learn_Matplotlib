# Steps to plan a data visualization
Let’s go through an example of a real-life situation where a data analyst might need to create a data visualization to share with stakeholders. Imagine you’re a data analyst for a clothing distributor. The company helps small clothing stores manage their inventory, and sales are booming. One day, you learn that your company is getting ready to make a major update to its website. To guide decisions for the website update, you’re asked to analyze data from the existing website and sales records. Let’s go through the steps you might follow. 

### Step 1: Explore the data for patterns
First, you ask your manager or the data owner for access to the current sales records and website analytics reports. This includes information about how customers behave on the company’s existing website, basic information about who visited, who bought from the company, and how much they bought.

While reviewing the data you notice a pattern among those who visit the company’s website most frequently: geography and larger amounts spent on purchases. With further analysis, this information might explain why sales are so strong right now in the northeast—and help your company find ways to make them even stronger through the new website. 

### Step 2: Plan your visuals
Next it is time to refine the data and present the results of your analysis. Right now, you have a lot of data spread across several different tables, which isn’t an ideal way to share your results with management and the marketing team. You will want to create a data visualization that explains your findings quickly and effectively to your target audience. Since you know your audience is sales oriented, you already know that the data visualization you use should:

* Show sales numbers over time
* Connect sales to location
* Show the relationship between sales and website use
* Show which customers fuel growth

### Step 3: Create your visuals
Now that you have decided what kind of information and insights you want to display, it is time to start creating the actual visualizations. Keep in mind that creating the right visualization for a presentation or to share with stakeholders is a process. It involves trying different visualization formats and making adjustments until you get what you are looking for. In this case, a mix of different visuals will best communicate your findings and turn your analysis into the most compelling story for stakeholders. So, you can use the built-in chart capabilities in your spreadsheets to organize the data and create your visuals.


# MATPLOTLIB GRAPHS AND CUSTOMIZATIONS

#### Markers 
marker = '.', ',', 'o', 'v', '^', '<', '>', 's', 'p', '*', 'h', 'H', '+', 'x', 'D', 'd', '1', '2', '3', '4', '8', '|', '_', 'tickleft', 'tickright', 'tickup', 'tickdown' 

markersize = 1, 2, 3, and so on  OR  ms = 1, 2, 3, and so on   (Markersize)

mec = 'r', 'b', 'g' , etc   (Marker Color)

markerfacecolor = 'r', 'b', 'g' , etc

#### Colors
color = 'blue', 'green', 'red', 'cyan', 'magenta', 'yellow', 'black', 'white', 'orange', 'purple', 'brown', etc.

#### Linestyle
linestyle = '-', '--', '-.', ':'

color or the shorter c = 'r', 'b', 'g' , etc   (Line Color)

linewidth or the shorter lw = 20, 10, 12   (Line Width)


### 1) plt.plot()
* x: Data for the x-axis.
* y: Data for the y-axis.
* color: Line color ('r', 'g', etc.).
* linestyle: Type of line ('-', '--', '-.', ':').
* linewidth: Width of the line.
* marker: Marker style ('o', 's', '^', etc.).
* label: Label for the legend.
* eg: plt.plot(x, y, color='blue', linestyle='--', linewidth=2, marker='o')

### 2) plt.scatter()
* x: Data for the x-axis.
* y: Data for the y-axis.
* color: Color of the points.
* s: Size of the points.
* alpha: Transparency of the points.
* marker: Marker style.
* label: Label for the legend.
* eg: plt.scatter(x, y, color='blue', s=50, alpha=0.6)

### 3) plt.hist()
* x: Data to plot.
* bins: Number of bins (default is 10).
* range: The lower and upper range of the bins.
* density: If True, normalizes the histogram.
* color: Color of the bars.
* alpha: Transparency of the bars.
* eg: plt.hist(data, bins=20, color='green', alpha=0.7)

### 4) plt.bar()
* x: Categories for the x-axis.
* height: Heights of the bars.
* width: Width of the bars.
* color: Bar color.
* edgecolor: Color of the bar borders.
* align: How to align the bars ('center' or 'edge').
* label: Label for the legend.
* eg: plt.bar(x, height, width=0.8, color='red', edgecolor='black')

### 5) plt.pie()
* x: Values for each wedge.
* labels: Labels for each wedge.
* autopct: String to format the percentage (e.g., '%.1f%%' , '%1.1f%%').
* colors: List of colors for each wedge.
* explode: Fraction to separate the slices. For eg: [0, 0, 0, 0.1, 0]; if you want 4th element to explode from the pie.
* shadow: Whether to draw a shadow behind the pie.
* eg: plt.pie(data, labels=categories, autopct='%1.1f%%', explode=[0.1, 0, 0])

