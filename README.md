🏠 Kolkata House Price Prediction App
 
This is a **machine learning web app* built with **Streamlit** that predicts house prices in Kolkata based on key features like square footage, location, number of bedrooms, and bathrooms.

📁 Project Structure
  
```
├── app.py                             # Streamlit app for house price prediction
├── House_price_prediction.ipynb      # Jupyter notebook for data preprocessing and model training
├── House_Prediction_Model.pkl        # Trained ML model using Linear Regression
├── cleaned_data.csv                  # Cleaned dataset used for model training and prediction
├── Kolkata.csv                       # Raw or location-based housing data
├── README.md                         # Project overview and setup guide
```
 
--- 
  
🧠 Features

* Predicts house prices based on:

  * ✅ Area (in square feet)
  * ✅ Location in Kolkata
  * ✅ Number of bedrooms
  * ✅ Number of bathrooms
* Pre-trained machine learning model (Linear Regression or similar)
* Simple and interactive user interface with **Streamlit**

🏗️ Tech Stack

| Component        | Technology           |
| ---------------- | -------------------- |
| Language         | Python               |
| Web Framework    | Streamlit            |
| Machine Learning | scikit-learn, pandas |
| Interface Inputs | Streamlit Widgets    |

🚀 How to Run the Project

 🔧 1. Install Requirements

Make sure you have Python 3.8 or later installed. Then run:

```bash
pip install -r requirements.txt
```

If you don’t have a `requirements.txt`, here are the dependencies:

```bash
pip install streamlit pandas scikit-learn
```

---

🖥️ 2. Run the App

```bash
streamlit run app.py
```

Make sure the model (`House_Prediction_Model.pkl`) and dataset (`cleaned_data.csv`) are in the correct paths as referenced in `app.py`. If needed, update the paths like below:

```python
model = PK.load(open('House_Prediction_Model.pkl', 'rb'))
data = pd.read_csv('cleaned_data.csv')
```

---  

🧪 Model Details

* The model was trained using **cleaned\_data.csv**
* Feature columns:

  * Area (Sqft)
  * Location
  * Number of Bedrooms
  * Number of Bathrooms
* Target: Price (in INR)
* ML Algorithm: Likely Linear Regression (as observed in the Jupyter Notebook)


## 📸 App Preview

Once the app is running, it shows:

* A dropdown to select location
* Numeric input fields for area, bedrooms, and bathrooms
* A **"Predict Price"** button
* Output: Predicted price in INR (scaled/adjusted by a factor of 1.8)

---

📝 To-Do

* ✅ Add error handling for invalid or missing inputs
* ✅ Use relative file paths instead of absolute paths for portability
* 🔲 Deploy the app using Streamlit Cloud or other platforms
* 🔲 Enhance the UI with more styling/custom branding
* 🔲 Improve model accuracy with additional features like furnishing status, floor, amenities, etc.


📚 License

This project is for educational purposes only. Feel free to use and modify it.


🙋‍♂️ Author

Arunava Chakraborty
Beginner in Machine Learning and Python
Learning through hands-on projects 🚀

