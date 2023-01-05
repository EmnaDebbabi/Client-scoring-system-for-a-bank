# Client-scoring-system-for-a-bank

https://user-images.githubusercontent.com/47029962/210796748-d6ebc199-b1e8-40fa-891e-8b89c6c0a300.mp4

## Project’s Context

In order to be connected to its clients, banks need to think
differently about how to manage its data and incorporate it into its
professional practices.
Our mission is to analyze,
predict and find patterns within data by creating a platform to help
them make careful decisions about their clients.
Thus, our task is to model and implement an autonomous
multi-criterion matching engine and a dashboard to provide an
objective view of performance metrics for each client.

## Data Analysis and data visualization

### DataSet Preparation

In this phase we began by preparing our datasets, to achieve this
goal we went through several steps. Each dataset represents number of
account of clients from a bank that we will explain in the next
paragraph.

We have 3 types of banks American, Germain and Taiwan.


For each dataset we counted to clean up the data which include:
<ol>
<li> Removing extraneous data and outliers. </li> 
<li> Filling in missing values. </li>
<li> Conforming data to a standardized pattern. </li>
<li> Masking private or sensitive data entries. </li>
</ol>

Once data has been cleansed, we move to predictive
modeling where machine learning comes into our data science project.
We use the term predictive modeling because a good project is not one
that just trains a model and obsesses over the accuracy, but also uses
comprehensive statistical methods and tests to ensure that the
outcomes from the model actually make sense and are significant.

And finally once you’ve derived the intended insights from your
model, you have to represent them in a way that the different key
stakeholders in the project can understand.

### Data Preparation:

In any natural language processing task, cleaning raw text data
is an important step. It helps in getting rid of the unwanted
words and characters which helps in obtaining better features.
If we skip this step then there is a higher chance that you are
working with noisy and inconsistent data.

<ul>
<li>
<li> PCA :

Principal Component Analysis is a technique used for
identification of a smaller number of uncorrelated variables known
as principal components from a larger set of data. </li>

<li> Check for Missing Values  </li>

<li> Cleaning / Filling Missing Data either with median, mean or
most frequent value.  </li>
<li> Drop Missing Values.  </li>
</ul>
Once we finish cleaning up the data we move to encoding
categorical values we use a technique called label encoding or one
hot encoding it depends with the number of categorical values .
### Modeling:
#### Segmentation:

In order to create our segments, we thought of using K-means,
but the inconvenience is that in this algorithm we need to fix at
first the number of clusters in advance. To solve this problem, we
decided to use Elbow at the first step so we can determine the most
favorable number of clusters.
<ul>
<li> Elbow :

The Elbow method helps to select the optimal number of

Clusters by fitting the model with a range of values for K.
We applied Elbow method on our dataset and we got the
result shown in the figure below .
After applying Elbow now, we can cluster our dataset using
K-Means algorithm. </li>
<li> K-Means:

K-Means algorithm is an iterative algorithm that tries to
partition the dataset into Kpre-de_ned distinct non-overlapping
subgroups (clusters). </li>

<li> CAH:Hierarchical Clustering:

We can also use Hierarchical Clustering (CAH).By plotting the
Dendrogram we confirm the result we found in K-Means using
Elbow, where the perfect number of cluster (maximizing inter class
and minimizing intra class).</li>
</ul>

#### Classification:

Classification will serve the purpose of knowing where to classify
any new client in the number of segment that we already created
in the previous phase.

<ul>
<li> KNN:

Now , we tried KNN(nearest neighbor) method to find
the suitable model for our dataset. </li>

<li> CART:

CART is a decision tree where each fork is a split in a predictor
variable and each end node contains a prediction for the outcome
variable. </li>
</ul>

### Evaluation:

In this example Random Forest presents the most higher accuracy
which indicates that it is the best performance model

![image](https://user-images.githubusercontent.com/47029962/210827026-b99a0145-e1f5-4849-bfc3-1e50666d8d2a.png)

### Conclusion

Our solution allows our three banks to better understand
their clients behaviors to have an idea about them.
