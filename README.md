# Assignment-9
# Load the iris dataset
data(iris)

# Basic scatter plot
plot(iris$Sepal.Length, iris$Sepal.Width, 
     xlab = "Sepal Length", ylab = "Sepal Width", 
     main = "Sepal Length vs Sepal Width")

# Load lattice package
library(lattice)

# Lattice plot
xyplot(iris$Sepal.Length ~ iris$Sepal.Width,
       xlab = "Sepal Width", ylab = "Sepal Length",
       main = "Sepal Length vs Sepal Width")


# Load the ggplot2 package
library(ggplot2)

# Scatter plot with ggplot2
ggplot(iris, aes(x = Sepal.Length, y = Sepal.Width, color = Species)) +
  geom_point() +
  labs(x = "Sepal Length", y = "Sepal Width", title = "Sepal Length vs Sepal Width with Species") +
  theme_minimal()


Basic Scatter Plot (Base R): The basic R charting functions (plot()) are used to construct the initial plot.
Sepal Width is plotted on the y-axis and Sepal Length on the x-axis.
"Sepal Length vs. Sepal Width" is the plot's primary title, and the labels for the x and y axes are "Sepal Length" and "Sepal Width," respectively.

Schematic Lattice Plot:
Loading the lattice package (library(lattice)).
The lattice package's xyplot() method is used to construct the second plot.
Sepal Width is plotted on the x-axis and Sepal Length on the y-axis (notice the axes are reversed from the first plot).
The plot's primary title is "Sepal Length vs. Sepal Width," and the labels for the x and y axes are "Sepal Width and Sepal Length," respectively. 

ggplot2: Disk Plot:
The package library(ggplot2) is loaded, containing ggplot2. 
The ggplot() function from the ggplot2 package is used to construct the third plot. 
With dots colored by species, it plots sepal length on the x-axis and sepal width on the y-axis. 
"Sepal Length vs. Sepal Width with Species" is the plot's primary title, while the labels for the x and y axes are "Sepal Length" and "Sepal Width" respectively. 
Furthermore, theme_minimal() is used to set the theme to "minimal".





