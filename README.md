# Chess Opening Analysis & Winner Prediction

# <a href="Report.pdf" class="image fit"><img src="images/marr_pic.jpg" alt="">Link to Report</a>

A comprehensive statistical analysis and machine learning approach to understanding chess opening moves and predicting game outcomes.

## 📊 Project Overview

This project analyzes chess game data to understand the relationship between opening moves and game outcomes. We explore various statistical patterns in chess gameplay and develop machine learning models to predict winners based on opening sequences.

## 🎯 Objectives

- **Statistical Analysis**: Examine correlations between opening moves and win rates
- **Hypothesis Testing**: Determine if certain opening moves significantly impact victory
- **Predictive Modeling**: Build models to predict game winners from opening sequences
- **Pattern Recognition**: Identify strategic patterns that differentiate player skill levels

## 📈 Key Findings

### Statistical Insights

- **Opening moves have a statistically significant impact on game outcomes** (p ≈ 0, Chi-square test)
- **No significant rating difference between white and black players** (t-test for independence)
- **No single "best" opening move** exists that guarantees higher win rates (Kruskal-Wallis test)
- **White players show more predictable winning patterns** in opening sequences

### Model Performance

| Model                    | Accuracy | Precision | Recall |
| ------------------------ | -------- | --------- | ------ |
| Decision Tree (Baseline) | 59%      | 59%       | 59%    |
| Neural Network           | 50%      | 50%       | 50%    |
| BERT Transformer         | 60.2%    | 60%       | 60%    |

### Findings

- Decision trees and transformers significantly outperformed neural networks
- Both successful models showed bias toward predicting white victories
- Transformer model achieved slight edge with 60.2% accuracy

## 🔧 Methodology

### Data Processing

- **Dataset**: Lichess online chess platform games
- **Features**: Player ratings, move sequences, opening classifications, victory conditions
- **Engineering**: Extracted first 10 moves, one-hot encoded openings
- **Size**: Large-scale dataset with comprehensive game metadata

### Statistical Analysis

1. **T-test for Independence**: Comparing player ratings by color
2. **Chi-square Test**: Opening moves vs. victory status relationship
3. **Kruskal-Wallis Test**: Comparing win rates across top 10 opening moves

### Machine Learning Models

1. **Decision Tree (Baseline)**: Gini criterion with depth optimization
2. **Random Forest**: Ensemble method to reduce overfitting
3. **Neural Network**: 5 hidden layers with sigmoid activation
4. **BERT Transformer**: Fine-tuned language model for move sequences

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy scikit-learn tensorflow transformers
pip install matplotlib seaborn chess python-chess
```

## 🔍 Technical Highlights

- **Feature Engineering**: Sophisticated move sequence parsing and encoding
- **Overfitting Management**: Grid search optimization and ensemble methods
- **Deep Learning**: Novel application of BERT transformers to chess notation
- **Statistical Rigor**: Multiple hypothesis tests with proper significance testing

## 📚 Research Background

This work builds upon existing chess analysis research, particularly "Predicting Chess Opening Through Modelling Of Chess" by Chowdhury & Sen (2021). Our approach differs by focusing on winner prediction rather than move prediction, utilizing modern deep learning architectures.

## 🎯 Future Work

- **Custom Chess Transformer**: Train transformer specifically on chess notation
- **White Advantage Analysis**: Investigate why models predict white victories more accurately
- **Extended Move Sequences**: Analyze beyond opening moves (10+ moves)
- **Real-time Prediction**: Deploy models for live game analysis

## 👥 Contributors

**Group 10 - Math 189 Project**

- Qirui Zheng (A17317403)
- Samantha Lin (A16758004)
- William Kam (A16940420)
- Aryan Kanuparti (A18093864)
- Derek Klopstein (A17008856)
- Daniel Gitelman (A16861627)

---

⭐ **Star this repo** if you found our chess analysis interesting!
