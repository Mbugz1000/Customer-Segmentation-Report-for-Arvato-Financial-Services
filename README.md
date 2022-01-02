# Create a Customer Segmentation Report for Arvato Financial Services
## Installation
Run the following command to set up the environment for this project. 

```
conda create --name project_4_udacity python==3.7.3 && conda activate project_4_udacity && conda install pandas jupyterlab altair "pandas-profiling>2.0" pytest scikit-learn lightgbm hdbscan shap umap-learn imbalanced-learn
```

Download the datasets used in this project here:
- [reviews.csv.gz](http://data.insideairbnb.com/united-states/wa/seattle/2021-09-25/data/reviews.csv.gz)
- [calendar.csv.gz](http://data.insideairbnb.com/united-states/wa/seattle/2021-09-25/data/calendar.csv.gz)
- [listings.csv.gz](http://data.insideairbnb.com/united-states/wa/seattle/2021-09-25/data/listings.csv.gz)

Once downloaded, dump this data in _/data/raw_


## Project Motivation
This is the first of several Udacity projects in the Data Science Nano-degree program. The primary aim of this project 
is therefore to complete the course-work of the mentioned program. 

The secondary aim of this project was to answer the 4 business questions related to AirBnB Seattle listings:
1. Does becoming a verified host positively impact your monthly income or occupancy rate in Seattle?
1. Does becoming a Super-Host positively impact your monthly income or occupancy rate in Seattle?
1. Does proximity to competition negatively impact your monthly income?
1. What factors should influence the rate you set for your listing?

## File Descriptions
This project is has 2 primary folders: 
- **data** : Data Folder. It contains 2 folders
    - **processed**: Output of the analysis
    - **raw**: The raw data downloaded from InsideAirBnb
- **src**: Source code folder. It contains 2 files:
    - **Analysis Notebook**: Jupyter notebook where the analysis was performed
    - **multiprocessing_fn**: A python module that is imported by the notebook

## How to Interact with Project
To interact with the project, take the following steps:
1. Activate the _project_1_udacity_ environment on the Anaconda console
1. Navigate to the directory of the project on the Anaconda Console
1. Start up Jupyter Lab using the command `jupyter lab`
1. Open the Analysis notebook from the jupyter notebook page
1. Run all the cells to run the analysis.

## Results Summary
The results of this analysis were as follows: 
- Question 1:
   - No. It does not positively impact your monthly AirBnb income
- Question 2:
   - Yes. It positively impacts your monthly income by $900 on average
- Question 3:
   - Yes. It negatively impacts your monthly income by $300 on average
- Question 4:
   - The top 5 listing based factors that should be considered are as follows: 
        1. No. of guests that you can accommodate
        1. Location of your listing
        1. Competition in your area
        1. Kitchen appliances that you make available
        1. Type of property

## Licensing, Authors & Acknowledgements
- [How to Use t-SNE Effectively by Martin Wattenberg,Fernanda Viégas & Ian Johnson](https://distill.pub/2016/misread-tsne/)
- [How HDBSCAN Works - HDBSCAN Docs](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
- [Understanding UMAP by Andy Coenen & Adam Pearce](https://pair-code.github.io/understanding-umap/)
- [Using UMAP for Clustering - UMAP Docs](https://umap-learn.readthedocs.io/en/latest/clustering.html)
- [tSNE vs. UMAP: Global Structure by Nikolay Oskolkov](https://towardsdatascience.com/tsne-vs-umap-global-structure-4d8045acba17)
- [The right way of using SMOTE with Cross-validation by KSV Muralidhar](https://towardsdatascience.com/the-right-way-of-using-smote-with-cross-validation-92a8d09d00c7)
- [Compare over-sampling samplers - ImbLearn Docs](https://imbalanced-learn.org/stable/auto_examples/over-sampling/plot_comparison_over_sampling.html)
- [AZ Germany grid](https://www.regionale-marktdaten.de/az-deutschland-raster/)
- [PLZ8 for Germany](https://www.regionale-marktdaten.de/plz8/)