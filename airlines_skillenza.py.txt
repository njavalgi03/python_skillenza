import pandas as pd
records=pd.read_csv('airlines.csv')  #Reads The CSV file
air_uniq=(record['Airport.Name'].value_counts()) #Lists the unique values
air_uniq.to_json() #Output 1
print((record['Airport.Name'].value_counts()).idxmax(axis='columns')) #Output 2
print((record['Airport.Name'].value_counts()).idxmin(axis=0)) #Output 3

