# Exploring Youth Drug Use Patterns: A Decision Tree Analysis

## Overview  
This project analyzes youth drug use patterns (cigarettes, alcohol, and marijuana) using decision tree and random forest models applied to the 2020 National Survey on Drug Use and Health (NSDUH). It investigates key predictors of drug use behaviors and discusses their implications for public health.

## Objectives  
- Predict youth cigarette frequency, alcohol use, and marijuana frequency using machine learning models.  
- Compare performance metrics (e.g., Mean Squared Error, classification accuracy) for decision tree and random forest models.  
- Identify significant predictors and their influence on youth drug use.  

## Dataset  

- **Source**: National Survey on Drug Use and Health (NSDUH), 2020.  
- **Target Variables**:  
  - *Cigarette Frequency*: Continuous variable (monthly frequency).  
  - *Alcohol Use*: Binary classification (used or not used).  
  - *Marijuana Frequency*: Multi-class classification (frequency categories).  
- **Features**:  
  - Demographic data  
  - Youth experiences  
  - Parental attitudes  
  - School influences  
  - Peer behaviors  

## Methodology  

### **Data Preparation**  
1. Loaded the `youth_data` dataset (pre-processed NSDUH data).  
2. Handled missing values using case-wise deletion.  
3. Conducted exploratory analysis with summary statistics and visualizations.  
4. Created target variables:  
   - **Cigarette Frequency**: Continuous variable (monthly frequency).  
   - **Alcohol Use**: Binary classification (used or not used).  
   - **Marijuana Frequency**: Multi-class classification (frequency categories).  
5. Split data into training (80%) and testing (20%) sets for model evaluation.  

### **Models**  

#### 1. Decision Trees  
- Built decision tree models for regression and classification tasks.  
- Used cross-validation to prune overfitted trees.  
- Visualized tree structures for interpretability.  
- Evaluated performance using MSE (regression) and accuracy (classification).  

#### 2. Random Forest  
- Trained random forest models to reduce variance and improve accuracy.  
- Generated feature importance plots to identify key predictors.  
- Compared performance metrics with decision trees.  

## Results  

### **Model Performance**  

#### 1. Cigarette Frequency (Regression)  
- **Decision Tree MSE**: 3.44  
- **Random Forest MSE**: 2.68  

#### 2. Alcohol Use (Binary Classification)  
- **Decision Tree Accuracy**: 79.97%  
- **Random Forest Accuracy**: 81.26%  

#### 3. Marijuana Frequency (Multi-class Classification)  
- **Decision Tree Accuracy**: 86.4%  
- **Random Forest Accuracy**: 86.3%  

### **Key Findings**  
- **Cigarette Frequency**: Youth selling illegal drugs and peer smoking behavior are significant predictors.  
- **Alcohol Use**: Peer marijuana use and individual attitudes strongly influence alcohol consumption.  
- **Marijuana Frequency**: School grade and peer usage are critical factors.  

### **Visualization**  
- Decision tree visualizations for regression and classification tasks.  
- Random forest feature importance plots.  

## Dependencies  

### **Language**  
- R  

### **Libraries**  
- `rpart` (Decision Trees)  
- `randomForest` (Random Forest)  
- `rpart.plot` (Tree Visualization)  
- `ggplot2` (Visualizations)  

## Usage  

1. Install required R packages:  
   ```r
   install.packages(c("rpart", "randomForest", "rpart.plot", "ggplot2"))
