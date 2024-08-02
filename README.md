## Credit Card Fraud Detection using Autoencoder

This project uses an autoencoder neural network to detect anomalies in credit card transactions, with the goal of identifying fraudulent transactions.

### Requirements

The project requires the following Python packages:

- torch
- torchvision 
- pandas
- numpy
- matplotlib
- scikit-learn
- kaggle

You can install the required packages by running:

```bash
pip install -r requirements.txt
```

The `requirements.txt` file contains:

```
torch
torchvision
pandas
numpy
matplotlib
scikit-learn
kaggle
```

### Usage

1. **Install the required packages**:

```bash
pip install -r requirements.txt
```

2. **Download the dataset**:

```bash
kaggle datasets download -d mlg-ulb/creditcardfraud
unzip creditcardfraud.zip
```

3. **Run the anomaly detection script**:

```bash
python anomalydetection.py
```

This will train an autoencoder model on the normal credit card transactions, and then detect anomalies based on the reconstruction error. The script will output the number of detected anomalies, actual frauds, true positives, false positives, true negatives, and false negatives.

4. **Visualize the results**:

The script will generate a histogram plot showing the distribution of reconstruction errors. This can help in setting an appropriate threshold for anomaly detection.

### Acknowledgments

- The dataset used in this project is from the [Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud) dataset on Kaggle.
- The autoencoder architecture and training process are based on the [Anomaly Detection using Autoencoder](https://www.kaggle.com/code/sudalairajkumar/anomaly-detection-using-autoencoder) kernel on Kaggle.
