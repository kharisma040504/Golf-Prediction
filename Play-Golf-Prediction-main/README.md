# Play-Golf-Prediction ⛳

## Project Description
The **Play Golf Prediction** project aims to predict whether it is suitable to play golf based on weather conditions, such as outlook, temperature, humidity, and wind. Using machine learning classification techniques, this project models the decision-making process to determine "Play" or "Don't Play" scenarios. The project emphasizes systematic data preprocessing, exploratory data analysis (EDA), and model evaluation to deliver robust predictions.

By leveraging these techniques, the project contributes to understanding environmental factors influencing human decision-making, while also providing a practical implementation of machine learning concepts.

---

## Project Structure

```
Play-Golf-Prediction/
├── data/               
├── notebooks/          
├── README.md           
└── requirements.txt    
```

---

## Workflow

### **1. Data Exploration**
- Perform exploratory data analysis (EDA) to understand the dataset's structure, distributions, and correlations.
- Visualize the relationships between weather conditions and the decision to play golf (e.g., correlation between humidity and "Play").
- Identify and handle missing or inconsistent data.

### **2. Data Preprocessing**
- **Handle Missing Values:**
  - Fill missing data for temperature, outlook, or humidity using appropriate imputation techniques (mean/mode).
- **Feature Engineering:**
  - Encode categorical variables such as outlook (e.g., Sunny, Overcast, Rainy) and wind (e.g., Weak, Strong) using one-hot encoding.
- **Normalization:**
  - Scale numerical features like temperature and humidity to improve model performance.

### **3. Modeling**
- Train classification models using:
  - **Decision Tree Classifier:** For interpretable decision-making.
  - **Random Forest Classifier:** For robust predictions by aggregating multiple decision trees.
  - **Logistic Regression:** For baseline comparison in classification tasks.

### **4. Model Evaluation**
- Evaluate model performance using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix
- Use cross-validation to ensure model generalizability.

### **5. Results Interpretation**
- Analyze feature importance to identify which weather conditions influence the decision most significantly.
- Visualize model performance using metrics such as confusion matrices and feature importance plots.

---

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/2AM-Labs/Play-Golf-Prediction.git
   ```
2. Navigate to the project folder:
   ```bash
   cd Play-Golf-Prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the notebook for data exploration and modeling:
   ```bash
   jupyter notebook notebooks/play_golf_analysis.ipynb
   ```

---

## Technologies Used

- **Programming Language:** Python 3.9+
- **Libraries and Tools:**
  - **Pandas:** For data manipulation and cleaning.
  - **NumPy:** For numerical computations.
  - **Scikit-learn:** For machine learning models and evaluation metrics.
  - **Matplotlib & Seaborn:** For data visualization.
  - **Jupyter Notebook:** For interactive experimentation and documentation.

---

## Dataset Information
- **Attributes:**
  - **Outlook:** Sunny, Overcast, Rainy
  - **Temperature:** Hot, Mild, Cool
  - **Humidity:** High, Normal
  - **Wind:** Weak, Strong
  - **Target Variable:** Play (Yes/No)
- **Data Source:** A weather dataset designed for binary classification tasks.

---

## Results and Analysis
- **Key Insights:**
  - Outlook and humidity are the most significant predictors of whether golf is playable.
  - Wind strength has a secondary but notable influence on the decision.

---

## Documentation and Resources
- **Presentation Deck:** [Play Golf Presentation](https://www.canva.com/design/DAFyVvQu-to/Z-xMuUJ4Y53XjjckrCGLvw/view?utm_content=DAFyVvQu-to&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h5959a7de4f)
- **Exploratory Notebooks:** Detailed steps for data exploration and modeling are available in the `notebooks/` folder.
- **Technical Reports:** Additional findings and documentation are in the `docs/` folder.

---

## Contribution Guidelines

1. Fork this repository.
2. Create a new branch for features or fixes:
   ```bash
   git checkout -b feature-branch-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Description of changes"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-branch-name
   ```
5. Create a pull request on GitHub.

---

# requirements.txt

```
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter
