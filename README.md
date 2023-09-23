# Phonepe-Pulse-Data-Visualization
Phonepe Pulse Data Visualization and Exploration: A User-Friendly Tool Using Streamlit and Plotly

Introduction
PhonePe Pulse Data Visualization and Exploration is a user-friendly tool built with Streamlit and Plotly that allows users to explore and visualize data related to PhonePe Pulse.

What is PhonePe Pulse?
PhonePe Pulse showcases over 2000+ Crore transactions by consumers on an interactive map of India. With over 45% market share, PhonePe's data is representative of the country's digital payment habits. The insights on the website and in the report have been drawn from two key sources: the entirety of PhonePe's transaction data combined with merchant and customer interviews. The report is available as a free download on the PhonePe Pulse website and GitHub.

Libraries/Modules
This project relies on several libraries and modules:

Plotly: Used for plotting and visualizing data.
Pandas: Utilized to create a DataFrame with scraped data.
mysql.connector: Employed for storing and retrieving data from a MySQL database.
Streamlit: Utilized to create a graphical user interface (GUI).
json: Used for loading JSON files.
git.repo.base: Necessary for cloning the GitHub repository.

Workflow
Step 1: Importing the Libraries
Start by importing the required libraries. Ensure you have them installed using the following command:

import pandas as pd
import mysql.connector as sql
import streamlit as st
import plotly.express as px
import os
import json
from streamlit_option_menu import option_menu
from PIL import Image
from git.repo.base import Repo

Step 2: Data Extraction
Clone the GitHub repository containing PhonePe Pulse data to fetch the required data. Use the following code to clone the repository:

repo_url = 'https://github.com/phonepe/pulse.git'
git.Repo.clone_from(repo_url, clone_dir)

Step 3: Data Transformation
Convert the JSON files obtained from the GitHub repository into a readable and understandable DataFrame format. Use the following code to iterate through the files and create the DataFrame:

Step 4: Database Insertion
To insert the DataFrame into a MySQL database, create a new database and tables using the mysql.connector library. Establish a connection to the database and insert the transformed data using SQL commands. Here's how to do it:

Step 5: Dashboard Creation
To create an interactive and visually appealing dashboard, use Plotly libraries to plot charts and maps. Streamlit can be used to create a user-friendly interface with dropdown options for users to select different data to display.

Step 6: Data Retrieval
If necessary, use the mysql.connector library to connect to the MySQL database and retrieve data into a Pandas DataFrame.

Feel free to adapt these steps and code snippets to your specific project requirements.





















