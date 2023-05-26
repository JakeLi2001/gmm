# Handwritten Digit Recognition

**Goal**: Explore how to implement Gaussian Mixture Model (GMM) as a density estimator algorithm, as a classifier, and as a generative model.

**Note**: This is my take-home final for my machine learning class MTH 4330.

## :mag_right: Data Sources: Scikit-learn datasets.
- [Two moons](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_moons.html)
- [Handwritten Digits](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_digits.html)

## :open_book: Summary

1. Gaussian Mixture Model as density estimator algorithm.
- Generate 3000 points with a noise of 0.1 from `sklearn.datasets.make_moons`.
- Build two component GMM and plot the level sets.
- Use `GridSearchCV` to find the best number of components with BIC criterion.
2. Gaussian Mixture Model as a classifier.
- Build GMM and assign components to a label.
- Plot components and points along with their assigned labels.
- Build for loop to find out the best number of components using accuracy as the criterion.
3. Gaussian Mixture Model as a generative model.
- Import the MNIST dataset from `sklearn.datasets.load_digits`.
- Perform principal component analysis to reduce dimension.
- Build GMM similar to part 2 and assign each components to a digit. 
- Generate sample points from the GMM and use PCA to inverse transform the points back to the original dimension.
- Plot those digits and see if they look like handwritten digits.
- Test GMM performance by building another classification model and see if it can classify the genereated digits correctly.

## :dart: Results

See [report](Final Report.docx).

## :hammer_and_wrench: Tech Stack

**Language:** Python

**Libraries:** Numpy, Pandas, Scikit-learn, Seaborn, Scipy

**Tool:** Jupyter Lab
