# Predicting Student Performance in High School Math 
This project uses machine learning regression and classification algorithms to predict the final math scores of students from two Portuguese schools, based on various demographic and social factors.  Using multiple linear regression and decision tree classification, the identification of important features, results of linearity testing, and model accuracy in predicting on new data is developed and displayed.  

The results of this project can be found at the end of the `Grudinschi Predicting Student Performance.ipynb` program.

### Installation

This project requires **Python** and the following Python libraries installed:


- [Pandas](http://pandas.pydata.org/)
- [NumPy](http://www.numpy.org/)
- [seaborn](https://seaborn.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [SciPy](https://scipy.org/)
- [math](https://docs.python.org/3/library/math.html)
- [xgboost](https://pypi.org/project/xgboost/)
- [statsmodels](https://pypi.org/project/statsmodels/)
- [itertools](https://docs.python.org/3/library/itertools.html)

You will also need to have software installed to run and execute a Python program. 

You may run the code on [Jupyter Notebook](http://jupyter.org/install.html), [Google Colab](https://www.freecodecamp.org/news/google-colaboratory-python-code-in-your-google-drive/#:~:text=To%20run%20the%20code%20in,having%20to%20install%20them%20first.), [Pycharm](https://www.jetbrains.com/help/pycharm/installation-guide.html), ect.

### Code

The code is provided in the `Grudinschi Predicting Student Performance.ipynb` notebook file.  You will also need to use the `student-mat.csv` data file.


### Run:

Download `Grudinschi Predicting Student Performance.ipynb` notebook and `student-mat.csv` data file.  Use your preferred software to upload the two files and execute the Python program.  Ensure the two files are stored in the same folder and follow the same path.

### Data:
Source: https://archive.ics.uci.edu/ml/datasets/student+performance

The Data Dictionary is summarized below.

**Features:**

- `school` - student's school (binary: 'GP' - Gabriel Pereira or 'MS' - Mousinho da Silveira)
- `sex` - student's sex (binary: 'F' - female or 'M' - male)
- `age` - student's age (numeric: from 15 to 22)
- `address` - student's home address type (binary: 'U' - urban or 'R' - rural)
- `famsize` - family size (binary: 'LE3' - less or equal to 3 or 'GT3' - greater than 3)
- `Pstatus` - parent's cohabitation status (binary: 'T' - living together or 'A' - apart)
- `Medu` - mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2 – 5th to 9th grade, 3 – secondary education or 4 – higher education)
- `Fedu` - father's education (numeric: 0 - none, 1 - primary education (4th grade), 2 – 5th to 9th grade, 3 – secondary education or 4 – higher education)
- `Mjob` - mother's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
- `Fjob` - father's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
- `reason` - reason to choose this school (nominal: close to 'home', school 'reputation', 'course' preference or 'other')
- `guardian` - student's guardian (nominal: 'mother', 'father' or 'other')
- `traveltime` - home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour)
- `studytime` - weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours)
- `failures` - number of past class failures (numeric: n if 1<=n<3, else 4)
- `schoolsup` - extra educational support (binary: yes or no)
- `famsup` - family educational support (binary: yes or no)
- `paid` - extra paid classes within the course subject (Math) (binary: yes or no)
- `activities` - extra-curricular activities (binary: yes or no)
- `nursery` - attended nursery school (binary: yes or no)
- `higher` - wants to take higher education (binary: yes or no)
- `internet` - internet access at home (binary: yes or no)
- `romantic` - with a romantic relationship (binary: yes or no)
- `famrel` - quality of family relationships (numeric: from 1 - very bad to 5 - excellent)
- `freetime` - free time after school (numeric: from 1 - very low to 5 - very high)
- `goout` - going out with friends (numeric: from 1 - very low to 5 - very high)
- `Dalc` - workday alcohol consumption (numeric: from 1 - very low to 5 - very high)
- `Walc` - weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)
- `health` - current health status (numeric: from 1 - very bad to 5 - very good)
- `absences` - number of school absences (numeric: from 0 to 93)
 
**The following attributes are grades for the course subject Math:**

- `G1` - first period grade (numeric: from 0 to 20)
- `G2` - second period grade (numeric: from 0 to 20)
- `G3` - final grade (numeric: from 0 to 20)) - Target Variable

**The following variables are created within the program:**

- `Avg_G1&G2` - average first and second period grade (numeric: from 0 to 20)
- `Avg_Alc` - weighted average weekend and workday alcohol consumption (numeric: from 1 - very low to 5 - very high)
- `Avg_Par_Edu` - average mother and father education (numeric: 0 - none, 1 - primary education (4th grade), 2 – 5th to 9th grade, 3 – secondary education or 4 – higher education)
