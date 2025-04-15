Note: 2025 edition is at [github.com/mauro3/EGU2025-Julia-intro-and-showcase-for-geoscience](https://github.com/mauro3/EGU2025-Julia-intro-and-showcase-for-geoscience)

# [Introduction to Julia for Geoscience](https://meetingorganizer.copernicus.org/EGU24/session/49443) - EGU 2024

Julia offers a fresh approach to scientific computing, high-performance computing and data crunching. Recently designed from the ground up Julia avoids many of the weak points of older, widely used programming languages in science such as Python, Matlab, and R. Julia is an interactive scripting language, yet it executes with similar speed as C(++) and Fortran. Its qualities make it an appealing tool for the geo-scientist.

Julia has been gaining traction in the geosciences over the last years in applications ranging from high performance simulations, data processing, geostatistics, machine learning, differentiable programming to general modelling. The Julia package ecosystem necessary for geosciences has substantially matured, which makes it readily usable for research.

This course provides a hands-on introduction to get you started with Julia. We aim to give a broad overview of Julia and its ecosystem as well as going through hands-on coding exercises based around concrete earth science applications. In particular you will:
- Learn about the Julia basics and why it is such an interesting language for science
- Learn how to easily and efficiently manipulate data, as well as how to produce beautiful plots
- Learn how to easily solve differential equations, and how to solve inverse optimization problems

Organizers: Mauro Werder, Lazaro Alonso Silva, Jordi Bolibar

## Content

The content is organized into three notebooks:
- Intro to the basics `julia-basics.ipynb`
- Intro to geo-data & computations `geo-ecosystem.ipynb`
- Intro to scientific computing and inversions `diff-eqs.ipynb`

Notebooks are found in the `notebooks/` and `notebooks-solution/`
folder, the latter being with hands-on stuff evaluated.

## Installation

For the short course we will (try to) provide a Jupyter Hub server
with all the packages installed and ready to go.

If you want to run this on your computer, the following steps should
work:

- install Julia (do install 1.10 or later, as quality of life is much
  better that way)
  - we recommend to do this via `juliaup` https://github.com/JuliaLang/juliaup
- clone / download this repository
- launch the Julia REPL in folder of the repository with `julia --project`
- hit `]` to enter package mode and type `instantiate`
  - this will take a long time (10min) to download and install all
    packages (about 300 packages in total as the geo and differential
    equation stacks are extensive; additionally it may pull in a
    JupyterHub install via Conda)
- restart the repl in the folder with `julia --project`
- execute `using IJulia; notebook(dir=".")` which should open a
  browser window with Jupyter running
