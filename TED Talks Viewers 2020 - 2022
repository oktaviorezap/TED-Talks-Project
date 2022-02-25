# TED-Talks-Project

#IMPORT DATA
import pandas as pd
import numpy as np
import openpyxl

ted_talks = pd.read_csv('TED Talks.csv')
ted_talks

#DATA CLEANSING
ted_talks = ted_talks.dropna()
ted_talks.info()
print('\nShape TED Talks Dataset:', ted_talks.shape)

del ted_talks['link']
ted_talks.info()

#TRANSFORMING_DATA
ted_talks['year'] = ted_talks['date'].str.extract(r'(\d+)')
ted_talks['year']

#SAVE THE DATA
ted_talks2022 = ted_talks[(ted_talks['year']=='2022') & (ted_talks['author'])]
ted_talks2022.to_excel(r'C:\Users\Oktavio Reza Putra\OneDrive\Documents\Dataset_TED Talks 2022.xlsx', index = False)

ted_talks2021 = ted_talks[(ted_talks['year']=='2021') & (ted_talks['likes'])]
ted_talks2021.to_excel(r'C:\Users\Oktavio Reza Putra\OneDrive\Documents\Dataset_TED Talks 2021.xlsx', index = False)

ted_talks2020 = ted_talks[(ted_talks['year']=='2020') & (ted_talks['likes'])]
ted_talks2020.to_excel(r'C:\Users\Oktavio Reza Putra\OneDrive\Documents\Dataset_TED Talks 2020.xlsx', index = False)
