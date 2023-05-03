---
title: "Introduction to Decision Trees"

---


Decision trees are a popular machine learning algorithm used for classification and regression. In this post, I give an introduction to decision trees. I used <a href="https://www.youtube.com/@DataTalksClub">DataTalksClub</a> as my main resource, and I highly recommend their channel.


<h1>What does a decision tree look like? How do each of the parts of a decision tree correspond to a dataset?</h1>

<div class="container">
  <p>A real-life tree consists of branches, roots, and leaves. </p>
</div>
  

  
<img src="https://user-images.githubusercontent.com/125330688/235809811-e27f37c8-f391-4840-95d2-53e971937b64.png" alt="legit_tree" width="400">


<div class="container">
  <p>Similarly, a decision tree consists of branches, a root node, internal nodes, and leaves. Consider the following table regarding cats: </p>
</div>



<img src="https://user-images.githubusercontent.com/125330688/235816220-899ce3b6-52cf-418a-9e25-879ef7c73573.png" alt="cats" width="400">

<div class="container">
  <p>This dataset consists of four cats, each with four features. We don't have a target in the dataset, but let's say we want to predict whether a cat is "default" or "okay". </p>
</div>

<img src="https://user-images.githubusercontent.com/125330688/235816672-6ceb6da9-155a-4a8e-96d1-40557d9b6360.png" alt="decision1" width="400">


<div class="container">
  <p>We will start with a condition which asks whether or not the cat is neutered. This is called the "root node". There is only one root node.</p>
</div>
  
<img src="https://user-images.githubusercontent.com/125330688/235816891-49eb8750-593b-496e-9a7e-d6db563a8ee8.png" alt="decision2" width="400">


<div class="container">
  <p>From our chart, three cats are neutered and one is not neutered. The three neutered cats will go down the "True" branch and the one non-neutered cat will go down the "False" branch. </p>
</div>

<img src="https://user-images.githubusercontent.com/125330688/235817483-99c70036-9ad4-4c24-a704-f4cc80a56657.png" alt="decision3" width="400">

<div class="container">
  <p>Next, we have two "internal nodes". On the left branch, we have our one non-neutered cat, and we will check whether the cat satisfies the condition "Whiskers>2 inches". On the right branch, we have our three neutered cats. For each of these cats, we will check whether the cat satisfies the condition "fur length=long". The internal node is similar to the root node in that we are checking a condition.</p>
</div>

<img src="https://user-images.githubusercontent.com/125330688/235817485-b160f385-2e37-4db3-8153-6afd966953a6.png" alt="decision4" width="400">

<div class="container">
  <p>Next, we fill in the rest of the internal nodes and branches. We have one more internal branch, "fur color=orange".</p>
</div>

<img src="https://user-images.githubusercontent.com/125330688/235817487-da809eff-b3d6-44dd-97e5-95cdbf28450d.png" alt="decision5" width="400">

<div class="container">
  <p>Our decision tree ends with the leaf nodes, which are denoted as "default" or "ok". In our specific case, we have four cats that will be classified into one of the five leaf nodes. These leaf nodes represent the final output of our decision tree and serve as our target variable. For instance, if our task is to predict if a cat will be "adopted" or "not adopted", we would label the leaf nodes accordingly.</p>
</div>




<h1>How are each of the nodes chosen? </h1>
<h1>What is overfitting and why is this an important consideration for decision trees?</h1>
<h1>What is impurity? </h1>
<h1>Decision tree learning algorithm</h1>

