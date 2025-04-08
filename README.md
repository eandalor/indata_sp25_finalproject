## **Final Project Milestone #1**

April 7, 2025

The goal for the first milestone of the final project was to create visualizations of different color spaces for comparison.

I used [Colour - Datasets](https://github.com/colour-science/colour-datasets) to pull a dataset from Zenodo. The dataset I used was [Camera Dataset](https://zenodo.org/records/8314702) by Solomatov and Akkaynak (2023)[](https://color-lab-eilat.github.io/Spectral-sensitivity-estimation-web/). When loading  Solomatov and Akkaynak's (2023) dataset through  Colour, there is data from 169 cameras, although the dataset on Zenodo has data from over 1,000 cameras. I would like to dive further into the larger dataset as I progress in the final project because it includes data for my personal camera. For Milestone #1, I chose one expensive camera (Leica M (Type 262) and one cheap camera (Olympus PEN E-PM2) to see if price point affects spectral sensitivity.

For Milestone #2, creating a camera match may not be attainable, but I am excited to add interactivity to choose between different visualizations. Also, Colour's plotting functions use matplotlib, and I would like to dive more into customizing the visualizations.

Because the goal of Milestone #1 was relatively simple, I think expectations were met (no failures, no huge successes). I did not visualize color spaces, but that is because the color spaces are built into Colour, so it wouldn't have led to particularly interesting visualizations. The spectral sensitivity data is *estimated* data, but for the purposes of this project, I think it is a perfect dataset for learning Colour, visualizing differences between cameras, and creating an interactive tool that could have real data added in the future. Also, the dataset for this project is based on RAW DNG data processed by Adobe DNG Converter, so the current state of the data is only applicable to the RAW images.
