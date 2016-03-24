Predict the cuisine to which a recipe belongs based on its ingredients.

We used a bag of words model for the ingredients. we used PCA to reduce the number of features to 1150. We extended the feature vector by adding 20 more features wherein each feature corresponds to one cuisine. Firstly, we find the set ingredients corresponding to every cuisine. 

Let I be the set of ingredients in a recipe. Let $I_c$ be the set of all ingredients corresponding to cuisine c. Now the feature corresponding to cuisine c is $|I \cap I_c|$.

The feature vector was extended further by adding 20 more features similar to the previous 20 features. In this case, the feature corresponding to a particular cuisine represented the number of signature ingredients of that cuisine present in the recipe.

Finally, we used this 1190 dimensional feature vector to perform our prediction task.