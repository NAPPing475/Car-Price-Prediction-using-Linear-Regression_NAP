# Car-Price-Prediction-using-Linear-Regression_NAP


**CAR PRICE PREDICTION USING AUTO-REGRESSION MODEL**

**Objective:**
- **To Predict Car Prices** based on the **Type of Fuel**, **Kilometers Driven**, and the **Year of the Model** using an **Auto Regression Model**.

**Methodology:**
1. **Data Source:**
   - **Dataset:** **Quikr Car Sales Data**.
   - **Models Used:** **Linear, Non-Linear**, and **Classification Models** were built and evaluated for accuracy.
2. **Preprocessing Steps:**
   - **Format Adjustment:** Converted the **Year** column from **object** to **integer** using `.astype(int)`.
   - **Price Cleanup:** Removed non-numeric values (e.g., **"Ask for Price"**) and commas, followed by converting to **integer**.
   - **Kilometer Cleanup:** Stripped **"kms"** from **Kms Driven** values and converted to **integer**.
   - **Handling Missing Data:** **NaN** values in **Fuel_Type** were removed.

3. **Model Creation:**
   - **Simple Linear Regression Model** was created to predict car prices.
   - **Prediction Function:** The **pipe.predict()** function was used to estimate **Car Price** based on the independent variables: **Type of Fuel**, **Kilometers Driven**, and the **Year** of the model.

**Data Visualizations:**
- **Visualizing Relationships:**
   - **Company vs. Price**
   - **Year vs. Price**
   - **Kilometers Driven vs. Price**
   - **Fuel Type vs. Price**
   - **Fuel Type, Year, and Company** combined in a **Multi-variable Plot**.
 
     
 **Checking Relation Between Company with Price**
    
![image](https://github.com/user-attachments/assets/9407ca19-ab90-428f-a2a0-466f9d379b72)

**Checking Relation Between Year with Price**
![image](https://github.com/user-attachments/assets/17fba3ab-b894-4fba-9795-6ea9296fc66a)

**Checking Relation Between Kms_Driven with Price**
![image](https://github.com/user-attachments/assets/073aed41-976c-42b1-8c47-65c776a701b7)
    
**Checking Relation Between Fuel_Type with Price**
![image](https://github.com/user-attachments/assets/03e49109-58ed-4175-b42f-6c1883ce5d5d)
    
**Checking Relation Between Fuel_Type ,Year and Company**
![image](https://github.com/user-attachments/assets/5650709d-eb32-4c12-a5f1-f3dc26f7b255)

    
****





**Model Comparison:**
- **Train/Test Split:** Used the **train_test_split()** method from **sklearn.model_selection** to divide the data into training and testing sets.
- **Handling Categorical Data:** Applied **OneHotEncoder** to handle **Fuel_Type** and other categorical variables.

**Accuracy Metrics:**
- **R-Squared and Adjusted R-Squared:** Chose **Adjusted R-Squared** to measure how well the model fits the data, with **Random State** tuning to maximize accuracy.
![image](https://github.com/user-attachments/assets/6255a9ad-3f26-4c0b-b548-ea72c3b09d91)
- **Looping for Optimal Random State:** A loop was applied to find the **best random state** that yields maximum accuracy for the prediction model.
![image](https://github.com/user-attachments/assets/236d0bb9-c813-4e61-9cef-bbc0422fa227)

**Prediction From Training Dataset:**
![image](https://github.com/user-attachments/assets/b94473e5-548e-4edf-bf54-79b10a3ce277)

- **Car:** **2006 Toyota Corolla**.
   - **Kilometers Driven:** 5100.
   - **Fuel Type:** Petrol.
   - **Predicted Price:** **₹428,873.63** (Four Hundred Twenty-Eight Thousand, Eight Hundred Seventy-Three Rupees).

**Conclusion:**
- The model provides a reliable estimate of car prices with a high degree of accuracy based on essential independent variables.
  

