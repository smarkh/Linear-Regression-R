# Linear-Regression-R
Linear Regression R


This is the data exploration and data modeling of container unload times.

This uses simple linear regression to predict the amount of time a container will take to be unloaded.

Currently the model predicts well with a MSE of 111, an RMSE of 10.1, a MAE of 8, and an R^2 of .87. 

That being said there are some assumptions that are being violated (independance, and slightly linearity). I am in the process of investigating and improving these.

Model being used: UNLOAD.MINS~CASES*QTY+log(SKUs)+OCEAN.TL+TEAM.SIZE+log(complexity)

Note: Complexity is a score that I created for each container through feature extraction using the cases and QTY numbers. This is where I am assuming the non linearity assumption
  is being violated, but adding it has improved its predictions, so for now I am leaving it in.
