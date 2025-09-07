# Demo: Working Locally with Python and/or R

> This demo is for students who prefer to work with their own local installations of `Python` and/or `R` instead of Colab.  

---

## Python Users

We recommend three ways to set up Python locally:  

#### 1. Full Anaconda (can take up to ~3 GB)  
- Install [Anaconda](https://www.anaconda.com/download).  
- **Jupyter Notebook is included**.  
- Comes with most of the necessary packages and a GUI for managing environments.  
- Easiest option, but large in size.  

#### 2. Mini-version of Anaconda (takes less space)  
- Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html).  
- Only installs **Python and Conda** (no unnecessary space taken).  
- You will need to install Jupyter yourself:  
  ```bash
  conda install jupyter
  ```  
  or:  
  ```bash
  pip install notebook
  ```  
- Saves space, but requires more manual installation later.  

#### 3. No Anaconda, relying on the system Python  
- Install Python directly from [python.org](https://www.python.org/downloads/).  
- Install Jupyter Notebook separately:  
  ```bash
  pip install notebook
  ```
After installing Jupyter Notebook, you can simply run Jupyter Notebook from the command line or Anaconda prompt:
 ```bash
  jupyter notebook
  ```

---

## R Users

*Typically, R users:*  
- *Download **R** from [CRAN](https://cran.r-project.org/).*  
- *Use [**RStudio**](https://rstudio-education.github.io/hopr/starting.html) as their main IDE.*  
- *Work with [**RMarkdown**](https://rmarkdown.rstudio.com/) documents instead of Jupyter Notebooks.*  

In this course, however, we are using **Jupyter notebooks** (to ensure that all students have the same environment via Colab).  

> Therefore, if you want to run R **locally**, the recommended approach is to install [Anaconda](https://www.anaconda.com/download) (just like Python users).  

Benefits of using Anaconda for R in this course:  
- Comes with **Jupyter Notebook** pre-installed.  
- Supports both **Python and R** in the same environment.  
- Ensures your local setup mirrors the course notebooks exactly.  
- Simplifies package management and environment maintenance, just like for Python users.  

This way, whether you are working with Python or R, your workflow remains consistent, and you can follow the course materials seamlessly.  

---

## Creating Environments
Environments (like conda environments or virtualenvs) are isolated spaces where you can install packages and libraries without affecting other projects or the system Python/R installation.

Key reasons to use environments:
- Avoid conflicts: Different projects often require different package versions. Environments prevent one project’s dependencies from breaking another.
- Reproducibility: An environment lets you recreate the same setup on another computer or at a later time. This is crucial for research, collaboration, and professional work.
- Course-specific isolation: During this course, we use specific versions of Python, R, and various packages. Using a dedicated environment ensures your exercises and homework run exactly as intended.
- Best practice in professional workflows: In industry and academia, maintaining separate environments for each project is the standard. It makes software maintenance, debugging, and collaboration much easier.
- Easy cleanup and updates: When a project ends or requires upgrading packages, you can safely delete or rebuild the environment without breaking anything else on your system.

> Bottom line: Using environments is not just a course requirement, it’s how data scientists and developers manage dependencies and maintain reproducible workflows in real life.

#### Quick Guide

| Step | Python | R |
| --- | --- | --- |
| Create a new environment | `conda create -n EDS_py python=3.13` | `conda create -n EDS_R r-base r-essentials` |
| Activate the environment | `conda activate EDS_py` | `conda activate EDS_R` |
| Install packages | `conda install jupyter numpy pandas matplotlib seaborn` | `conda install r-tidymodels` |
| Start Jupyter Notebook | `jupyter notebook` | `jupyter notebook` |
| Deactivate/close environment | `conda deactivate` | `conda deactivate` |


Here is the full documentation on how to manage `conda` environments: https://docs.conda.io/projects/conda/en/4.6.0/user-guide/tasks/manage-environments.html


