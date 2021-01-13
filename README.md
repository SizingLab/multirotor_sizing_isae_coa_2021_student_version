# Sizing of multi-rotor drones

*This set of documents aims to provide an introduction on the use of Python and Jupyter notebooks for the sizing of multi-rotor drones.*

*Written by Marc Budinger (INSA Toulouse) and Scott Delbecq (ISAE-SUPAERO), Toulouse, France.*

### Table of contents

##### Architecture & sizing scenarios
1. [Case study and architecture presentation](01_CaseStudy.ipynb)
2. [Sizing scenarios equations](02_SizingScenariosEquations.ipynb) ([Student Version](02_SizingScenariosEquations-Student.ipynb))

##### Estimation models 
3. [Scaling laws of electrical components](03_ScalingLawsElectricalComponents.ipynb) ([Student Version](03_ScalingLawsElectricalComponents-Student.ipynb))
4. [Linear regression of propellers data](04_PropellerLinearRegression.ipynb) ([Student Version](04_PropellerLinearRegression-Student.ipynb))

##### Component sizing code  
5. [Introduction](05_SizingModelsIntroduction.ipynb)  
    a. [Propeller](05a_PropellerSelection-Student.ipynb)
    
    b. [Motor](05b_MotorSelection-Student.ipynb)
    
    c. [Battery and ESC](05c_BatteryESCSelection-Student.ipynb)
    
    d. [Frame](05d_FrameSelection-Student.ipynb)

##### System sizing code and optimization  
6. [Drone Sizing Code and Optimization - Student Version](06_SystemSizingCodeOptimization-Student.ipynb)
##### Appendices  
A1. [Quadrotor description](A1_QuadroDescription.ipynb)

A2. [Sizing scenarios synthesis](A2_Sizing_equations.ipynb)

### Remarks

This document has been written with Jupyter Notebook. The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. 

More informations about Jupyter can be found [here](http://jupyter.org/).

The "live" code is python 3 with numpy, scipy packages. Jupyter and a lot of scientific packages are included in the [Anaconda](https://www.anaconda.com/what-is-anaconda/) python distribution.

Additional package to install:

*pip install --user cloudpickle*

*pip install  --proxy=http://proxy.isae.fr:3128 --user cloudpickle* (if connected to ISAE-SUPAERO network)

The narrative text is formatting with markdown section. Here is a short tutorial about the use of the [markdown](http://www.markdowntutorial.com) standard.  

[RISE](https://github.com/damianavila/RISE) allows you to instantly turn your Jupyter Notebooks into a slideshow.  
[Pandoc](https://pandoc.org/) enables to [convert](https://mrjoe.uk/convert-markdown-to-word-document/) markdown file into word documents:  

*pandoc -o output.docx -f markdown -t docx filename.md*