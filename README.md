# Group-detection
Under the impact of COVID-19, keeping social distancing is very important. We use smartphone to recognize that wether the two people are close to each other.
## System Flow
Recording videos to simulate people's sight. Use YOLOv4 to get the bounding box of items in every frame. Train a machine learning model by the position data between two people (video). Recognize the position relationship.

  <img src=./demo.png width=80% />
  
## result
We have three label for position relationship. Using three classifier to train it.

1. KNN 

  <img src=./result/1.png width=80% />
  <img src=./result/2.png width=80% />
  
2. Random Forest

  <img src=./result/3.png width=80% />
  <img src=./result/4.png width=80% />
  
3. XGB boost

  <img src=./result/5.png width=80% />
  <img src=./result/6.png width=80% />

High training/valid accuracy but low testing accuracy.
We assume this model is overfitting.
