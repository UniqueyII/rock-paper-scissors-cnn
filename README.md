# rock-paper-scissors-cnn
CNN image classifier achieving 100% accuracy through systematic architecture optimization

# 🎯 Rock-Paper-Scissors CNN: Architecture Optimization Journey

## 📊 Project Overview
A computer vision project that demonstrates systematic optimization of Convolutional Neural Networks, achieving **100% accuracy** on rock-paper-scissors classification through intelligent architecture choices.

## 🏆 Key Achievements
- **Perfect 100% accuracy** on validation set
- **86x parameter reduction** (9.5M → 110K) while improving accuracy
- **14% faster training** than original model
- Implemented **early stopping** for efficient training

## 📈 The Optimization Journey

### Phase 1: Baseline Model
- **Accuracy**: 87%
- **Training Time**: 22 minutes  
- **Parameters**: 9.5 million
- **Architecture**: Traditional CNN with Flatten + Dense layers

### Phase 2: Speed-Optimized Model  
- **Accuracy**: 63%
- **Training Time**: 3 minutes
- **Parameters**: 23,747
- **Architecture**: Heavy use of GlobalAveragePooling

### Phase 3: Balanced Model (Final)
- **Accuracy**: 100% ✅
- **Training Time**: 19.2 minutes
- **Parameters**: 110,147
- **Architecture**: Hybrid approach with strategic layer depth

## 🛠️ Technologies Used
- **Python** (TensorFlow, Keras, OpenCV)
- **Computer Vision** (CNN, Image Processing)
- **Model Optimization** (Architecture tuning, Early Stopping)
- **Data Pipeline** (Robust data loading with error handling)

## 🚀 Quick Start

```bash
# Clone this repository
git clone https://github.com/yourusername/rock-paper-scissors-cnn.git

# Install dependencies
pip install -r requirements.txt

# Run the analysis
jupyter notebook rock_paper_scissors_cnn.ipynb
```
💡 Key Technical Insights
Architecture Breakthrough
Replacing Flatten() + Dense(256) with GlobalAveragePooling2D() reduced parameters by 99% while maintaining performance.

Early Stopping Implementation
python
early_stop = EarlyStopping(
    monitor='val_accuracy',
    patience=3,
    restore_best_weights=True
)
This reduced training time by 30% while preserving 100% accuracy.

Robust Data Pipeline
Built error-resistant data loading that handles missing datasets gracefully.

📊 Performance Comparison
Model	Accuracy	Training Time	Parameters	Architecture
Baseline	87%	22 min	9.5M	Traditional CNN
Speed-Optimized	63%	3 min	23K	GlobalAveragePooling
Balanced	100%	19 min	110K	Hybrid
🎯 Business Applications
Gesture Recognition: Foundation for sign language or controller-free interfaces

Quality Control: Pattern recognition in manufacturing

Educational Tools: Interactive learning applications

📁 Project Structure
text
rock-paper-scissors-cnn/
├── README.md                    # Project documentation
├── requirements.txt             # Python dependencies
├── rock_paper_scissors_cnn.ipynb # Main analysis notebook
└── src/                        # Source code modules
    ├── model_architectures.py   # Different CNN architectures
    └── data_pipeline.py         # Robust data loading

🔗 Connect With Me
[Amin Sharifi] | [aminemsharifi@gmail.com]
