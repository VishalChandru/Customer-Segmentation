## Customer Segmentation using K-Means and PCA (Principal Component Analysis)
- **Goal** - What problem to solve?  <br>
  - In the business context, understanding customers is crucial. This project focuses on **customer segmentation analysis using the KMeans unsupervised learning method**. The objective is to categorize customers into distinct groups based on various characteristics and behaviors, aiming to uncover unique needs and pain points within each segment. The ultimate goal is to provide **actionable recommendations** aligned with the specific preferences and characteristics identified in each customer segment
- **ML approach**?
  - For clustering, the unsupervised **KMeans** method will be employed. While other clustering methods could be considered, because lots of analysis happens post-modeling for this project, I will only focus on KMeans for simplicity. 
    
  - Since KMeans is vulnerable to curse of dimensionality, we will do lots of **feature selection/engineering** including **PCA**.  
    
    
- **Model tuning for unsupervised learning**?
  - Unsupervised learning don't have labels. In this project, tuning happens in the following areas:
    
    - **Scaling**: although technically not tuning, scaling is key for KMeans performance. With the help of PCA visualization, a comparison of MinMax and Standard scaling will be conducted.
    
    - **PCA Dimensions**: will be determined using variance analysis, principal component coefficients analysis, and consideration of business interests. 
    - **Number of Clusters**: will be determined using elbow method with a practical analysis based on resutling clustering groups.