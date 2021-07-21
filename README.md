# Fin-Tech_Challenge14_Machine_Learning _Trading_Bot

In this Challenge, you’ll assume the role of a financial advisor at one of the top five financial advisory firms in the world. Your firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, your firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave your firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. You’re thus planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, you’ll enhance the existing trading signals with machine learning algorithms that can adapt to new data.




## Conclusion

#### 1. Establish a Baseline Performance

At the start, actual returns and strategy returns looks well matched; however, strategy returns outperforms the actual one at the end of 2019 and keep its leading position in the following years.

![0_stats](images\0_stats.PNG)

![0_result](images\0_result.png)

#### 2. Tune the Baseline Trading Algorithm

##### 2.1. Tune the training algorithm by adjusting the size of the training dataset.

What impact resulted from increasing or decreasing the training window? 

Based on the best strategy returns with training window size 6 month, either increasing or decreasing the size of the training dataset from 6 month would lower the performance.



![1_stats](images\1_stats.PNG)

![1_result](images\1_result.png)



##### 2.2. Tune the trading algorithm by adjusting the SMA input features.

What impact resulted from increasing or decreasing either or both of the SMA windows? 

Increasing the size of fast SMA window from 4 days to 32 days would lower the trading algorithm's performance.

![2_stats](images\2_stats.PNG)

![2_results](images\2_results.png)



##### 2.3. Choose the set of parameters that best improved the trading algorithm returns.

The trading algorithm's performance is not as good as actual returns until early in 2020; it performs well after that.

![3_stats](images\3_stats.PNG)

![3_results](images\3_results.png)

### 3. Evaluate a New Machine Learning Classifier: `LogisticRegression`

Logistic regression classifier performs slightly better than actual returns in 2016; however, it drops steeply at the end of 2016, and underperforms for a long period. At the start of 2020, it catches up and performs slightly better than the actual returns again.

![alternative_stats](images\alternative_stats.PNG)

![alternative_results](images\alternative_results.png)



## Technologies

This project leverages python 3.7 with the following packages:

  * [Pandas](https://pandas.pydata.org/) - Pandas is a Python library that’s designed specifically for data analysis. It offers a streamlined way of reviewing datasets and includes
    various functions that simplify importing, updating, and analyzing data.

  * [JupyterLab](https://jupyter.org/) - JupyterLab is a web-based user interface that you use to run and review Python-based programs. It easily integrates with the Anaconda
    software package and your Conda development environment.



## Installation Guide

Before running the application first install the following dependencies.

```python
sourse activate 
conda activate dev
conda list pandas
conda list jupyterlab
conda deactivate
conda remove --name dev --all
conda info --envs
conda update conda
conda create -n dev python=3.7 anaconda
python -m pip install pandas
pip install jupyter 
#check if pandas is installed successfully
conda list pandas
#check if jupyterlab is listed successfully
conda list jupyterlab
```



## Usage

To use the Crypto Arbitrage application simply clone the repository, download applicants_data.csv,   and run the **machine_learning_trading_bot.ipynb** with:

```python
jupyter lab
```

