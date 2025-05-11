 
Image Analysis Project
This project is a Jupyter Notebook implementation designed to load, analyze, and visualize a dataset of images from two categories: Real Art and AI-generated Art. It includes classes for data loading, feature extraction, analysis, and visualization, producing statistical summaries and graphical representations of image features.

Overview
The notebook processes images from specified directories, extracts features such as mean intensity, standard deviation, contrast, and aspect ratio, and generates visualizations including histograms, scatter plots, boxplots, bar charts, and a grid of the top 10 images by contrast. The code is structured into modular classes for reusability and clarity.

Requirements
Python 3.x
Required libraries:
numpy
pandas
pillow (PIL)
matplotlib
Installation
Install the required dependencies using pip:

pip install numpy pandas pillow matplotlib
Ensure you have Jupyter Notebook installed to run the .ipynb file:

pip install notebook
Alternatively, use a Python environment like Anaconda, which includes Jupyter and the necessary libraries:

conda install jupyter numpy pandas pillow matplotlib
Usage
Clone or Download the Repository:

Download the _Project_DS120 (1).ipynb file or clone the repository containing it.
Prepare the Dataset:

Create two directories with your image datasets:
RealArt for real art images (e.g., D:\PC\Downloads\archive (5)\RealArt\RealArt).
AiArtData for AI-generated art images (e.g., D:\PC\Downloads\archive (5)\AiArtData\AiArtData).
Supported image formats: .png, .jpg, .jpeg, .bmp, .gif.
Update the file paths in the "Main Execution" cell to match your directory locations.
Run the Notebook:

Open a terminal or command prompt and navigate to the directory containing the notebook.
Launch Jupyter Notebook:
jupyter notebook
Open _Project_DS120 (1).ipynb in the browser interface.
Execute the cells sequentially (Cell 1 through 11) by selecting each cell and pressing Shift + Enter.
Explore the Output:

The notebook will display:
Summary statistics of image features.
A histogram of mean intensity.
A scatter plot of mean intensity vs. contrast.
A boxplot of standard deviation.
A bar plot of the top 10 images by contrast.
A 2x5 grid showing the top 10 images.
File Structure
_Project_DS120 (1).ipynb: The main Jupyter Notebook containing the code and visualizations.
Classes and Functionality
DataLoader: Loads images from a directory, resizes them to 128x128 pixels, and converts them to RGB mode. Handles palette-based images with transparency.
FeatureExtractor: Extracts features (mean intensity, standard deviation, contrast, aspect ratio) from the loaded images into a pandas DataFrame.
DataAnalyzer: Provides statistical analysis, including summary statistics and the top 5 images by contrast.
Visualizer: Generates plots and displays the top 10 images based on contrast.
Notes
Image Paths: Adjust the real_path and ai_path variables in the "Main Execution" cell to point to your dataset directories.

Dependencies: Ensure all libraries are installed and compatible with your Python version.

Performance: Processing large datasets may take time; consider optimizing image sizes or using a subset for testing.

Debugging: If images fail to load or display, check the console for error messages (e.g., file not found) and verify file paths and formats.
