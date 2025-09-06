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

### <img width="50" alt="r" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/R_logo.svg/2560px-R_logo.svg.png" />: built for statisticians
- Developed in the **early 1990s** by [**Ross Ihaka**](https://en.wikipedia.org/wiki/Ross_Ihaka) and [**Robert Gentleman**](https://en.wikipedia.org/wiki/Robert_Gentleman_(statistician)) at the University of Auckland.
- Inspired by **S**, the statistical language created at Bell Labs in the 1970s.
- Designed first for **academic statisticians**; today it’s a go-to tool across many scientific disciplines.
- 22,676 packages on [CRAN](https://cran.r-project.org/web/packages/)

**Foundational papers**

📄 [**Ihaka & Gentleman**: *R: A Language for Data Analysis and Graphics*](https://www.stat.auckland.ac.nz/~ihaka/downloads/R-paper.pdf)

📄 [**Ross Ihaka**: *R: Past and Future History*](https://www.stat.auckland.ac.nz/~ihaka/downloads/Interface98.pdf)

---

### <img width="50" alt="py" src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/1200px-Python-logo-notext.svg.png" />: general-purpose language
- Started by [**Guido van Rossum**](https://en.wikipedia.org/wiki/Guido_van_Rossum) (webpage: https://gvanrossum.github.io/) in **1989** (famously as a holiday project).
- Named after *Monty Python’s Flying Circus*, not the snake.
- Began as a **general-purpose** language focused on readability; later exploded in web, AI/ML, and data science thanks to its rich ecosystem.
- Today, Python **consistently ranks at or near the top** of programming-language popularity indices (https://www.tiobe.com/tiobe-index/, https://pypl.github.io/PYPL.html, https://survey.stackoverflow.co/2025/technology).
- 665,810 packages on [PyPI](https://pypi.org)

**Further reading**

📄 Python history overview: https://www.python.org/doc/essays/

---
## Feature Comparison

| Aspect | <img width="30" alt="r" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/R_logo.svg/2560px-R_logo.svg.png" /> | <img width="30" alt="py" src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/1200px-Python-logo-notext.svg.png" /> |
|---|---|---|
| **Primary Objective** | Data analysis and statistics | General-purpose language with strong support for data science & ML |
| **Primary Users** | Statisticians, researchers | Programmers, developers, professionals in many fields (including researchers) |
| **Flexibility** | Strong in statistical analysis, data visualization | Highly versatile (ML, AI, apps, web development, data science) |
| **Learning Curve** | Steeper (requires stats knowledge, unique syntax) | Smoother, beginner-friendly, English-like syntax |
| **Integration** | Runs locally, less focus on integration | Strong integration with apps, APIs, and web development |
| **Task Efficiency** | Excels in statistical reporting and visualization | Faster for large-scale ML, big data, and algorithm deployment |
| **Database Handling** | Handles large datasets, good with statistical data | Handles large datasets with superior database integration tools |
| **IDE** | `RStudio` | `Jupyter Notebook`, `Spyder`, `IPython`, `VS Code` |
| **Key Libraries** | `tidyverse`, `ggplot2`, `caret`, `dplyr`, `readr`, `tidymodels` | `NumPy`, `Pandas`, `SciPy`, `Scikit-Learn`, `TensorFlow`, `PyTorch`, `Seaborn`, `Matplotlib` |
| **Strengths** | Excellent for visualization, deep statistical analysis | Easy to learn, versatile, strong ML & AI (including deeplearning) ecosystem, high speed |
| **Weaknesses** | Slower performance, steep learning curve, fewer integrations | Weaker at graphics |

---

## What others think: Python or R?

**Videos**

<img alt="YT" src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/YouTube_full-color_icon_%282017%29.svg/2560px-YouTube_full-color_icon_%282017%29.svg.png" width="15" /> [**Aaron Oliver**: *R vs Python | Which should you learn in 2025?*](https://www.youtube.com/watch?v=JAEs5IAhAYY&ab_channel=AaronOliver)

<img alt="YT" src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/YouTube_full-color_icon_%282017%29.svg/2560px-YouTube_full-color_icon_%282017%29.svg.png" width="15" /> [**RichardOnData**: *R or Python: Which Should You Learn in 2024?*](https://www.youtube.com/watch?v=AexVDfAueGQ)

<img alt="YT" src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/YouTube_full-color_icon_%282017%29.svg/2560px-YouTube_full-color_icon_%282017%29.svg.png" width="15" /> [**R Programming 101**: *R vs Python*](https://www.youtube.com/watch?v=rMT8NaDcIq0)


**Articles & blog posts**

<img alt="GG" src="https://media.geeksforgeeks.org/gfg-gg-logo.svg" width="15" /> [*R vs Python*](https://www.geeksforgeeks.org/python/r-vs-python/)

<img alt="Medium" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSnyyHXgvbYgVysw0TVvhoi3Zn4cbfYzrXYSHvK8u7aGfPqnlzgW6OXXQX-Dyclke9DVi4&usqp=CAU" width="15" /> [**Kenny William**: *R vs Python: Let’s Settle This with Data!*](https://medium.com/@k3nnywilliam/r-vs-python-lets-settle-this-with-data-837ad273747f)

<img alt="Dataquest" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTmTm75k-qho345hw1Ccc_0FgCl7pxT6FoK6w&s" width="15" /> [**Vik Paruchuri**: *R vs Python for Data Analysis — An Objective Comparison*](https://www.dataquest.io/blog/python-vs-r/)



