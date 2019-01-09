# SMA-effectiveness-analysis
Basic comparison of the effectiveness of Simple Moving Average (SMA) strategies for Commoodities and Equities markets 

# file_data variable (important note for general usage)
e.g. 

file_data = pd.read_csv(r'C:/Users/Tan Zong Hong/Python_codes/DAO2704 Project/Equity_excel/' + ticker_array[i] + ".csv")

should be replaced with pd.read_csv(r'location_of_Equity.csv_storage' + ticker_array[i] + ".csv")

reasoning:
While attempting to consolidate price data into pandas dataframe, it was found that the consolidation would introduce 
"nan" (not-a-number) into the dataframe due to the difference in time-series. Forward fitting datas would create artifical 
prices and lead to gross over-estimation of the SMA Strategy accuracy.

Since there was no significant time-load difference, the more accurate method was used, manually extracting every Equity csv 
file from 'Equity_csv' file for its calculation.

(note: due to small population size of commodities (31 commodities with sufficient volume), it is viable to do a population census) 

# Full PDF report 
Simple Moving Average analysis (Comparison between Commodity and Equity market)

https://drive.google.com/open?id=12rTuEGf0jhB3LfIcQTp32Be4esSCiDM3 
