## **Final Project Milestone #3** ##

April 28, 2025

The original goal for the third milestone of the final project was to create a Dash app that allows users to choose between visualizations and camera matching. It goes without saying, as I have worked on this project and explored Colour, my goals have changed.

Last milestone, I learned how to add interactivity to the figures, and I set a goal to explore the different types of figures that could be generated with Colour’s built-in plotting functions. One of the figures that I find most interesting for the target audience are the spectral distributions in the chromaticity diagram (plot_sds_in_chromaticity_diagram) that shows where the different cameras’ RGB values are in a 2D visualization of a color gamut. By default, it plots RGB values, which is helpful, but I need to figure out how to change the labels of the points to make the visualization make sense. I also found the color swatch plotting (plot_multi_colour_swatches) interesting. If I plug in the RGB values of the dataset, it is the most straightforward way of showing the audience the difference in the resulting color rendition.

I am trying to keep my audience in mind - that of photographers and filmmakers - as I work on this project. All of these diagrams are understandable for professionals in the space. However, if I am trying to target individuals who may not have a solid understanding of color science, then the majority of these visualizations are still not simple enough to show the story of the data. After talking with classmates and exploring Colour, I have realized that the best use of this project is to show the initial steps in *the camera doesn’t matter* journey. I hope to explain that camera sensors capture data, and the images we see are simply how data is interpreted and made available to view. If we can alter the data - if we can move the red, green, and blue points to line up (I am thinking of the chromaticity diagram), then we can alter the final image we see.

***

## **Final Project Milestone #2**

April 14, 2025

The goal for the second milestone of the final project was to add interactivity to visualizations and create a camera match.

I spent much more time working on this one interactive visualization than I would like to admit. Colour's built-in plotting functions are wonderful, but making the visualizations from Matplotlib interactive is not particularly intuitive (for obvious reasons). First, I tried assigning variable names to the figures & using Colour's [plot_image function](https://colour.readthedocs.io/en/latest/generated/colour.plotting.plot_image.html#colour.plotting.plot_image) to hopefully not have to download each figure and reference the file path later. After some failed attempts and some Googling, the most recommended path for using Matplotlib figures in Plotly is to download/export the visualizations and then read them as PNGs.

When using Plotly to read in images, the files could not be saved locally and had to be sourced from a URL. Using an example from the [reference page](https://plotly.com/python/images/#zoom-on-static-images) and our [in-class button notes](https://github.com/dataesilva/indata_sp25/blob/main/plotly-buttons-prep.ipynb), I was able to create the buttons and load in each image. When toggling visibility, I tried using *add_layout_image* like it was used on the example page. In order to use the relayout buttons, I needed to use *update_layout*, and I was only able to solve this problem because of ChatGPT.

After Milestones #1 and #2, I've realized that my goals for this project were a little too ambitious. I can see the path of getting to a tool that creates camera matches, but there is a lot of work to be put in before I can get there. After Milestone #2, I am excited to have figured out how to tie Colour's built-in plotting functions into Plotly to create interactivity. This method is definitely brute force, but figuring the path out (mostly) on my own is rewarding. After solving this problem, I will be able to dive more into the visualizations & find the best visualizations that allow users to see the differences between cameras, and hopefully, how cameras are ultimately data-capturing tools that are what the end user makes them.

***

## **Final Project Milestone #1**

April 7, 2025

The goal for the first milestone of the final project was to create visualizations of different color spaces for comparison.

I used [Colour - Datasets](https://github.com/colour-science/colour-datasets) to pull a dataset from Zenodo. The dataset I used was [Camera Dataset](https://zenodo.org/records/8314702) by Solomatov and Akkaynak (2023)[](https://color-lab-eilat.github.io/Spectral-sensitivity-estimation-web/). When loading  Solomatov and Akkaynak's (2023) dataset through  Colour, there is data from 169 cameras, although the dataset on Zenodo has data from over 1,000 cameras. I would like to dive further into the larger dataset as I progress in the final project because it includes data for my personal camera. For Milestone #1, I chose one expensive camera (Leica M (Type 262) and one cheap camera (Olympus PEN E-PM2) to see if price point affects spectral sensitivity.

For Milestone #2, creating a camera match may not be attainable, but I am excited to add interactivity to choose between different visualizations. Also, Colour's plotting functions use matplotlib, and I would like to dive more into customizing the visualizations.

Because the goal of Milestone #1 was relatively simple, I think expectations were met (no failures, no huge successes). I did not visualize color spaces, but that is because the color spaces are built into Colour, so it wouldn't have led to particularly interesting visualizations. The spectral sensitivity data is *estimated* data, but for the purposes of this project, I think it is a perfect dataset for learning Colour, visualizing differences between cameras, and creating an interactive tool that could have real data added in the future. Also, the dataset for this project is based on RAW DNG data processed by Adobe DNG Converter, so the current state of the data is only applicable to the RAW images.
