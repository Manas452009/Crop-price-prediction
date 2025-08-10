#  Crop Price Prediction

A machine learning project to predict crop prices based on **weather conditions** and **soil types**.  
The system uses historical crop price data along with temperature, rainfall, humidity, and soil features to forecast future prices, helping farmers and traders make informed decisions.

---

##  Features
- **Data-driven price prediction** using historical datasets (2019–2024).
- Considers:
  -  Weather conditions (min/max temperature, humidity, rainfall)
  -  Soil type information
  -  Seasonal and monthly trends
- Built using **Python** and **XGBoost**.
- Modular and scalable for additional crops or states.

---

## Dataset
The dataset includes:
| Column Name | Description |
|-------------|-------------|
| State | State/region where the crop is grown |
| Commodity | Name of the crop |
| Year | Year of observation |
| Month | Month of observation |
| Min_Price | Minimum price recorded |
| Max_Price | Maximum price recorded |
| Predominant Soil Types | Major soil type for the area |
| Min_Temp | Minimum temperature |
| Max_Temp | Maximum temperature |
| Humidity | Average humidity |
| Rainfall | Total rainfall |

> **Note:** The dataset is stored locally due to its large size.  
> To use this project, place your dataset in the `src/` folder as `merged_data.csv`.

---

##  Installation & Setup
1. **Clone the repository**
   ```bash
   git clone https://github.com/Manas452009/Crop-price-prediction.git
   cd Crop-price-prediction

## Create a virtual environment (optional but recommended)
    python -m venv .venv
    source .venv/bin/activate    # On Linux/Mac
    .venv\Scripts\activate       # On Windows

## Install dependencies
    pip install -r requirements.txt

## Run the model training
    python train_model.py

## Model Performance
    Metric	Train Score	Test Score
    R² Score	0.8196	0.72
    MAE	        0.39	-
    RMSE        0.55	-

## Technologies Used
1. Python (pandas, numpy, matplotlib, seaborn)
2. XGBoost for regression
3. Scikit-learn for preprocessing & metrics
4. SPSS for additional statistical analysis

## Future Improvements
1. Integrate real-time weather API for up-to-date predictions.
2. Expand dataset to include more states and crop types.
3. Build a web-based dashboard for farmer-friendly predictions.

## Author
Manas Mishra
Manas452009