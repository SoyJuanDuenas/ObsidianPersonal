Contiguity refers to the state or quality of being contiguous, which means being in direct contact, touching, or adjacent to something else. It implies the spatial or geographical proximity of points or polygons that share a common boundary or are next to each other. In various contexts, contiguity can refer to physical proximity, temporal proximity, or even conceptual proximity. In the context of spatial analysis or [[spatial econometrics]], contiguity often involves neighboring regions or spatial units that share common boundaries and can influence each other. 

# Spatial Weights Matrix or Contiguity Matrix

One of the crucial operations in spatial econometrics is to formally express spatial dependencies in order to incorporate them into a model. For this purpose, we assume that the observations are organized as spatial data, which can be points in a regular or irregular area, or alternatively, regions on a map.

To achieve this, we introduce the concept of Spatial Weights Matrix or Contiguity Matrix. Consider a system S of N spatial units, numbered i = 1, 2, 3, ..., n, and an observable variable x for each of these spatial units.

$$
W = \begin{equation}\begin{bmatrix}w_{11} & w_{12} &  ... & w_{1n}\\w_{21} & w_{22} & ... & w_{2n} \\ ... & ... & ... & ...\\ w_{n1} & w_n2 & ... & w_{nn}\end{bmatrix}\end{equation}
$$
Where each element of this contiguity matrix are defined as:
$$
w_{ij}= \left\{ \begin{array}{lcc} 1 &   si  & j \in N(i) \\ 0 &  si &j \notin N(i)  
\end{array} \right.
$$

Here, N(i) represents the set of neighbors of location j. Therefore, the matrix W is a non-stochastic square matrix whose elements "w" reflect the contiguity between the spatial data. Each element "1" in the matrix corresponds to contiguity between spatial units. As a convention, spatial data cannot be contiguous with itself, resulting in a main diagonal of zeros.

To define the matrix W, we can use different criteria regarding the set of neighbors for a location. Usually, we resort to physical contiguity criteria, leading to three main types of criteria:
## Physical-based Contiguity

### Rook Criterion

The rook criterion defines neighbors as spatial observations or data sharing any spatial side. One can imagine the movements of a chess rook.
### Queen Criterion

The queen criterion defines neighbors as spatial observations or data sharing any spatial boundary. Similar to the previous example, one can imagine the movements of a chess queen.
### Bishop Criterion

The bishop criterion defines neighbors as spatial observations or data sharing diagonal boundaries. Again, one can envision the movements of a chess bishop.
## Distance-Based Contiguity

The three previous criteria are easily applicable to regular polygons. However, most polygons are irregular, making physical contiguity restrictive. Therefore, we turn to criteria based on distance, where distance can be calculated in different ways:

- [[Euclidean distance]]
- [[Manhattan distance]]
- [[Minkowski distance]]

### K-Nearest Neighbors (KNN)

In KNN, we obtain a binary matrix in which we generate centroids for each spatial polygon and calculate the distance between the centroid of our target polygon and the centroids of the other polygons. We organize them and consider the k nearest polygons as contiguous.

$$
w_{ij}= \left\{ \begin{array}{lcc} 1 &   if  & \text{the centroid of j is one of the k nearest centroids to i} \\ 0 &  if & \text{otherwise}  
\end{array} \right.
$$

### Distance-Based Threshold / Radius

In distance-based threshold or radius, we obtain a binary matrix where, based on the researcher's criterion, we consider contiguous if the distance between centroids is below a certain range.

$$
w_{ij}= \left\{ \begin{array}{lcc} 1 &   if  & \text{the distance between j and i is less than a given distance} \\ 0 &  if & \text{otherwise}  
\end{array} \right.
$$

### Inverse Distance

With inverse distance, we do not obtain a binary matrix; instead, our non-zero parameter changes based on the inverse distance. That is, the greater the distance, the lower the parameter, and vice versa. In this criterion, we can control the level of decline of distance influence with a parameter alpha, as follows:

$$
w_{ij}= \left\{ \begin{array}{lcc} \frac{1}{d^{\alpha}} &   if  & i \neq j \\ 0 &  if & i = j  
\end{array} \right.
$$

## Standardized Spatial Weights Matrix

Sometimes we need to standardize the matrix W, and this standardization corresponds to the following row operation:

$$
w^{*}_{ij} = \frac{w_{ij}}{\sum w_{ij}}
$$

where

$$w^{*}_{ij} \in W^{*}$$

In other words, each standardized element of the spatial weights matrix corresponds to the division between 0 or 1 and the sum of elements related to that row. This would be the percentage of total relations for each row.

This standardization can be very useful in some instances. For example, using the standardized spatial weights matrix, we can operate with spatial lags.

## Spatial Lag Operator

One of the objectives of using spatial weights matrices in specifying a spatial econometric model is to relate a variable at one point in space to observations for that variable among other spatial units in the system. In the context of time series, this is known as a lag operator in the form:

$$
y_{t-k} = L^{k}y
$$

In space, we do not have a temporal dimension but a geographical dimension. Depending on the type of criterion chosen, we will obtain a different spatial lag. To calculate the spatial lag, we use:

$$
\rho = W^{*}Y
$$

With a queen-type matrix, we obtain a lag as follows:

![Queen Spatial Lag](Retardo%20Espacial%20Reina.png)

While with a rook-type matrix, we obtain a lag as follows:

![Rook Spatial Lag](Retardo%20Espacial%20Torre.png)