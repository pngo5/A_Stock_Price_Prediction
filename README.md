# Stock Price Prediction System

## Overview
This project uses Long Short-Term Memory (LSTM) neural networks to predict future stock prices based on historical data. The implementation focuses specifically on predicting VERU stock prices, providing investors and analysts with a data-driven approach to understanding potential market movements.

## Features
- Historical stock data retrieval using pandas_datareader
- Data preprocessing and normalization for optimal model performance
- LSTM model implementation for time series forecasting
- Visualization of prediction results against actual stock data
- Docker containerization for easy deployment and reproducibility

## Technical Architecture
The project implements a deep learning approach utilizing LSTM (Long Short-Term Memory) networks, which are particularly effective for time series forecasting. LSTMs are a specialized form of recurrent neural networks capable of learning long-term dependencies in sequential data, making them ideal for stock price prediction where patterns may develop over extended periods.

## Technologies Used
- **Python 3.7+**
- **TensorFlow 1.8.0**: Deep learning framework
- **Keras 2.2.0**: High-level neural networks API
- **scikit-learn 0.24.0**: Machine learning library
- **pandas 1.1.3**: Data manipulation and analysis
- **pandas_datareader 0.9.0**: Remote data access
- **NumPy 1.19.4**: Numerical computing
- **Matplotlib 3.3.3**: Data visualization
- **Docker**: Containerization

## Environment Requirements
- Anaconda3:4.4.0 (recommended for dependency management)
- Docker for containerized deployment

## Installation and Setup

### Using Docker (Recommended)
1. Clone the repository:
   ```bash
   git clone https://github.com/pngo5/A_Stock_Price_Prediction.git
   cd A_Stock_Price_Prediction
   ```

2. Build and run the Docker container:
   ```bash
   docker run -it -p 8888:8888 model --allow-root
   ```

3. Access Jupyter Notebook at `http://localhost:8888` in your browser

### Manual Installation
1. Clone the repository
2. Create a conda environment:
   ```bash
   conda create -n stock-prediction python=3.7
   conda activate stock-prediction
   ```

3. Install required packages:
   ```bash
   pip install tensorflow==1.8.0 keras==2.2.0 scikit-learn==0.24.0 pandas==1.1.3 pandas_datareader==0.9.0 numpy==1.19.4 matplotlib==3.3.3
   ```

## Usage
1. Start the Jupyter Notebook server
2. Open the main notebook file
3. Run the cells sequentially to:
   - Load and preprocess historical stock data
   - Configure and train the LSTM model
   - Generate predictions
   - Visualize the results

## Data Sources
The project uses historical stock price data for VERU obtained through Yahoo Finance API via pandas_datareader.

## Model Architecture
The LSTM model is designed to capture temporal patterns in stock price movements with:
- Multiple LSTM layers for learning sequential patterns
- Dropout layers to prevent overfitting
- Dense output layer for price prediction

## Results and Evaluation
The model's performance is evaluated using standard metrics for regression tasks:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Visual comparison of predicted vs. actual price trends

## Future Improvements
- Incorporate additional features like trading volume and technical indicators
- Experiment with different network architectures (GRU, Bidirectional LSTM)
- Implement sentiment analysis from news and social media
- Develop an interactive web interface for real-time predictions

## Resources
- [Illustrated Guide to LSTMs and GRU's](https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21)
- [How to Run Jupyter Notebook on Docker](https://towardsdatascience.com/how-to-run-jupyter-notebook-on-docker-7c9748ed209f)
- [Jupyter Lab on Docker with Windows](https://medium.com/@alexjsanchez/jupyter-lab-on-docker-with-windows-368a24e18d0)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support and Contact
- **GitHub Repository**: [https://github.com/pngo5/A_Stock_Price_Prediction](https://github.com/pngo5/A_Stock_Price_Prediction)
- **Report Issues**: [https://github.com/pngo5/A_Stock_Price_Prediction/issues](https://github.com/pngo5/A_Stock_Price_Prediction/issues)
- **Email**: pngo5@example.com (replace with your actual email)

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
