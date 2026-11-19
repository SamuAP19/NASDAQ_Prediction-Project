# Updates 

 - I'm seperating the data splitting from the data cleaning , i didn't change anything from your code but i just am organising it since "Project_featres is a fucking massive file" 
 - i put it in "Data_splitting"
 - Theres a new notebook for PCA , imma do it since we don't have enough data 
 - PCA is done in 2_pca 
 - i put a number before the notebook to show the order we should eexecute the files 
 - 4 is model training , i used a logistic classification model 


 # Questions ? 

```
 # anti-leakage: no price level of day t in the features
feature_cols = [c for c in data.columns if c not in target_cols]
assert ("Close", "^NDX") not in feature_cols and ("Open", "^NDX") not in feature_cols
assert not data.columns.get_level_values(0).isin(["Open", "Close", "Volume"]).any() 
```

what is anti-leakage ? and what is assert ? doing here ? 

````
data = data.drop(columns=["Open", "Close", "Volume"], level=0)
data = pd.concat([data, stock_ret], axis=1)
``````
i don't get why you drop all the open , close , volume ? 