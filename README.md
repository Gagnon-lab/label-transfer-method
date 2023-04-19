# scRNA-seq Label Transfer Method 

A computational method to transfer labels from a reference cell atlas to an unlabeled single-cell data set.

The method begins with two dataframes, a reference cell atlas containing the top markers that establish a cell type and the highly differentiated markers that establish each unlabeled cluster of a single-cell dataset. The computational framework was designed to compare the markers of each of the two inputs to one another in order to find the most likely cell type for each unlabeled cluster. 

Three inputs are required: the reference cell atlas, the FindAllMarkers output of a Seurat object, and the cell type column names of the reference cell atlas in its own dataframe. With just these three inputs, the computational method will determine the most likely cell type for each cluster, and displaying these identities in the form of a heatmap and a table summary.  

Final Output Examples:

<img width="312" alt="image" src="https://user-images.githubusercontent.com/82175086/232967775-84af0d98-2a15-4d38-ad46-fe3643ce898d.png">
<img width="814" alt="image" src="https://user-images.githubusercontent.com/82175086/232967893-56a5d62f-407d-4866-8871-c606059dadde.png">
