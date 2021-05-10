# A-Feature-Engineering-Approach-To-Improve-Plant-Species-Classification-From-Leaf-Images

Plants play an important role in everyone’s life.It
is time consuming to manually collect information
on unknown plants, such as going to the local
nursery, reading books, or writing on the Internet.
Automatic plant identification system is therefore
of great importance to facilitate and speed up the
process.Plants are identified by their organic
characteristics, such as flowers, leaves, roots, or the
whole plants. After some research, it is understood
that leaves is origin of characteristics to identify a
plant species. A collection of features must be
extracted to use a leaf as a discriminating feature
of a plant. It is possible to extract features from a
leaf image from its form, colour and texture. 
Ourinterests in identifying the leaf species using an image
by applying image processing techniques drove us to understand the techniques, the cruxes of leaf features.

The current state of art in Image Classification
is Convolution Neural Networks(C-NN). Many
papers that were published illustrated the accuracy rate
for identifying the leaf image is quite high using CNN,
however, we have studied other Machine Learning
Algorithms in this project because they are still the
current state of art in the field. Algorithms like Support
Vector Machine(SVM),K-Nearest Neighbour(KNN),Random Forest(RF), Probabilistic Neural
Network(PNN) are implemented in this project.
We have studied the review project titled ”Image
Classification Techniques in Plant Leaf Species
Recognition” using the above classification algorithms.
These Algorithms provide the accuracy percentage (%
) using Flavia Dataset, LeafImage Dataset from UCI
Machine Learning repository. We have analyzed
and interpreted the limitations and advantages of each
algorithm. The maximum and minimum accuracy rate
is observed for SVM[1] and RF algorithms with
91.2% and 88.0% accuracy rate respectively.

We learned that accuracy recognition of a leaf depends
on Feature extraction from the image.In our
research project, the features extracted by processing
an image is obtained from the shape, color, and texture
of the leaf. Here the overall features extracted
from a leaf image are 17 features. Under these features,
the shape has 7 geometrical features, color and
texture have 6 and 4 features respectively.We have used different
combinations of these 17 features and trained with the
image classifiers. Later, we compared the accuracies
achieved on the test dataset by using every possible
combination of those extracted features. These obtained
accuracies enabled us to identify which feature
or combination of features are more important and
contribute strongly to classify one leaf species from
another species.

However, we explored other features
that we could train in the SVM Algorithm in Python
development environment, we found other features like
Hu Moments[8], Zernike moments[10], vein features
and other local features like Scale Invariant Feature
Transform (SIFT)and Speeded Up Robust Features
(SURF)[11]. Out of all these features we studied the
Hu Moments which are similar to Shape features in
a leaf like area, perimeter, circularity, etc which are
called Shape-descriptors for Hu Moments


![image](https://user-images.githubusercontent.com/55109738/117735089-ce6db480-b1c2-11eb-9c89-dc92722eddfd.png)

Block Diagram of Hu Moments

![image](https://user-images.githubusercontent.com/55109738/117735130-e5140b80-b1c2-11eb-9376-1110eb995c9c.png)

Binary Image of a Leaf

![image](https://user-images.githubusercontent.com/55109738/117735430-6c617f00-b1c3-11eb-89f1-27054e636cbe.png)

Training of Hu Moments

![image](https://user-images.githubusercontent.com/55109738/117735496-89964d80-b1c3-11eb-9157-18854d2b9bf5.png)

Comparison Graph for Algorithms with and
without Hu Moments


After performing the experiments and training the
classifier on various combinations of extracted features,
we got to know from our analysis that the shape
and texture features of leaf proves to be the most
contributing features to classify plant species. We also
found out that using Hu Moments as shape descriptors
instead of the geometrical shape features yield better
performance in identifying plant species because of
its consideration of pixel intensities which proves to
be more effective. From our results, we can deduce
that there is still a room for improvement in the
plant species classification task by focusing more on
feature engineering.

