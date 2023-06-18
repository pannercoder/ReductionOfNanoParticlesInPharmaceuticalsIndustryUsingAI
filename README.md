# ReductionOfNanoParticlesInPharmaceuticalsIndustryUsingAI
Reduction Of Nano Particles In Pharmaceuticals Industry Using AI

import numpy as np
from sklearn.cluster import Kmeans
def reduce_nanoparticles(data, num_clusters):    
      # Perform k-means clustering    
       kmeans = KMeans(n_clusters=num_clusters)   
       kmeans.fit(data)    
      # Get cluster assignments    
      cluster_labels = kmeans.labels_    
      # Calculate the centroid of each cluster    
      centroids = kmeans.cluster_centers_    
      # Replace each nanoparticle with the centroid of its assigned cluster
      reduce d_data = centroids[cluster_labels]
      return reduced_data
