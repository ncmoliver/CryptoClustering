
# ¢rypto ¢lustering ₳nalysis
![Crypt Analysis Logo](/images/readme_img.png)

# ௹verview
This project involves analyzing cryptocurrency market data using two approaches:   
1. The Original Dataframe
2. After Applying PCA     
The main goal was to determine the best number to use as the number of clusters (k) for both the original and PCA transformed dataset, using the elbow method and then performing KMeans clustering based on the recommended value for k. The analysis revealed the same results in the suggested optimal number of clusters when comparing the two sets of data.
# ₣iles ₺n ₸his řepository
* ***'Crypto_Clustering.ipynb'***: The Python script used to perform PCA, Standardscaler, and Kmeans clustering.   
* ***'orignal_elbow_curve.png'***: The elbow curve plot for the orignal datframe. 
* ***'PCA_elbow_curve.png'***: The elbow curve for the PCA tranformed data.   
* ***'orignal_k_cluster.png'***: The resulting clustering from the KMeans applied to the original data.    
* ***PCA_k_cluster.png'***: The resulting clusters from KMeans applied to the PCA tranformed data.
# ₺nstallation
This is a Jupyter Notebook, which is the recommended IDE for this program. 

| Installation Step | Description |
| ----------- | ----------- |
| Step 1 | Clone this repository `git clone https://github.com/ncmoliver/CryptoClustering.git` |
| Step 2 | In your terminal, change directory to the `CryptoClustering` project folder.  |
| Step 2 (example command) | ` cd CryptoClustering` |
| Step 3 | Pandas, sklearn (KMeans, PCA, StandardScaler) |
| Step 3 (example command) | `pip install -r requirements.txt` |
| Step 4 | Run the program and Enjoy ⭐️ |

# ₩orkflow
### 1. Data Preprocessing
**Original Data:** The raw cryptocurrency data was cleaned and preprocessed. This includes handling missing values and standardizing the features (columns) to ensure a fair comparison.
**PCA Transformed Data** The data was transformed using PCA to reduce dimensionality. The first three principal components (PCA1, PCA2, PCA3) were used for further analysis. PCA helped capture the most significant patterns in the data with minimal loss of information. 
### 2. Elbow Curve Analysis
**Original Data** The elbow curve found the optimal number for k to be 4, which indicates that the orignal data groups best into 6 clusters.
**PCA Transformed Data** The elbow curve also found the optimal number of k to be 4.    
### 3. KMeans Clustering
**Original Data** KMeans was applied to the original data with k=6. The resulting clusters grouped the cryptocurrencies based on similar patters across the original features (columns).    
**PCA Data** KMeans was also applied to the PCA-transformed data with k=8. This provided a different perspective clustering data based on the most significant principal components from the original data. 
## 4. Analysis of PCA Components
**PCA1:** The largest amount of variance in the data was heavily influenced by the 200 day price change.    
**PCA2** The largest amount of variance in PCA2 data was heavily influence by the 30 day price change.
**PCA3:** The largest amount of variance in PCA3 data was heavily influenced by 7 day price change.

# 𝖗esults
The original data elbow curve recommended k=4 resulting in 4 distinct clusters. The clusters reflect patterns based on the original dataset. Where after applying PCA the elbow curve also suggested k=4, reflecting the tranformed PCA dataset.

# Ŗeferences

[Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)    

