# Titanic Dataset Analysis

This project analyzes the famous Titanic dataset to uncover trends and patterns using data visualization and pandas data manipulation. The analysis covers various aspects of the passengers, including their demographics, class distribution, and survival status.
Requirements

The following Python libraries are required to run the analysis:

    pandas
    numpy
    matplotlib
    seaborn

You can install the required libraries using pip:

bash

pip install pandas numpy matplotlib seaborn

Dataset

The dataset used in this project is the Titanic dataset, typically found in the file train.csv. This dataset contains the following features:

    PassengerId: Unique ID of each passenger
    Survived: Survival status (0 = No, 1 = Yes)
    Pclass: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
    Name: Name of the passenger
    Sex: Gender of the passenger
    Age: Age of the passenger
    SibSp: Number of siblings/spouses aboard
    Parch: Number of parents/children aboard
    Ticket: Ticket number
    Fare: Passenger fare
    Cabin: Cabin number
    Embarked: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

Analysis Overview

The analysis is divided into several steps, exploring the dataset and visualizing various patterns:

    Initial Data Exploration:
        The dataset is loaded and briefly examined using titanic_df.info() and titanic_df.head() to check the structure and content of the data.

    Visualizations Using Seaborn:
        Gender Distribution: Count of male and female passengers.
        Gender and Class Distribution: Count of male and female passengers by class.
        Class Distribution by Gender: Count of passengers in each class grouped by gender.

    Custom Features:
        A new column Person is created to categorize passengers as male, female, or child (if under 16).
        Visualizations are generated to show the distribution of these categories across different classes.

    Age Analysis:
        The distribution of passengers’ ages is visualized using histograms and kernel density plots.
        The average age of passengers is calculated.

    Family Status:
        A new column Alone is created to distinguish passengers traveling alone or with family. A passenger is considered alone if they have no siblings/spouses or parents/children aboard.

    Cabin Analysis:
        The Cabin column is analyzed to explore the different decks where passengers were located. Deck names are extracted, and counts are visualized.

    Port of Embarkation:
        The distribution of passengers based on their port of embarkation is visualized, grouped by class.

    Survival Analysis:
        A new column Survivor is created to map the Survived column into a more human-readable format (yes or no).
        Count plots are generated to show survival rates based on various factors like traveling status (alone or with family) and class.

How to Run the Code

    Clone this repository or download the files.
    Ensure that the train.csv file is in the same directory as the script.
    Install the required libraries using pip (see the Requirements section).
    Run the script in a Jupyter notebook or any Python environment.

The script will generate a series of visualizations and insights about the Titanic passengers.
Output Examples

Here are some of the visualizations you can expect to generate:

    Count of passengers by gender and class.
    Age distribution of passengers.
    Survival rates based on various criteria.

Notes

    This analysis uses the Seaborn library for visualizations. Warnings related to layout changes may appear, but they don't affect the correctness of the code.
    Some columns contain missing values, such as Age and Cabin. Handling these missing values may be explored in future versions of the analysis.
