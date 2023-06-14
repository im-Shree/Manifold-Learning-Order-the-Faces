## Manifold Learning:
  
  Manifold learning, also known as nonlinear dimensionality reduction. <br>
  It is a set of techniques used to uncover the underlying structure or geometry of high-dimensional data in a lower-dimensional space. <br>
  It aims to preserve the essential characteristics of the data while reducing its dimensionality.<br>

  The dataset (face.mat) contains 33 faces of the same person in different angles.<br>
  Then we will use different manifold algorithms to manipulate dimensionality and order <br>
  
![org](https://github.com/im-Shree/Manifold-Learning-Order-the-Faces/assets/90651908/2b19381b-30a0-4bf0-b439-bd2b83d2fe22)
the faces.
  

##  MDS embedding
  We perform Multidimensional Scaling (MDS) on the input data X using a specified number of components (component).<br>
  The MDS algorithm aims to reduce the dimensionality of the data while preserving the pairwise distances between the samples.<br>
  The resulting MDS embeddings are stored in the faces_mds variable after fitting the MDS model with a maximum of 2000 iterations and a single initialization.<br>

![MDS](https://github.com/im-Shree/Manifold-Learning-Order-the-Faces/assets/90651908/77bc7c11-d95c-43c3-9803-e1cf6b0fa021)


##  ISO Map Embedding
  We performs Isomap embedding on the input data X using a specified number of neighbors (n_neighbors) and components (component)..<br>
  Isomap is a nonlinear dimensionality reduction technique that constructs a low-dimensional representation of the data by preserving the geodesic distances between samples on a manifold..<br>
  The resulting Isomap embeddings are stored in the face_isomap variable after fitting the Isomap model with a maximum of 2000 iterations.<br>
  
  ![ISO](https://github.com/im-Shree/Manifold-Learning-Order-the-Faces/assets/90651908/05b4cb0a-aae0-41e7-af72-9c8ecfa4ae3a)


##  LLE Embedding
  We performs Locally Linear Embedding (LLE) on the input data X using a specified number of components (component) and neighbors (n_neighbors). <br>
  LLE is a nonlinear dimensionality reduction technique that aims to preserve local relationships between neighboring samples.<br>
  The LLE model is initialized with parameters such as the maximum number of iterations (max_iter), eigen_solver, and method.<br>
  The resulting LLE embeddings are stored in the face_lle variable after fitting the LLE model with a maximum of 2000 iterations.<br>

![LLE](https://github.com/im-Shree/Manifold-Learning-Order-the-Faces/assets/90651908/cafb5c45-ae40-4c36-bb9e-bd1699ffc3ad)


##  Spectral Embedding
We performs Spectral Embedding on the input data X using a specified number of components (component). <br>
Spectral Embedding is a technique for dimensionality reduction that maps the data into a lower-dimensional space using the eigenvectors of a graph Laplacian matrix.<br>
The SpectralEmbedding model is initialized with parameters such as affinity (set to 'nearest_neighbors' for using k-nearest neighbors graph), gamma, random_state, eigen_solver, n_neighbors, and n_jobs.<br>
The resulting Spectral Embedding embeddings are stored in the face_Le variable after fitting the model to the input data X.<br>

![SE](https://github.com/im-Shree/Manifold-Learning-Order-the-Faces/assets/90651908/d088bdcc-257f-416a-8b02-a0cf4de2f505)


