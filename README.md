# applied-statistics #

**by Finbar Dennehy** 

## Repository Overview ##

This repository primarily contains a Jupyter Notebook `problems.ipynb`, representing my project submission for the 'Applied Statistics' module as part of the HDip in Science in Data Analytics at ATU.

This project applies statistical simulation and inference techniques to classical problems in applied statistics.
The notebook demonstrates the use of Monte Carlo simulation, sampling distributions, hypothesis testing, and analysis of variance (ANOVA), with an emphasis on interpretation and reproducibility rather than purely numerical results.

The work is intended to demonstrate both statistical understanding and reproducible, clean and concise Python code.

## Repository Contents ##

- `.gitignore`: File using the Python, Windows and Mac OS gitignore templates.
- `README.md`: This README file.
- `requirements.txt`: Included in the repository for easy installation, it contains the third-party package dependencies.
- `problems.ipynb`: The notebook is structured with an initial inroduction and import of all required packages, clearly labelled sections for each problem, and a conclusion summary.

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

[ChatGPT](chatgpt.com) was used primarily for assistance genertaing this README and for both the introduction and conclusion sections of the notebook. It was also used as a general debugging tool for Python code cells.
For this README, this [prompt](https://chatgpt.com/share/694735d0-e404-8006-af07-d98244b077ad) was used to generate suggested improvements, the majority of which have been included.

## End ##