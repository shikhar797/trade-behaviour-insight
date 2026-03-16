# trade-behaviour-insight

For performing the above program you need to have Python installed and the required Python packages, which you can install using the following commands:

1. pip install pandas  

2. pip install numpy  

3. pip install matplotlib  

So let's start the explanation of Trade-behavior Analysis.

Step 1: Import the dataset  

In the first step I imported both 'fear_greed_index.csv' file and 'historical_data.csv' file.


Step 2: Preprocessing of the data  

In this step you will make your data in a format so that we can use it for analysis.

Here I identified the columns which are very useful for me:

1. Account and Date, through which I can get 'trader_per_day'.

2. PnL, through which I can get the total number of profitable and loss trades in a day.

3. I calculated buy and sell per day, which will be very helpful for classifying the buy and sell in each emotion such as greed, fear, neutral, etc.

4. I dropped unnecessary columns.

5. I grouped the data based on Date and Account.

6. Then I joined both data frames of 'fear_greed_index.csv' file and 'historical_data.csv' file using a left outer join.

Step 3: Analysis

1. I plotted the graph of Emotions and buy and sell on that particular emotion.

2. I plotted the graph of Emotions and total trade per day.

3. I plotted the graph of number of losses and Emotions.


========= conclusion =========

1. By the graph of Emotions and buy and sell on that particular emotion, I understand that during fear people are buying and selling the most.

<img src="graph1.png" alt="My Project Screenshot" width="300" height="200">


2. By the graph of Emotions and total trade per day, I understand that during extreme greed people are doing the least number of trades.

<img src="graph2.png" alt="My Project Screenshot" width="300" height="200">


3. By the graph of number of losses and Emotions, I understand that losses during fear and greed are extremely high.

<img src="graph3.png" alt="My Project Screenshot" width="300" height="200">