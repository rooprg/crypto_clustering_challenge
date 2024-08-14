**CRYPTOCURRENCY CLUSTERING CHALLENGE**

**(1) Project Overview and Purpose:**

The purpose of this exercise is to use Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes. First, original data from a .csv file was used for ascertaining the best k value (visualized on an Elbow Curve) and plotting clusters on Scatter Plots via K-Means. Secondly, Principal Component Analysis (PCA) was used to optimize the clusters, then finding the best k value (visualized on an Elbow Curve) and plotting clusters on Scatter Plots via K-Means for transformed data. Lastly, the first and second parts were visualized in tandem and compared.


**(2) Dataset Description:** 

The dataset includes various crytocurrencies and multiple values for price change percentage at 24 hours, 7 days, 14 days, 30 days, 60 days, 200 days, 1 year, respectively. Data is stored in a .csv file, stored in the Resources folder.


**(3) Data Cleaning and Preprocessing:**

The data in this dataset did not required dropping any rows for missing or incomplete data. Data was normalized with the StandardScalar module to make the modified DataFrame (named "market_data_scaled"). A Principal Component Analysis [PCA] model was used later in the exercise.


**(4) Data Visualization Techniques:**

Two types of visualizations were generated for this exericse. 

(a) Line graphs were used to show:

(i) all cryptocurrencies and their percent change values-

![Cryptocurrencies](Output/one_df_market_data_line_graph.png)

(ii) an Elbow Curve [EC] for the scaled data-

![Scaled Data](Output/two_original_data_elbow_curve.png)

(iii) EC of data after PCA-

![PCA Data](Output/four_pca_data_elbow_curve.png)

(iv) a composite EC showing EC for (ii) and (iii) above-

![EC Composite](Output/six_elbow_curve_comparison.png)


(b) Scatter plots were used to:

(i) Clusters for Price Change Percentage at 24 hours versus 7 days-

![24 v. 7 Clusters](Output/three_df_market_data_scaled_predictions_scatter_plot.png)

(ii) Optimized Clusters after PCA completed-

![Optimized Clusters](Output/five_crypto_clusters_scatter_plot.png)

(iii) a composite of (i) and (ii) above-
![Clusters Side by Side](Output/seven_cluster_comparison.png)



**(5) Results and Analysis:**

This exercise allows for answers to the following questions:

(a) After scaling the original dataset, what is the best value for k, including using an EC for visualization? 

_Four (4) appears to be the best value for k._

(b) After optimizing the Clusters using PCA, what is the total explained variance of the three principal components? 

_Approximately 89.5% is the total explained variance._

(c) 

(i) When using the PCA data, what is the best value for k? 

_The best value for k is 4 for the PCA data._

(ii) Does it differ from the best k value found using the original data? 

_No, they are both 4._

(d) After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means? 

_The impact of using fewer features to cluster the data (using K-Means) is that a more distinct and tighter area on the plot for a majority of the points plotted at or near the origin (0, 0). Regardless of the features used, there are still plotted plots that are quite distant and thus, need to be considered as clusters (along with other plotted points). Setting k to 4 (k=4) seems justified as a result of this Cluster Comparison._


**(6) Ethical Considerations:**

There don't seem to be any ethical considerations with this dataset as its presented. Cryptocurrency information is available online and percent change calculations can be performed on publically available data.


**(7) Instructions for Interacting with the Project:**

(a) Python code is stored in the main folder as "crypto_clustering_roop.ipynb"

(b) Dataset is stored in the Resources folder as "crypto_market_data.csv"

(c) Visualizations are stored in the Output folder, with individual file names


**(8) Citations:**

(a) Details on hover_cols at https://discourse.holoviz.org/t/add-an-extra-field-when-hovering-in-hvplot-scatter/2331/2

(b) Composite plots at https://hvplot.holoviz.org/user_guide/Plotting.html

(c) Xpert Learning Assistant provide feedback on:

(i) Code syntax

(ii) Composite plots






