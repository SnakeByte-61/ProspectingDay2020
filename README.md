# Demand-forecasting-sagemaker

Welcome to the AWS hands-on demand forecasting workshop!


With Cyber Monday well underway, we will be using this session to take a step back and assess how companies can access utilization and inventory cost.

In this workshop, we will be forecasting customer demand for food at a restaurant. The workflow today incorporates SageMaker's bulit-in **DeepAR algorithm.** This method has been used in applications ranging from financial data analysis to estimating future AWS spot pricing.

To run this algorithm and explore how timeseries forecasting can help your team, we will be using SageMaker and S3. We will explore and learn how SageMaker helps accelerate the process of training your model and creating inference endpoints.

## [Sagemaker Setup](sagemaker-setup/README.md)

Before you start playing with the system, you have to login into your AWS account and setup a SageMaker Notebook Instance.

## [DeepAR Lab](DeepAR-demo/DeepAR_Lab.ipynb)
The DeepAR forecasting algorithm is a supervised learning method that has been iterated upon by way of a number of applications within Amazon. This method is based on modern deep learning techniques and has been shown to improve forcast accuracy over traditional techniques such as as Autoregressive Integrated Moving Average (ARIMA) and Exponential Smoothing (ES). Moreover, DeepAR requires little to no hyperparameter tuning on a wide variety of datasets and performs well in building representations even on a few hundred traing examples. For more background, it is worthing looking into both the DeepAR [paper](https://arxiv.org/abs/1704.04110) & the launch [blog post.](https://aws.amazon.com/blogs/machine-learning/now-available-in-amazon-sagemaker-deepar-algorithm-for-more-accurate-time-series-forecasting) 

In our demo, the data moves from May 2013 to December 2016 and contains 4 offerings that the restaurant sells. The restaurant has 25 branches all over the country and the training set contains information around the sales of each item sold during the above mentioned period.

As part of this workshop we will work to help the owner of the restaurant forecast expected sales for events following December 2016.

[This](DeepAR-demo/DeepAR_Lab.ipynb) Notebook will take us through the following steps:
* Data preprocessing.
* Uploading data to S3.
* Visualization for observing seasonality.
* AutoRegression.
* Model building.
* HTTP inference endpoint creation.

## [Clean Up](cleanup.md)

Don't forget to clean up your resources at the end of the session. We will walk through this step to ensure it is done in a thorough fashion.
