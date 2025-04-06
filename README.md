# IE0005-DSAI


<h1>Stock Price Volatility Prediction with LSTM and Frontend Dashboard</h1>
This project, developed by Unnav Sharma, Naman Srivastava, Arjun Dabral, and Benjamin Yap, focuses on predicting stock price volatility using machine learning models, with a particular emphasis on Long Short-Term Memory (LSTM) networks. We utilized a dataset of Tesla stock prices spanning over 10 years, sourced from Kaggle, to build and evaluate our models. The final model is integrated into an interactive frontend dashboard built with Tailwind CSS and JavaScript for seamless user interaction.

<h2>Workflow</h2>
<h3>Data Analysis, Cleaning, and Visualization</h3>

We began by performing exploratory data analysis (EDA) on the Tesla stock price dataset using Python libraries such as Seaborn, Matplotlib, and Scikit-learn. This step involved identifying trends, patterns, and anomalies in the time series data. We cleaned the dataset by handling missing values, normalizing the data, and preparing it for model training.

<h3>Model Development and Evaluation</h3>

Four machine learning models were implemented to predict stock price volatility: Logistic Regression, XGBoost, Random Forest, and LSTM. Each model was trained and tested on the preprocessed dataset. After rigorous evaluation, LSTM emerged as the superior model for time series data due to its ability to capture long-term dependencies and handle sequential patterns effectively.

<h3>LSTM Architecture</h3>

The LSTM model, a type of recurrent neural network (RNN), was chosen for its robustness in time series prediction. Below is the architecture of an LSTM cell, which consists of several gates that regulate the flow of information:
![image](https://github.com/user-attachments/assets/bf3e432c-a1d2-4c56-b6db-03d34cf3247f)




Forget Gate (f<t>): Decides which information from the previous cell state (C<t-1>) to discard.
Input Gate (i<t>): Determines which new information from the current input (x<t>) and previous hidden state (h<t-1>) to store in the cell state.
Cell State Update (C<t>): Combines the previous cell state (after forgetting) with new information (via the input gate and a Tanh activation) to update the cell state.
Output Gate (o<t>): Controls what parts of the cell state are output to the hidden state (h<t>), which is passed to the next time step.
The Tanh activation functions ensure that values are scaled appropriately, while the gates use sigmoid activations (σ) to produce values between 0 and 1, effectively acting as filters.
Frontend Integration

The trained LSTM model was integrated into a user-friendly dashboard built using Tailwind CSS and JavaScript. The frontend allows users to input parameters, visualize predictions, and explore stock price volatility trends interactively. The dashboard is designed to be responsive and intuitive, ensuring a seamless experience for end users.

Why LSTM?
LSTM outperformed other models like Logistic Regression, XGBoost, and Random Forest in our tests, as it is specifically designed for sequential data. Its ability to retain long-term dependencies through the cell state and gates makes it ideal for time series tasks like stock price volatility prediction.

Tools and Technologies
Data Analysis and Visualization: Seaborn, Matplotlib, Scikit-learn
Machine Learning Models: Logistic Regression, XGBoost, Random Forest, LSTM
Frontend: Tailwind CSS, JavaScript
Dataset: Tesla stock price data (10+ years) from Kaggle
Feel free to explore the code, contribute, or provide feedback!

<h3>Access the frontend website for the dashboard of the stock volatility that I and my team have curated:</h3>
https://v0-tesla-stock-dashboard-gold.vercel.app/

![image](https://github.com/user-attachments/assets/71b36689-807f-4a8d-8edc-73c331f6019f)
