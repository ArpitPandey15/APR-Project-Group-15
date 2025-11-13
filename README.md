# Sequential Data Classification – RNN, LSTM & GRU

This project compares Recurrent Neural Network architectures — **RNN**, **LSTM**, and **GRU** — on two sequential datasets:

1. **Handwritten Character Stroke Sequences**
2. **Hindi CV Speech MFCC Sequences**

The goal is to identify the best-performing recurrent model for each dataset.

---

## 📦 Datasets

### 1. Handwriting Dataset
- 5 Kannada/Telugu character classes  
- Each sample is a sequence of `(x, y)` coordinates  
- Variable sequence lengths  

### 2. MFCC CV Speech Dataset
- 5 Hindi Consonant-Vowel (CV) classes  
- Each sample is a sequence of **39-dimensional MFCC features**  
- Variable-length audio-derived sequences  

---

## 🔧 Methods & Hyperparameters

- Models used: **RNN**, **LSTM**, **GRU**
- Tested layers: `1`, `2`
- Hidden units: `64`, `128`
- Optimizer: **Adam (lr=0.001)**
- Loss: **CrossEntropy**
- Early stopping: Convergence threshold of `1e-4` change in epoch loss

---

## 🧠 Best Model Results

| Dataset | Best Model |
|--------|------------|
| Handwriting | **LSTM — 1 layer, 128 hidden units** |
| MFCC Speech | **GRU — 2 layers, 128 hidden units** |

Accuracy curves and confusion matrices for these models are included in the notebook and report.

---

## 🏁 Conclusion

- **LSTM** handles smooth coordinate-based sequences effectively, giving best results on handwriting data.  
- **GRU** is computationally efficient and performs best on MFCC speech features.  
- Hyperparameter tuning and early stopping significantly improve overall accuracy.

---

## 👥 Contributors

- Arpit Pandey  
- Sooraj Veer R  
- Chinmay Bhat  
- Satish Kumar  
- Sujay Das  
- Ronit Datta  
- Anmol Kashyap  
- Gavinolla Abhishek Reddy  
- Ayush Kumar

---
