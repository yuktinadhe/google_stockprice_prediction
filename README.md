## 📈 Google Stock Price Prediction using LSTM
This project demonstrates how to build a Recurrent Neural Network (RNN) using LSTM layers to predict the closing stock price of Google based on historical data. The model was built and trained using Keras with TensorFlow backend.

## 🧠 Tech Stack & Libraries
- Python
- NumPy & Pandas
- Matplotlib
- TensorFlow / Keras
- Scikit-learn
- Regular Expressions (for data cleaning)

## 📊 Dataset
- Source: Google_Stock_Price_Train.csv
- Features: Date, Close
- Columns like Open, High, Low, and Volume were dropped during preprocessing.

## ⚙️ Workflow
Part 1: Data Preprocessing
- Cleaned comma-separated numeric strings using RegEx.
- Used only the Close price and formatted Date.
- Applied MinMaxScaler to normalize data.
- Created time series structure with 100 timesteps as input and 1 timestep as output.
- Reshaped input to match LSTM requirements: (samples, timesteps, features).

Part 2: Build and Train the RNN
- Used 4 stacked LSTM layers with Dropout regularization.
- Compiled with adam optimizer and mean_squared_error loss.
- Trained on the training set.

Part 3: Prediction and Visualization
- Prepared test data similarly with scaling and reshaping.
- Predicted test set results and inverse-transformed the predictions.
- Visualized predicted vs real stock prices using Matplotlib.

## 📷 Sample Output
![image](https://github.com/user-attachments/assets/4de7711f-b714-48d0-bde2-4da0c765cd90)


## 📌 Possible Enhancements
- Predict multiple days ahead (multi-step forecasting)
- Add more features like volume, moving averages, etc.
- Deploy the model using Flask or Streamlit
- Add news sentiment data to improve accuracy

## 🤝 Connect with Me
- GitHub: yuktinadhe
- LinkedIn: https://www.linkedin.com/in/yukti-nadhe-47342b21b/
## Yukti Nadhe
