# Bias-Variance Model Selection In-Depth

## Table of Contents

- [Introduction](#introduction)
- [Environment Setup](#environment-setup)
- [Installation Instructions](#installation-instructions)
- [Evaluation](#evaluation)
- [Resources](#resources)
- [License](#license)
- [Conclusion](#conclusion)
- [About Author](#about-author)

## Introduction

Join me on a journey through the intricate landscape of model selection, bias, and variance. Through a series of illuminating examples, we delve into the concepts of overfitting and underfitting using polynomial data and uninformative features, providing a nuanced understanding of model complexity.

Uncover the fundamental principles of bias and variance and their implications for linear regression and beyond. Through practical demonstrations, gain insights into how these factors shape the performance and robustness of machine learning models.

Explore advanced model selection techniques, including K-Fold Cross-Validation and the 1-SE rule to navigate the delicate balance between bias and variance. Equip yourself with the knowledge and tools needed to make informed decisions when selecting models that best fit your data and objectives.

#### Attribution

Parts of this notebook borrow from, or are inspired by, the following
sources:

-   The Introduction section is based on [Hyperparameters and Model
    Validation](https://jakevdp.github.io/PythonDataScienceHandbook/05.03-hyperparameters-and-model-validation.html),
    in the Python Data Science Handbook by Jake VanderPlas
-   The section on polynomial models is based on [the model order
    selection demo
    notebook](https://colab.research.google.com/github/sdrangan/introml/blob/master/unit04_model_sel/demo_polyfit.ipynb)
    by Prof. Sundeep Rangan, and some of the text in that section is
    copied from that notebook.
-   The section on uninformative features is based on [Cross Validation:
    The Right and Wrong
    Way](http://nbviewer.ipython.org/urls/raw.github.com/cs109/content/master/lec_10_cross_val.ipynb)
    from [Harvard CS109 Data Science](https://github.com/cs109/content)
-   The simulation plots are based on the `scikit-learn` example [Single
    estimator versus bagging: bias-variance
    decomposition](https://scikit-learn.org/stable/auto_examples/ensemble/plot_bias_variance.html#sphx-glr-auto-examples-ensemble-plot-bias-variance-py)

## Environment Setup

**Prerequisites**: Ensure Python 3.6 or newer is installed on your system.

1. **Create a Virtual Environment**:
    - Install `virtualenv` if you prefer it over the built-in `venv` (optional):
        ```bash
        pip install virtualenv
        ```
    - Create the environment:
        - With `venv` (Python 3.3+):
            ```bash
            python -m venv env
            ```
        - Or, with `virtualenv`:
            ```bash
            virtualenv env
            ```
    - Activate the environment:
        - Windows: `env\Scripts\activate`
        - Unix/MacOS: `source env/bin/activate`
    - To deactivate: `deactivate`

2. **Dependencies**:
    Ensure all dependencies are listed in `requirements.txt`. Install them using:
    ```bash
    pip install -r requirements.txt
    ```

## Installation Instructions

To use this project, clone the repository and set up the environment as follows:

1. **Clone the Repository**:
    ```bash
    https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth.git
    ```
2. **Setup the Environment**:
    - Navigate to the project directory and activate the virtual environment.
    - Install the dependencies from `requirements.txt`.


## Evaluation

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/e7cff7f8-0dc7-406d-b46f-9686c04dda59)
This is an example of under-fitting or under-modeling. The estimated function is not able to capture the complexity of the relation between  x and  y - it is not flexible enough.

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/bb9fad55-a952-479a-b27a-1bd547a4e751)
This is called over-fitting or over-modeling. Because the model is very flexible, it is fitting the noise in the data and not the underlying relationship  y=t(x).


The following plot shows the coefficient value for each feature:
![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/8253fbb7-59e8-4a13-8c56-8897d6792b54)

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/b4d64d4f-e074-4b75-ac5c-aa5f97921e1e)

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/7acea43b-af85-4c14-99ba-064c65c46ca4)

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/84c7268b-4920-4363-be01-66d16caf6401)


### Model selection using best K-Fold CV score

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/82ca66ab-1ec4-412f-8302-c0185cfc0514)

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/90527a0a-4832-4660-9c28-3dfb69e6f038)

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/e7323127-08dc-4fad-87c7-e86985dcf48e)

### Model selection using 1-SE rule

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/1852a966-656d-4778-bae0-529b72f4a3a0)

![image](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth/assets/149146155/30bb7448-0112-49d2-aef8-260d141225da)







## Resources

- **Kaggle Notebook**: [View Notebook](https://www.kaggle.com/code/muhammadimran112233/bias-variance-model-selection-in-depth)

## License

This project is made available under the MIT License.

## Conclusion

Through this in-depth exploration of bias-variance model selection, we've uncovered the intricate dynamics shaping machine learning performance. Armed with insights into bias, variance, and model complexity, we've navigated the terrain of overfitting and underfitting with practical examples. By using advanced techniques like K-Fold Cross-Validation and the 1-SE rule we've honed our ability to select models optimized for real-world performance. Equipped with this knowledge, we're prepared to navigate the complexities of machine learning, ensuring our models strike the ideal balance between bias and variance for reliable results.

## About Author

- **Name**: Muhammad Imran Zaman
- **Email**: [imranzaman.ml@gmail.com](mailto:imranzaman.ml@gmail.com)
- **Professional Links**:
    - Kaggle: [Profile](https://www.kaggle.com/muhammadimran112233)
    - LinkedIn: [Profile](linkedin.com/in/muhammad-imran-zaman)
    - Google Scholar: [Profile](https://scholar.google.com/citations?user=ulVFpy8AAAAJ&hl=en)
    - YouTube: [Channel](https://www.youtube.com/@consolioo)
- **Project Repository**: [GitHub Repo](https://github.com/Imran-ml/Bias-Variance-Model-Selection-In-Depth.git)
