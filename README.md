# financial_planner

This is a python-jupyter notebook integrated development environment(IDE) based Financial Planning tool to evaluate financial health. The notebook works as per the standard phases of finacial analysis by extracting Portfolio data from online data sources([Alternative.me API](https://alternative.me/crypto/api/), [Alpaca API](https://alpaca.markets/docs/api-references/)) using Application Programing Interface(API) from the source provider, preparation of datasets by cleaning the data and finally analyzing the data through quantitative analysis and visualizations. The analysis provides details for the member portfolio of a credit union with respect to their cryptocurrency, stocks and bonds portfolio, a financial planner for emergencies to determine if they have enough reserves for an emergency fund based on their monthly income, and a financial planner for retirement to determine the desired retirment portfolio with stocks and bonds. 


---


## Technologies

This project leverages python 3.7 with the following packages:

* [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/#) - Is a browser-based interface to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner.

---

## Installation Guide

You will need Python version 3.7 or above and gitbash/terminal on your computer, along with other supporting packages as mentioned below. 

Please follow instructions from the below link to install python 3.7 or above on your computer

[To install Python, follow instructions from this link](https://www.python.org/downloads/)

[To install Git Bash, follow instructions from this link](https://github.com/git-guides/install-git)

To access the Jupiter notebook, first install the following dependencies.

 [Anaconda](https://docs.anaconda.com/anaconda/install/)

```python
# install conda dev environment and activate it
  conda update conda
  conda create -n dev python=3.7 anaconda
  conda activate dev
#  install Jupyter Lab
   pip install jupyterlab
# To start Jupyter lab (this will enable you to see hidden files such as .env, remember to check 'Show Hidden Files' in the View menu in case that is not  enabled)
  jupyter lab --ContentsManager.allow_hidden=True
   
```


---


## Usage

To use the Jupyter Notebook, clone the repository and once you run the above commands, open 'risk_return_analysis.ipynb'

```git
git clone https://github.com/sidbetatester/financial_planner.git
#This will download all the required files except .env file which you need to create by yourself to access the API through the jupyter notebook.
```

Upon launching the the notebook, you will notice an interface similar to the one below, click  on the 'financial_planning_tools.ipynb' file and you will have the complete analysis. 
![financial_planner](Images/Jupyter_Screenshot.jpg)

Note:
* You can shut down the notebook from the File menu when you are done using the report.

* Generate your API KEY and your SECRET KEY after registering on the [Alpaca site](https://alpaca.markets/), you will not require any paid services to access the data for this Application, so ensure you are not providing any payment information.  

* Create an environment file (.env) in the financial_planner folder, you may create a text file and rename it to .env. 
    * Include variables for ALPACA_API_KEY and ALPACA_SECRET_KEY in this file for accessing the Alpaca API as shown below
    * ALPACA_API_KEY=Your_API_Key_here
    * ALPACA_SECRET_KEY=Your_Secret_Key_here
---


## Contributors

Siddharth Venkumahanti
[linkedin](https://www.linkedin.com/in/siddharthvenkumahanti/)


---


## License

### MIT License

Copyright (c) [2022] [Siddharth Venkumahanti]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

![MIT License](Images/MIT_License.png)



