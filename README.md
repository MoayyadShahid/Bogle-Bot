# 📈 Bogle Bot - Stock Market Predictor

This repository contains the code for a Streamlit app designed to predict stock prices using historical data from Yahoo Finance. The prediction model is implemented using TensorFlow and Keras, providing insights into future stock trends.

![example](https://github.com/MoayyadShahid/Bogle-Bot/assets/55198028/d82d497f-3a96-4082-979d-cc05ea1244f3)

## 🚀 Features

- **Real-time stock data fetching** using `yfinance`.
- **Predictive modeling** with a pre-trained TensorFlow model.
- **Interactive visualizations** with `matplotlib` showing historical data and predictions.
- **User-friendly interface** built with Streamlit.

## 🛠 Installation

To get started with this project, clone the repository and install the required dependencies.

```bash
git clone https://your-repository-url.git
cd your-repository-directory
pip install -r requirements.txt
```

This sets up everything needed to run the app locally. Ensure that you replace https://your-repository-url.git with the actual URL of your GitHub repository.

## 🖥 Usage

To run the app locally, navigate to the project directory and run the following command:

```bash
streamlit run app.py
```

Visit http://localhost:8501 in your web browser to interact with the app. This will allow you to see the app in action, input different stock symbols, and view the results dynamically as you interact with the interface.

## 🧠 Model Details

The stock prediction model is trained on historical data from Yahoo Finance, utilizing a neural network architecture crafted with TensorFlow and Keras. Below is a detailed breakdown of the process involved in creating and deploying this model:

### Data Preprocessing
The model starts with data preprocessing where historical stock data is fetched and prepared. This involves:
- **Normalization**: Scaling the stock prices to a normal range, typically 0 to 1, which helps in speeding up the training process.
- **Segmentation**: Dividing the data into training and testing datasets to ensure the model is validated accurately.

### Model Creation
The model is constructed using Keras layers within TensorFlow:
- **Dense Layers**: Fully connected layers that bring depth to the network.
- **Dropout Layers**: Used to prevent overfitting by randomly dropping units during training.
- **LSTM Layers**: Long Short-Term Memory units are great for making predictions based on time series data.

### Training the Model
- The model is trained using the backpropagation algorithm, where it learns from the historical data.
- We use a loss function and an optimizer to measure how well the model performs and to improve it iteratively.

### Testing the Model
- After training, the model is tested against unseen data, the testing set extracted during preprocessing.
- This phase helps to evaluate the accuracy and effectiveness of the model in predicting stock trends.

## 📊 Data Visualizations

The app provides interactive charts displaying historical stock prices, moving averages, and predictive trends. These visualizations help users understand the stock performance over time and the model's predictions, enhancing the interactive experience of the app.

## 🤝 Contributing

Contributions to improve the app or the predictive model are welcome. Please feel free to fork the repository, make changes, and submit a pull request. Here's how you can contribute:

1. **Fork the Repository**: Click on the fork button on the repository's page. This will create a copy of the current repository in your account.
2. **Make Changes Locally**: Clone the forked repository to your machine and make the changes you wish to implement.
3. **Commit Changes**: After making your changes, commit them with a clear commit message explaining the enhancements.
4. **Push to the Branch**: Push your changes to your fork.
5. **Open a Pull Request**: Open a pull request to the original repository with a detailed description of what changes you've made and why.

Your contributions are highly appreciated!
