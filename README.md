Sequential Data Classification – RNN, LSTM & GRU

This project builds and compares RNN, LSTM, and GRU models on two sequential datasets:

Handwritten Character Stroke Sequences

Hindi CV Speech MFCC Sequences

The objective is to identify the best recurrent architecture for each dataset.

📦 Datasets
1. Handwriting Dataset

5 classes of Kannada/Telugu characters

Each sample → sequence of (x, y) coordinates

Variable sequence lengths

2. MFCC CV Speech Dataset

5 Hindi CV classes

Each sample → sequence of 39-dim MFCC vectors

Variable sequence lengths

🔧 Methods & Hyperparameters

Models: RNN, LSTM, GRU

Layers: 1, 2

Hidden Units: 64, 128

Optimizer: Adam (0.001)

Loss: CrossEntropy

Early stopping: Loss change < 1e-4

🧠 Best Models
Dataset	Best Model
Handwriting	LSTM (1 layer, 128 hidden)
MFCC Speech	GRU (2 layers, 128 hidden)

Plots (accuracy + confusion matrix) for the best models are included in the notebook.

🏁 Conclusion

LSTM performs best for smooth, continuous coordinate sequences.

GRU performs best for MFCC speech features due to efficiency and fast temporal modeling.

Hyperparameter tuning significantly impacts model performance.

👥 Contributors

Arpit Pandey, Sooraj Veer R, Chinmay Bhat, Satish Kumar,
Sujay Das, Ronit Datta, Anmol Kashyap,
Gavinolla Abhishek Reddy, Ayush Kumar
