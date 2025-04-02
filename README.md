## RNN vs. LSTM vs. GRU - Sequence Prediction

### Overview
This project demonstrates the use of different recurrent neural network (RNN) architectures for sequence prediction. It compares three types of models:
- **Simple RNN**
- **LSTM (Long Short-Term Memory)**
- **GRU (Gated Recurrent Unit)**

Each model is trained to predict the next number in a simple numerical sequence.

### Requirements
To run this project, you need Python and the following libraries installed:

```bash
pip install numpy tensorflow
```

### Dataset
The dataset consists of small numerical sequences, where each sequence predicts the next number:

**Example Data:**
```plaintext
Inputs:  [[1, 2, 3], [2, 3, 4], [3, 4, 5]]
Targets: [4, 5, 6]
```

### Model Training
The `train_model()` function trains a model based on the specified type (`RNN`, `LSTM`, or `GRU`). Each model consists of:
- A recurrent layer (`SimpleRNN`, `LSTM`, or `GRU`)
- A dense output layer
- Adam optimizer and Mean Squared Error (MSE) loss function

### Running the Project
Execute the script to train all three models and compare their predictions:

```bash
python script.py
```

#### Expected Output Format:
```plaintext
RNN Final Loss: 0.XXXX
LSTM Final Loss: 0.XXXX
GRU Final Loss: 0.XXXX

RNN Prediction: X.XXXX
LSTM Prediction: X.XXXX
GRU Prediction: X.XXXX
```

### Usage
- Modify the input sequences to experiment with different time series data.
- Change the number of neurons in each model to see how it affects performance.
- Compare the effectiveness of RNN, LSTM, and GRU for different sequence lengths.

### License
This project is open-source and available under the MIT License.


