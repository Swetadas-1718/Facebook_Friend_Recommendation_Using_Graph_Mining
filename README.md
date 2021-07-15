# Facebook Friend Recommendation Using Graph Mining

![Sierralane Architects (1)](https://user-images.githubusercontent.com/71088477/125852290-3881d50b-763d-4be1-acef-4026c0b4158d.png)

https://github.com/Swetadas-1718/Facebook_Friend_Recommendation_Using_Graph_Mining/blob/main/Sierralane%20Architects%20(1).png

## Still amazed at how accurate the "people you may know" thing on Facebook is?

## Real-World Problem
- Here, we present each user of a social network with a dot called node/vertex and we connect people who are friends/followers/connections with edges called links. So this whole thing in computer science and applied mathematics is called graphs.
- In Facebook, you must have encountered the recommendation which is known as a friend recommendation, and similarly, in Instagram, it is known as a follower recommendation.
- Given the graph, we take the help of already existing links. Here, u5 is a friend of u3 and u3 is a friend of u1. Now, Is it sensible to assume that u5 could be a friend of u1?

## Problem statement:
Given a directed social graph, we have to predict missing links to recommend friends/connnections/followers.

## Data Overview
- Dataset from facebook's recruting challenge on kaggle: https://www.kaggle.com/c/FacebookRecruiting
- Data contains two columns:
  - source node
  - destination node
- We are given directed graph data.

## Mapping the problem to supervised learning problem:
- We will generate edges which are not present in the existing graph for supervised learning.
- Remember,we will consider and generate only those bad links for graph which are not in the graph & whose shortest path is greater than 2.
- We want to convert this into a binary classification problem as discussed before such that existing edges are labelled as "1" and non existing edges or absent edges are labelled as "0".

## Business Constraints & Metrics
- No low-latency requirements
- We will recommend the highest probability links to a user, so we need to predict the probabilities of the links which are useful.
- Ideally, We want high Precision and high Recall when we are recommending Uj to Ui.

## Performance Metric for Supervised Learning
- Both precision and recall are important, hence F1 score is a good choice here.
- Confusion matrix

## Author
- Swetapadma Das
