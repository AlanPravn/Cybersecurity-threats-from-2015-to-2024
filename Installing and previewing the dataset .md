!pip install pandas
!pip install numpy
!pip install matplotlib
!pip install seaborn

# Import libraries for data analysis and visualization
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Importing dataset from google drive
from google.colab import drive
drive.mount('/content/drive')

def load_data(file_path):
  file_path = '/content/drive/My Drive/Cyber security dataset GBP.xlsx'
  df = pd.read_csv(file_path)
  return df

  # Preview the dataset

def load_data(file_path):
  df = pd.read_excel(file_path)
  return df

file_path = '/content/drive/My Drive/Cyber security dataset GBP.xlsx'
df = load_data(file_path)

print("Data Preview:")
print(df.head())

# Displaying descriptive statistics of the DataFrame
print("\nData Description:")
print(df.describe())
