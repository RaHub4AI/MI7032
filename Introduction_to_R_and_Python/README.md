# <img width="4831" height="1350" alt="BANNER" src="https://github.com/user-attachments/assets/58f4cd8b-ea72-47c8-92ca-6304c3d325ca" />
### R or Python?

If you want opinions, the internet is full of blog posts, videos, and forum threads debating which language to use for data science: `R` or `Python` (a few curated links: [What others think: Python or R?](#what-others-think-python-or-r))
Additionally, this document covers some background, key facts, and the main strengths and trade-offs for both.

However, in this course, you’re free to use either **`R`** or **`Python`**. 
Both are powerful and widely used for environmental data analysis, modeling, and visualization.
Before you decide (and yes, you can use both), we’ll spend the first two days covering the ABCs of each language so you can test-drive them and see which feels right.

And if you care about my opinion: an **exceptional environmental data scientist** benefits from knowing **both**.
If you have the time, I fully support learning both. 
You’ll see plenty of shared concepts, and once the programming fundamentals click, switching between them isn’t that hard. 
At a minimum, aim to **learn the one most common in your subfield**. You’ll get a feel for that during your thesis project and courses by watching what researchers actually use.


---
## Origins & History

### R: built for statisticians
- Developed in the **early 1990s** by [**Ross Ihaka**](https://en.wikipedia.org/wiki/Ross_Ihaka) and [**Robert Gentleman**](https://en.wikipedia.org/wiki/Robert_Gentleman_(statistician)) at the University of Auckland.
- Inspired by **S**, the statistical language created at Bell Labs in the 1970s.
- Designed first for **academic statisticians**; today it’s a go-to tool across many scientific disciplines.

**Foundational papers**

📄 [**Ihaka & Gentleman**: *R: A Language for Data Analysis and Graphics*](https://www.stat.auckland.ac.nz/~ihaka/downloads/R-paper.pdf)

📄 [**Ross Ihaka**: *R: Past and Future History*](https://www.stat.auckland.ac.nz/~ihaka/downloads/Interface98.pdf)

---

### Python: general-purpose language
- Started by [**Guido van Rossum**](https://en.wikipedia.org/wiki/Guido_van_Rossum) (webpage: https://gvanrossum.github.io/) in **1989** (famously as a holiday project).
- Named after *Monty Python’s Flying Circus*, not the snake.
- Began as a **general-purpose** language focused on readability; later exploded in web, AI/ML, and data science thanks to its rich ecosystem (NumPy, pandas, SciPy, scikit-learn, PyTorch, etc.).
- Today, Python **consistently ranks at or near the top** of programming-language popularity indices.

**Further reading**

📄 Python history overview: https://www.python.org/doc/essays/

---

## 🔍 Feature Comparison

| Feature/Domain         | Python 🐍                         | R 🧮                               |
|------------------------|----------------------------------|------------------------------------|
| Data analysis          | ✅ Yes (`pandas`, `numpy`)        | ✅ Yes (built-in, `dplyr`, `tidyverse`) |
| Visualization          | Strong (`matplotlib`, `seaborn`) | Very strong (`ggplot2`, `plotly`) |
| Statistics             | Decent (`scipy`, `statsmodels`)  | Excellent (core strength)         |
| Machine learning       | Industry standard (`scikit-learn`, `TensorFlow`) | Growing support (`caret`, `mlr3`) |
| Reproducible reports   | Jupyter, Sphinx, nbconvert        | RMarkdown, Quarto                 |
| Dashboards             | Streamlit, Dash                  | Shiny                             |
| Programming power      | Full general-purpose language     | Specialized for data/statistics   |
| IDEs                   | VS Code, PyCharm, Jupyter         | RStudio, Jupyter                  |

---

## 🧑‍🔬 Who Uses Them?

### **Python**:
- Used by: Google, NASA, Spotify, Meta, Netflix, CERN
- Typical domains: Remote sensing, AI, automation, climate models, web apps
- Many open-source environmental science packages (e.g., xarray, rasterio)

### **R**:
- Used by: WHO, UN, OECD, EPA, many universities and journals
- Dominant in: Ecology, biostatistics, social sciences, public health
- Well-established workflows in academia and regulatory reporting

---

## 🎉 Fun & Interesting Facts

| Fun Fact                       | R                                         | Python                                     |
|--------------------------------|-------------------------------------------|--------------------------------------------|
| Name origin                    | First names of creators (Ross & Robert)   | Monty Python comedy troupe                 |
| Native IDE                     | RStudio                                   | None – many options (VS Code, Jupyter)     |
| First-class DataFrame support  | Yes, native                               | Yes, via `pandas`                          |
| Language style                 | Functional + vectorized                   | Object-oriented + flexible scripting       |
| Package installation           | `install.packages()`                      | `pip`, `conda`                             |
| Community focus                | Academia, statistics                      | Industry, software, ML                     |

---

## 🌍 Popularity & Ecosystem

- **Python**:
  - #1 language globally in 2024 (TIOBE, Stack Overflow)
  - Over **10 million** users worldwide
  - 350,000+ packages on [PyPI](https://pypi.org)

- **R**:
  - Top 2 in data science/statistics
  - Over **2.5 million** users (mainly in science and gov)
  - 19,000+ packages on [CRAN](https://cran.r-project.org/web/packages/)

---

## 📚 Recommendations for This Course

Choose **R** if:
- You come from a statistics, ecology, or social science background
- You prefer built-in stats models and beautiful visualizations
- You like the idea of Shiny apps or academic publishing

Choose **Python** if:
- You want a language that works across domains (web, automation, ML)
- You’re interested in programming beyond data analysis
- You want to dive into AI, APIs, and earth observation data tools

---
## What others think: Python or R?

**Videos**

<img alt="YT" src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/YouTube_full-color_icon_%282017%29.svg/2560px-YouTube_full-color_icon_%282017%29.svg.png" width="15" /> [**RichardOnData**: *R or Python: Which Should You Learn in 2024?*](https://www.youtube.com/watch?v=AexVDfAueGQ)

<img alt="YT" src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/YouTube_full-color_icon_%282017%29.svg/2560px-YouTube_full-color_icon_%282017%29.svg.png" width="15" /> [**R Programming 101**: *R vs Python*](https://www.youtube.com/watch?v=rMT8NaDcIq0)


**Articles & blog posts**

<img alt="GG" src="https://media.geeksforgeeks.org/gfg-gg-logo.svg" width="15" /> [*R vs Python*](https://www.geeksforgeeks.org/python/r-vs-python/)

<img alt="Medium" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSnyyHXgvbYgVysw0TVvhoi3Zn4cbfYzrXYSHvK8u7aGfPqnlzgW6OXXQX-Dyclke9DVi4&usqp=CAU" width="15" /> [**Kenny William**: *R vs Python: Let’s Settle This with Data!*](https://medium.com/@k3nnywilliam/r-vs-python-lets-settle-this-with-data-837ad273747f)

<img alt="Dataquest" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTmTm75k-qho345hw1Ccc_0FgCl7pxT6FoK6w&s" width="15" /> [**Vik Paruchuri**: *R vs Python for Data Analysis — An Objective Comparison*](https://www.dataquest.io/blog/python-vs-r/)







## 📎 References

- [R Project History](https://www.r-project.org/about.html)
- [Python History](https://www.python.org/doc/essays/blurb/)
- [Stack Overflow Developer Survey 2024](https://insights.stackoverflow.com/survey)
- [TIOBE Index](https://www.tiobe.com/tiobe-index/)
- [CRAN Package Index](https://cran.r-project.org/web/packages/)
- [PyPI Stats](https://pypi.org)

---

> 🧑‍🏫 *In this course, we use Jupyter Notebooks as a shared platform. You can work with either language — we will guide you through setting up both!*


# 🛠️ Setting Up Your Tools: IDEs, Environments, and Notebooks

Once you've chosen between **R** and **Python**, it's time to set up your development tools. This guide will walk you through:

- What is an IDE?
- What is an environment and why it matters
- What is a kernel?
- How to set up Anaconda environments
- How to use Jupyter Notebooks (with both R and Python)
- Using Google Colab (for those who don’t want to install anything)

---

## 💻 What Is an IDE?

**IDE** stands for **Integrated Development Environment**. It’s a software application that makes coding easier by combining:

- A code editor
- A debugger
- A terminal or console
- File management tools
- Package management (in some cases)

### Common IDEs:
| Language | IDE | Link |
|---------|-----|------|
| Python | [Visual Studio Code](https://code.visualstudio.com/), [PyCharm](https://www.jetbrains.com/pycharm/) | Fast, extensible, modern |
| R | [RStudio](https://posit.co/download/rstudio-desktop/) | Tailored for R scripting, modeling, and reporting |
| Both | [JupyterLab](https://jupyter.org/), [Rodeo](https://rodeo.yhat.com/) | Notebook-based environments |

---

## 🧪 What Is an Environment?

An **environment** is a self-contained workspace with:

- A specific version of a programming language
- A set of libraries or packages
- Its own interpreter or kernel

### Why use environments?
- Prevents **version conflicts** between projects
- Keeps your machine organized
- Essential for reproducibility and collaboration

We recommend using **[Anaconda](https://www.anaconda.com/)** to manage environments for this course.

---

## ⚙️ Creating Environments with Anaconda

### 🔹 For Python:

```bash
conda create -n dataenv_python python=3.11
conda activate dataenv_python
conda install jupyter pandas matplotlib seaborn scikit-learn
```

### 🔹 For R:

```bash
conda create -n dataenv_r r-essentials r-base
conda activate dataenv_r
conda install -c r r-irkernel
```

**Tip:** Use the Anaconda Navigator UI if you’re not comfortable with the command line.

---

## 🧠 What Is a Kernel?

A **kernel** is the computational engine behind a notebook or IDE. It interprets your code, runs it, and returns results.

- In **Jupyter**, the kernel is language-specific (R or Python)
- You can switch kernels using the toolbar in Jupyter or JupyterLab

---

## 📃 What Are Notebooks?

**Notebooks** are interactive documents where you can write code, view output, and add text or math explanations.

| Tool | Notebook Format | Language |
|------|------------------|----------|
| Jupyter Notebook | `.ipynb` | Python, R, Julia, etc. |
| R Markdown | `.Rmd` | R |

> 📌 In this course, **Jupyter Notebooks** will be the standard for both R and Python. You’re free to convert `.ipynb` notebooks to `.Rmd` if needed.

---

## 🧪 How to Launch Jupyter Notebook

### 1. Activate your environment:

```bash
conda activate dataenv_python   # or dataenv_r
```

### 2. Launch Jupyter:

```bash
jupyter notebook
```

### 3. Create a new notebook:
- Select your preferred kernel from the dropdown (Python 3 or R)

---

## 🌐 Google Colab – The No-Install Option

**Google Colab** is a cloud-hosted Jupyter Notebook platform. It requires no setup, just a Google account.

### ✅ Pros:
- No installation
- GPU/TPU support
- Easy to share

### ❌ Cons:
- Internet required
- Not ideal for R (requires workaround)
- Files are temporary unless saved to Drive

### 🔹 Getting Started:

1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Choose “New Notebook”
3. To enable R, go to `Runtime > Change Runtime Type > R`

> 📍 You may need to install R packages manually each time, since Colab resets your environment on restart.

