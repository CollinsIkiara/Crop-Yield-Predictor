# Crop Yield Prediction

## Project Title
Machine Learning-Based Yield Prediction Model

## Project Description
This project leverages machine learning techniques to predict crop yields, with a specific focus on rice production. By analyzing various agricultural and environmental factors, the model aims to provide accurate yield forecasts. While the dataset includes information on 22 different crops, this project concentrates on rice yield prediction as a proof of concept. The goal is to assist farmers, agricultural planners, and policymakers in making informed decisions about crop management and resource allocation.

## Installation Instructions
1. Clone this repository:
   ```
   git clone https://github.com/CollinsIkiara/crop-yield-prediction.git
   cd crop-yield-prediction
   ```
2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
3. Install required libraries:
   ```
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```

## Usage
1. Open the `Crop Yield Prediction.ipynb` notebook in Jupyter.
2. Run the cells sequentially to perform data analysis, preprocessing, model training, and evaluation.
3. To make predictions with the trained model:
   ```python
   # Example usage (replace with actual values)
   input_data = [[20, 80, 7, 200, 25, 85]]  # Example: temperature, humidity, pH, rainfall, nitrogen, phosphorus
   prediction = model.predict(input_data)
   print(f"Predicted rice yield: {prediction[0]} kg/hectare")
   ```

## Data
- **Dataset**: Crop Price Prediction Dataset (source: [Kaggle](https://www.kaggle.com/datasets/varshitanalluri/crop-price-prediction-dataset))
- **Features**: Soil composition (Nitrogen, Phosphorus, and Potassium levels), environmental factors (temperature, humidity, pH, rainfall), and other relevant agricultural parameters
- **Target**: Yield 
- **Preprocessing**: Handled missing values, normalized numerical features, and encoded categorical variables where applicable

## Methodology
1. **Data Analysis**: Explored the dataset structure, visualized feature distributions and correlations, and identified patterns affecting yield.
2. **Feature Selection and Engineering**: Selected relevant features based on domain knowledge and correlation analysis. 
3. **Model Implementation**: Experimented with the Random Forest model and performed hyperparameter tuning.
4. **Model Evaluation**: Assessed model performance using metrics such as accuracy, precision, recall, and F1-score.

## Results
- The Random Forest model had a performance of 90% accuracy. However, upon performing cross-validation, that figure was reduced to 82%.
- The model shows good generalization ability across different regions in the dataset.

## Contributors
- [Collins Ikiara](https://github.com/CollinsIkiara)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Conclusion
This machine learning-based rice yield prediction model demonstrates the potential of data-driven approaches in agricultural forecasting. By providing accurate yield predictions based on environmental and soil factors, it can help stakeholders in the agricultural sector make informed decisions about crop management, resource allocation, and policy planning. 

Future work could include:
1. Extending the model to predict yields for other crops in the dataset
2. Incorporating additional data sources such as satellite imagery or historical weather patterns
3. Developing a user-friendly interface or API for easier adoption by agricultural professionals
4. Exploring the impact of climate change scenarios on long-term yield predictions

By continuing to refine and expand this approach, we can contribute to more sustainable and efficient agricultural practices.
