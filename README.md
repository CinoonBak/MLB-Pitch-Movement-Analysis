# MLB-Pitch-Movement-Analysis
Collection of visualizations and clustering analysis to view group similar pitchers together
# Project Overview
* Collected all pitchers pitch movement who threw in the MLB 2022 season. 
* Cleaned and joined all pitch movement data. 
* Used visualzation tools to analyze each pitch and each pitcher. 
* Optimized clustering analysis to learn the pitch movement for each cluster. 
# Code & Resources Used
Python Version: 3.9.12 | Tableau Public
* Python Packages: pandas, numpy, sklearn, matplotlib, seaborn
* Finding Optimal Cluster Number: https://towardsdatascience.com/cheat-sheet-to-implementing-7-methods-for-selecting-optimal-number-of-clusters-in-python-898241e1d6ad
# Data Collection
* MLB.com provides all statistical data for all MLB player. 
* MLB.com has a feature for everyone to download the data into a CSV file. 
* Collected six different pitche movements which are: four seam fasteball, sinker, cut fastball, curveball, slider, and changeup.
# Data Cleaning
After collecting the data I have made the following changes: 
* Individually cleaned all six pitch data
* Deleted useless columns 
* Dropped all null values
* Joined all six pitches together into one dataframe
# EDA
I have visualized through Tableau Public and Matplotlib. Here are some of the foundings: 

<img width="147" alt="Screen Shot 2023-03-05 at 4 49 34 PM" src="https://user-images.githubusercontent.com/118776460/224375370-7ffdf058-3a00-43bf-8e72-353380e5b9cf.png">

<img width="496" alt="Sandy Alcantara" src="https://user-images.githubusercontent.com/118776460/224376457-1cc651c1-09b2-48ef-8a38-290764379abc.png">

<img width="625" alt="Screen Shot 2023-03-10 at 10 49 23 AM" src="https://user-images.githubusercontent.com/118776460/224374772-20be17b3-58b6-46ef-a9dd-578548708bfd.png">

#Data Preprocessing
* I have deleted other columns and only included the columns for average speed, vertical break, and horizontal break
* I have scaled all of my columns to standardize the numeric values
# Model Building
* I have modeled a cluster with 10 cluster
* I used the Elbow Method and Silhouette Method to find the optimal cluster numbers
<img width="411" alt="Screen Shot 2023-03-10 at 11 05 32 AM" src="https://user-images.githubusercontent.com/118776460/224378280-d4fb77cd-6bcf-4917-a7eb-5f3cddf372b4.png">

# Model Testing 
* I have specifically left out one player to test the model
* I included him in the columns and ran another clustering analysis with everything hold consetent
* The cluster numbers changed but the players in the cluster did not change except 2 or 3
