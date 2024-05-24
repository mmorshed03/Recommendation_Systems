Link to data: https://drive.google.com/drive/folders/1lJ1VhRM7MUHmhCt9a3xPWvxFTAD1SqYL

In this case study,a recommendation system is built using four different algorithms. They are as follows:
  - Rank-based using averages
  - User-user similarity-based collaborative filtering
  - Item-item similarity-based collaborative filtering
  - Model-based (matrix factorization) collaborative filtering

To demonstrate **"user-user similarity-based collaborative filtering", "item-item similarity-based collaborative filtering", and "model-based (matrix factorization) collaborative filtering"**, **surprise** library has been used. For these algorithms, **grid search cross-validation is used to find the optimal hyperparameters for the data**, and improve the performance of the model**.
**For performance evaluation** of these models, **precision@k and recall@k** are used. Using these two metrics, the F_1 score is calculated for each working model. 
Overall, the **optimized user-user similarity-based recommendation system** has given the **best performance** in terms of the F1-Score (~0.86)
- Collaborative Filtering searches for neighbors based on similarity of books (example) preferences and recommend books that those neighbors read while Matrix factorization works by decomposing the user-item matrix into the product of two lower dimensionality rectangular matrices.
- Matrix Factorization has lower RMSE (1.50) due to the reason that it assumes that both books and users are present in some low dimensional space describing their properties and recommend a book based on its proximity to the user in the latent space. Implying it accounts for latent factors as well.
- We can try to further improve the performance of these models using hyperparameter tuning. 
- We can also try to combine different recommendation techniques to build a more complex model like hybrid recommendation systems.
