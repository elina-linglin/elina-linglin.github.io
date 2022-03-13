---
layout: posts
title: "Cost Complexity Pruning -- A Clear Explanation!"
description: ""
comments: true
---

The key idea of this method is to: 

1. Find a limit on the complexity (represented by $\alpha$) to find a balance between overfitting and generalization.   

= hyper-parameter tuning. alpha is the hyper-parameter

2. Use this hyper-parameter to find the best subtree. 

### Step 1

Divide data into training and test sets. Put the test data aside as they are used only at the end of this article. 

### Step 2

Use the training set to grow a large tree (a.k.a the full tree) using recursive binary splitting. 

### Step 3

Apply cost complexity pruning to obtain a sequence of the best subtree as a function of $\alpha$. 

And now I will explain how cost complexity pruning works. 

- Imagine there is a pool of all the possible subtrees from the full tree.
