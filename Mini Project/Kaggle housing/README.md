# Kaggle_housing

### XGBoost 사용
~~~python
xgboost = xgb.XGBRegressor(max_depth=9, n_estimators=2000, learning_rate=0.01, booster='dart', subsample=0.8, colsample_bytree=0.6, random_state=random_state)
~~~
----
**score**
- 104244.58567
