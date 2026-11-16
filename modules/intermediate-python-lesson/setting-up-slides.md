---
title: Setting up Environment
type: slides
order: 2
author: Sander van Rijn
description: "Section 1: Setting Up Environment For Collaborative Code Development & Intro to Our Software Project​"
---

<!-- .slide: data-state="title" -->

<style>

/* Blockquote main style */
.blockquote {
    position: relative;
    font-weight: 800;
    padding: 30px 0;
    width: 100%;
    max-width: 500px;
    z-index: 1;
    margin: 80px auto;
    align-self: center;
    border-top: solid 1px;
    border-bottom: solid 1px;
}

/* Blockquote right double quotes */
.blockquote:after {
    position: absolute;
    content: "”";
    font-size: 10rem;
    line-height: 0;
    bottom: -43px;
    right: 30px;
}

/* Blockquote subheader */
.blockquote h4 {
    position: relative;
    font-size: 1.4rem;
    font-weight: normal;
    line-height: 1;
    margin: 0;
    padding-top: 20px;
    z-index: 1;
}

</style>

# Setting Up Environment For Collaborative Code Development & Intro to Our Software Project

===

<!-- .slide: data-state="standard 10" -->

## Introduction

In order to develop (write, run, test, debug, backup) code efficiently, you need to use a number of different tools interchangeably ​

- Introduction to software project and software development tools (refresher)​
  - Command line, IDE, Git + GitHub ​
- Setting up virtual development environment to isolate code (pip, venv)​
- Writing and checking for well-formatted and readable code - PEP8 coding style convention & linting​

===

<!-- .slide: data-state="standard 10" -->

# 1.1 Introduction to our software project

Patient Inflammation Study Project

<img src='./media/image15.png'>

==

<!-- .slide: data-state="standard 10" -->

# Project structure

```
├── data
│   ├── inflammation-01.csv
│   …
│   └── inflammation-12.csv
├── inflammation
│   ├── __init__.py
│   ├── models.py
│   └── views.py
├── inflammation-analysis.py
├── LICENCE.md
├── pyproject.toml
├── README.md
└── tests
    ├── test_models.py
    └── test_patient.py
```

==

<!-- .slide: data-state="standard 10" -->

# Model – View – Controller architecture


- Model (represents the data)
- View (interacts with the user), and
- Controller (handles input and output).

<!-- .element: class="fragment" data-fragment-index="1" -->

Example:
<!-- .element: class="fragment" data-fragment-index="2" -->
- I click on ‘summary of inflammation study results for these 10 patients’ (View)
- Controller accepts this input and asks Model for the appropriate data
- Model retrieves the data and sends it to Controller
- Controller analyses the data and sends it to View
- View presents the results

<!-- .element: class="fragment" data-fragment-index="2" -->

==

<!-- .slide: data-state="standard 10" -->

# Model – View – Controller architecture

- It makes sense to gather functionality that is related to each other in a module and make it clear how modules interact with each other (how they ‘interface’).
- This makes the code more **modular**, and thereby more **reusable, readable, and manageable**. We will get back to this in section 3.


===

<!-- .slide: data-state="standard 10" -->

# Instructions

- Follow instructions for "Downloading Our Software Project" (also carry out the exercise)
- Quickly go over "Our Software Project’s Structure", which we have covered in the presentation.

===

<!-- .slide: data-state="standard 10" -->

# 1.2 Virtual Environments for Software Development


<div style="display: flex; gap: 1em;">
<div style="flex: 2;">
  <img src='./media/image16.png'>
</div>
<div style="flex: 1;">

Is there anyone who already uses virtual environments?

Why is this useful?

</div>
</div>

==

<!-- .slide: data-state="standard 10" -->

# 1.2 Instructions

- Go through introductory sub-sections on virtual environments in Python, especially if not familiar with the topic.
- Follow instructions, which guide you through setup of venv and pip.
- If you consider yourself experienced on the topic, try out uv.

===

<!-- .slide: data-state="standard 10" -->

# 1.3 Integrated Developer Environment

- An Integrated Development Environment (IDE) is a very powerful editor that has a lot of useful extra features. 
- If you do not want to you do not have to leave the environment while programming.
- What do you use? And why?

==

<!-- .slide: data-state="standard 10" -->

# 1.3 Instructions

Pick an IDE:
- PyCharm: Python-oriented, free community edition (free pro versions for educational institutions).
- Visual Studio Code (VS Code): free general-purpose IDE.

Follow instructions to configure the selected IDE. 


<div style="display: flex; gap: 1em;">
<div style="flex: 1;">
  <img src='./media/image17.png'>
</div>
<div style="flex: 1;">
  <img src='./media/image19.png'>
</div>
</div>

===
