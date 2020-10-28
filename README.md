# Differential-Privacy-Project
## Summary
In this project we looked at the Geolife data. This trajectory dataset constitutes 182 users who have been tracked regularly on a 4 year period. The data from one individual is split into many trajectories, or a paths, which are located in subfiles from the individual's folder. While working on the project, we focused on two principles:

1. Differential Privacy - mathematical noise added to some individuals' usage pattern to obscure personal data. In other word, a way to keep privacy of an individual within the data set, but keep the data public.

2. K-anonymity - A way to make sure privacy is well kept within a dataset. It shows whether or not the information for each person contained in the release cannot be distinguished from at least x individuals - 1 whose information also appear in the release.

## The libraries
  We used pandas with a few other libraries to load the data, and maped the points using Ipyleaflet and folium. However, mapping millions of points on Ipyleaflet proposes two problems: run time and laggy map. Forunatley, we came across the datashader library which with geoviews, holoview, and bokeh allowed us to plot millions of points in a matter of seconds. While we used ipyleaflet and folium to draw a heatmap, or the individuals' trajectories, we used datashader, geoviews, holoviews and bokeh to plot all the data points from the 182 individuals. After, we used numpy to apply the concepts of k-anonymity and differential privacy on our data (more on that in the notebook). Matplotlib also came in helpful to plot interesting graphs using data on k-anonimity and influence (again more on that in the notebook)
  
## The notebook
  The Jupyter notebook first starts off by explaining the libraries we used throughout the project. These go from simple libraries such as pandas and numpy, to more complicated like geoviews and datashader. After explaining the library, I go over dowloading the data, graphing the data and finally applying the concepts of k-hotspots and differential privacy onto the dataset. As we continue to work on this project, we want to add sections of random variables and playing with randomness. 
