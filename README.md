# applied-statistics #

**by Finbar Dennehy** 

## Repository Overview ##

This repository primarily contains a Jupyter Notebook `problems.ipynb`, representing my project submission for the 'Applied Statistics' module as part of the HDip in Science in Data Analytics at ATU.

This project applies statistical simulation and inference techniques to classical problems in applied statistics.
The notebook demonstrates the use of Monte Carlo simulation, sampling distributions, hypothesis testing, and analysis of variance (ANOVA), with an emphasis on interpretation and reproducibility rather than purely numerical results.

The work is intended to demonstrate both statistical understanding and clean, reproducible scientific computing practices in Python.

## Repository Contents ##

- `.gitignore`: File using the Python, Windows and Mac OS gitignore templates.
- `README.md`: This README file.
- `requirements.txt`: Included in the repository for easy installation, it contains the third-party package dependencies.
- `problems.ipynb`: The notebook is structured with an initial import of all required packages, clearly labelled sections for each problem, and concluding discussion summaries where applicable.

## Problems ##

The purpose of this repo is to solve the below:

### Problem 1: Extending the Lady Tasting Tea ###

Let's extend the Lady Tasting Tea experiment as follows.
The original experiment has 8 cups: 4 tea-first and 4 milk-first.
Suppose we prepare 12 cups: 8 tea-first and 4 milk-first.
A participant claims they can tell which was poured first.  

Simulate this experiment using `numpy` by randomly shuffling the cups many times and calculating the probability of the participant correctly identifying all cups by chance.
Compare your result with the original 8-cup experiment.  

In your notebook, explain your simulation process clearly, report and interpret the estimated probability, and discuss whether, based on this probability, you would consider extending or relaxing the p-value threshold compared to the original design.  

### Problem 2: Normal Distribution ###

Generate 100,000 samples of size 10 from the standard normal distribution.
For each sample, compute the standard deviation with `ddof=1` (sample SD) and with `ddof=0` (population SD).
Plot histograms of both sets of values on the same axes with transparency.
Describe the differences you see.
Explain how you expect these differences to change if the sample size is increased.

### Problem 3: t-Tests ###

A type II error occurs when a test fails to reject the null hypothesis even though it is false.
For each mean difference $d = 0, 0.1, 0.2, \dots, 1.0$, repeat the following simulation 1,000 times:

1. Draw two samples of size 100, one from the standard normal distribution and one from the normal distribution with mean $d$ and standard deviation 1.
2. Run an independent samples t-test on the two samples, rejecting the null hypothesis if the p-value is less than 0.05.
3. Record the proportion of times the null hypothesis is not rejected.

Plot this proportion against $d$, and explain how the type II error rate changes as the difference in means increases.

### Problem 4: ANOVA ###

Generate three independent samples, each of size 30, from normal distributions with means 0, 0.5, and 1, each with standard deviation 1.

1. Perform a one-way ANOVA to test whether all three means are equal.
2. Perform three independent two-sample t-tests: samples 1 vs 2, 1 vs 3, and 2 vs 3.
3. Compare the conclusions.

Write a short note on why ANOVA is preferred over running several t-tests.

## Getting Started ##

You can run the Jupyter notebook either locally on your machine or directly in the cloud using [GitHub Codespaces](https://github.com/features/codespaces).

### Option 1: Running Locally ###

#### Prerequisites ####

- [Anaconda](https://www.anaconda.com/products/distribution) (recommended) or Python installed on your machine.
- [Visual Studio Code](https://code.visualstudio.com/) with the Jupyter extension.

#### Steps ####

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/fdennehy/applied-statistics
   cd applied-statistics
   ```

2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the Jupyter notebooks:
   - Open the notebooks in VS Code.
   - Select the appropriate Python interpreter to run the notebook.

### Option 2: Running in GitHub Codespaces ###

1. Open the repository on GitHub.
2. Click the Code button and select Codespaces.
3. Create a new Codespace or open an existing one.
4. Once the environment is ready, open the notebooks and start running the cells.

## Reproducibility ##

All results in the notebook can be reproduced by installing the listed dependencies and running the cells from top to bottom.
Random simulations use fixed seeds where appropriate to ensure consistent results.

## Get Help ##

Refer to the inline comments and markdown explanations within the notebook, as well as the official Python and SciPy documentation, for further clarification.

## Contribute ##

Developers are welcome to fork this repo and continue to develop and expand upon it as they wish.

## Acknowledgements ##

Special thanks to my lecturer on the Applied Statistics module, Ian McLoughlin, from whom I acquired the skills necessary to put this project together.

References to relevant statistical literature and official documentation (e.g. NumPy, SciPy, and classical statistical experiments) are included in the relevant sections of the notebook and discussed in context.

[ChatGPT](chatgpt.com) was used as a virtual reviewer to assist with refining the structure, clarity, and presentation of this repository and notebook.
All statistical analysis, implementation, and interpretation remain my own. Prompts are included where applicable in the notebook.

For this README, this [prompt](https://chatgpt.com/share/694735d0-e404-8006-af07-d98244b077ad) was used to generate suggested improvements, the majority of which have been included.

## End ##