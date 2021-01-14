# Sizing of multi-rotor drones

*This set of documents aims to provide an introduction on the use of Python and Jupyter notebooks for the sizing of multi-rotor drones.*

*Written by Marc Budinger (INSA Toulouse) and Scott Delbecq (ISAE-SUPAERO), Toulouse, France.*

### Organization

- 15/01/2021 A.M - Lecture on the **Preliminary design of mechatronic systems** (3 * 1 hour Zoom) by Marc Budinger
- 15/01/2021 P.M - Lab work on the **Preliminary sizing of multirotor drones** (3 * 1 hour Presential)
    * Architecture & sizing scenarios
    * Estimation models
    * Component sizing code (Propeller and motor)
 - 29/01/2021 A.M - Lab work on the **Preliminary sizing of multirotor drones** (4 * 1 hour Presential)   
    * Component sizing code (Battery/ESC and frame)
    * System sizing code and optimization
    
### Evaluation
You will be evaluated on a synthetic presentation (e.g. notebooks or Word or Powerpoint up to you) of your approach (model establishment, sizing code formulation) and analysis you will make (changing the drone architecture, comparing with existing consumer drones...). 
You will also be asked to send your notebooks with the sizing and optimization code working.

The following notebooks have two versions (Student and Teacher). The student versions have missing parts in the code that you will have to re-write.
The sizing and optimization Teacher code is not provided. However, you have a Reference version with a compiled model to compare and verify your results.

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
6. 
    a. [Drone Sizing Code and Optimization - Student Version](06_SystemSizingCodeOptimization-Student.ipynb)
    
    b. [Drone Sizing Code and Optimization - Reference Version](06_SystemSizingCodeOptimization-Reference.ipynb)
##### Appendices  
A1. [Quadrotor description](A1_QuadroDescription.ipynb)

A2. [Sizing scenarios synthesis](A2_Sizing_equations.ipynb)

### Remarks

This document has been written with Jupyter Notebook. The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. 

More informations about Jupyter can be found [here](http://jupyter.org/).

The "live" code is python 3 with numpy, scipy packages. Jupyter and a lot of scientific packages are included in the [Anaconda](https://www.anaconda.com/what-is-anaconda/) python distribution.

Dependencies:
numpy
scipy
cloudpickle
statsmodels
matplotlib
openpyxl
xlrd
pandas
jupyterlab

To install all the dependencies:
*pip install --user -r requirements.txt*

To install a single dependency:
*pip install --user cloudpickle*

*pip install  --proxy=http://proxy.isae.fr:3128 --user cloudpickle* (if connected to ISAE-SUPAERO network)

To run your notebooks from the root:

`jupyter notebook`


The narrative text is formatting with markdown section. Here is a short tutorial about the use of the [markdown](http://www.markdowntutorial.com) standard.  

[RISE](https://github.com/damianavila/RISE) allows you to instantly turn your Jupyter Notebooks into a slideshow.  
[Pandoc](https://pandoc.org/) enables to [convert](https://mrjoe.uk/convert-markdown-to-word-document/) markdown file into word documents:  

*pandoc -o output.docx -f markdown -t docx filename.md*