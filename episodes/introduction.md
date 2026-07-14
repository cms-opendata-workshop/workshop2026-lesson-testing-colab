---
title: "Introduction"
teaching: 20
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions

- What is Colab?
- Is it the same or different than a Jupyter notebook?
- Can it do more than just python?
- How do I use it to write or execute python code?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Learn how to open a shared Colab notebook, edit it, and save it.
- Learn how to execute python from within Colab.

::::::::::::::::::::::::::::::::::::::::::::::::

## Three things that are easy to confuse

Before we open a single notebook, it helps to untangle three terms that often get used
interchangeably but really mean different things: **Python**, **Jupyter notebooks**, and
**Colab**. In short, Python is a *language*, a Jupyter notebook is a *place to write and
run that language interactively*, and Colab is *a way to use those notebooks in the cloud
without installing anything*. If you keep that hierarchy in mind — language, then notebook,
then cloud host — everything else in this workshop will fit into place.

## Python: the language

[Python](https://www.python.org/) is a **programming language** — the actual instructions
you write to tell a computer what to do. It was created by Guido van Rossum and first
released in 1991, and, contrary to popular belief, it is named after the British comedy
troupe *Monty Python's Flying Circus*, not the snake. Python was designed to be readable
and approachable, which is a big part of why it has become one of the most widely used
languages in science, data analysis, and education. The current version is Python 3.14
(released in late 2025), and you can read more about its history and design on the
[official Python website](https://www.python.org/) and its
[Wikipedia entry](https://en.wikipedia.org/wiki/Python_(programming_language)).

On its own, Python is just the language. To *use* it, you need some environment that can
read your code and run it — and that is where notebooks come in.

## Jupyter notebooks: the interactive environment

A **Jupyter notebook** is a document that lets you write and run code in small, editable
chunks called *cells*, and it stitches together live code, the output that code produces
(numbers, tables, plots), and formatted explanatory text all in one place. That mix of
"code plus narrative" is what makes notebooks so popular for teaching and for exploratory
science. The notebook file itself has the extension `.ipynb`, and you open and run it
inside an application — either the classic Jupyter Notebook interface or the more modern,
IDE-like [JupyterLab](https://jupyter.org/).

::: callout
IDE stands for Interactive Development Environment, and refers to a program that
enables you to both edit and execute computer code.
:::


Notebooks have a lovely origin story for a physics audience. The project began as
**IPython**, built in 2001 by [Fernando Pérez](https://en.wikipedia.org/wiki/Fernando_P%C3%A9rez_(software_developer))
while he was a particle-physics graduate student looking for a better way to poke at his
simulation data. The browser-based IPython Notebook arrived in 2011, and in 2014 it was
rebranded as part of the broader [Project Jupyter](https://en.wikipedia.org/wiki/Project_Jupyter).
The name "Jupyter" is a nod to three core languages — **Ju**lia, **Py**thon, and **R** — and
an homage to Galileo's own notebooks documenting the moons of Jupiter. That history hints
at an important point: **notebooks are not limited to Python.** Jupyter runs code through
interchangeable *kernels*, so the same notebook interface can execute R, Julia, and dozens
of other languages, as well as ordinary shell commands.

## Colab: Jupyter in the cloud

**Google Colaboratory** — "Colab" for short — is a free, cloud-based service from Google
Research (first released in 2017) that lets you run Jupyter-style notebooks entirely in
your web browser, with **nothing to install**. The notebooks run on Google's computers
rather than yours, save to your [Google Drive](https://drive.google.com/) like any other
Google document, and can be shared and edited collaboratively the way a Google Doc can.
Colab also gives you free (if limited) access to more powerful hardware such as GPUs.
You can explore it at [colab.research.google.com](https://colab.research.google.com/) and
read the details in the [Colab FAQ](https://research.google.com/colaboratory/faq.html).

So, to answer two of our opening questions directly: Colab is **essentially Jupyter hosted
in the cloud**. If you already know Jupyter, you know Colab — a handful of menu items and
keyboard shortcuts differ, but the cell-based, code-plus-text experience is the same. And
because it is built on the same kernel system as Jupyter, it can run more than just Python.
The tidy summary to carry with you: *Python is the language, Jupyter is the notebook
environment that runs it, and Colab is Google's cloud version of that environment.*

## Saving your own copy so your edits stick

There is one habit worth building early. When you open a notebook we have shared with you,
your changes are **not** automatically saved back to a copy you own — and anything you type
can be lost when the session ends. To keep your work, make your own copy in your Google
Drive as soon as you open a shared notebook.

::::::::::::::::::::::::::::::::::::::::: callout

### Save a copy to your Drive first

In the Colab menu, choose **File → Save a copy in Drive**. This creates a personal copy in
your own Google Drive that you can edit freely, and your changes will persist across
sessions. You will need to be signed in to a Google account to do this.

::::::::::::::::::::::::::::::::::::::::::::::::::

## Optional!

### Running the notebooks locally instead

You are not required to stay in the cloud. If you would rather run these notebooks on your
own machine — for offline work, for privacy, or simply to keep them after the workshop —
you can download any Colab notebook and open it in Jupyter locally.

1. In Colab, choose **File → Download → Download .ipynb** to save the notebook file to your
   computer.
2. Install Python together with Jupyter. The simplest route for newcomers is the
   [Anaconda distribution](https://www.anaconda.com/download), which bundles Python,
   JupyterLab, and most of the scientific libraries you'll need. Alternatively, install
   Python and then run `pip install jupyterlab` (see the
   [Jupyter installation guide](https://jupyter.org/install)).
3. Launch JupyterLab and open your downloaded `.ipynb` file.

Keep in mind that a few Colab conveniences do not carry over: mounting Google Drive, the
free GPUs, and Colab's pre-installed packages are cloud features, so when running locally
you may need to install some libraries yourself with `pip` or `conda`.

## What's next

With those distinctions in hand, you're ready for the hands-on part. The shared Colab
notebooks will walk you step by step through opening, editing, and executing cells — so you
can start writing and running Python right away.

:::::::::::::::::::::::::::::::::::::: keypoints

- **Python** is a programming language; a **Jupyter notebook** is an interactive environment that runs code in cells alongside text and output; **Colab** is Google's free, cloud-hosted version of that notebook environment.
- Colab is essentially Jupyter in the cloud — if you know one, you can use the other.
- Notebooks are not Python-only; they can run other languages (and shell commands) through different kernels.
- Opening a shared notebook does not save your edits. Use **File → Save a copy in Drive** to keep a persistent, editable copy.
- You can download any notebook (**File → Download → Download .ipynb**) and run it locally with Jupyter, e.g. via [Anaconda](https://www.anaconda.com/download).

::::::::::::::::::::::::::::::::::::::::::::::::




[r-markdown]: https://rmarkdown.rstudio.com/
