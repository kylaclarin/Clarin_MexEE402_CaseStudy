# Clarin_MexEE402_CaseStudy
# MexEE 402: Data Preprocessing Case Study

MexEE Elective 2: Data Science and Machine Learning
Batangas State University, Alangilan Campus
1st Semester, AY 2026-2027

## 👤 Members

| Name | Student Number | Section |
|---|---|---|
| Clarin, Kyla Nicole F. | 20-03458 | MEXE - 4103 |

---

## 🔗 Notebook links

| Chapter | Member 1 | 
|---|---|
| Ch1_2_3 | [https://colab.research.google.com/drive/1UGICAYhnft6JnNV05ayw_6qMChwekXDd?usp=sharing]() | 
| Ch4 | [https://colab.research.google.com/drive/1iYa9tG_nkVzHZ5HSYQOFIlvqqwsANosu?usp=sharing]() | 
| Ch5 | [https://colab.research.google.com/drive/1W4TFxFUmmYx4KId1ja45wLgRxZuiaQ5J?usp=sharing]() | 
| Ch6 | [https://colab.research.google.com/drive/13qk_PptArr0kkWq0CM7OScsGTJFUZADy?usp=sharing]() | 
| Ch7 | [https://colab.research.google.com/drive/1qh6WhXX4XqtOss2srGZWlPJUr2OTzlpN?usp=sharing]() | 
| Ch8 | [https://colab.research.google.com/drive/1pmeJ0tR5Q0fK8GbyCAy3hwwB8ShBl_if?usp=sharing]() | 
| Ch9 | [https://colab.research.google.com/drive/1vMq9GEGmao1JurCf3fZoZ8UpjlX6MaSA?usp=sharing]() | 

---

## 💡 What I Learned

### **Chapter 1_2_3**
In these chapters, I learned how to upload and load a dataset, understand its data types, and clean it before using it for analysis or machine learning. I learned that raw data can have missing, inconsistent, or irrelevant information. And also, I learned how to handle it. What surprised me was that I need to upload the dataset first before running the code because it can cause an error if the data is not available. This helped me realize that data preparation isn't just about writing code, but also about properly setting up and organizing your files before doing any actual analysis.

### **Chapter 4**
In this chapter, I learned that feature engineering is about creating new features to make the data more useful. I learned about binning, interaction features, polynomial features, and encoding categorical data using one-hot and ordinal encoding. What surprised me was that we can create new information from existing data, such as Lemonade per Degree, to better understand relationships in the dataset. 

### **Chapter 5**
In Chapter 5, I learned that variables measured on totally different scales need to be rebalanced so the algorithm evaluates both fairly. What surprised me was how unscaled data can trick an algorithm into prioritizing a feature simply because its numbers are bigger, not because it actually matters more. In short, scaling balances all variables so predictions are based on true relationships rather than raw numerical sizes.

### **Chapter 6**
In this chapter, I learned that outliers are values that are very different from most of the data and can affect the results of an analysis. I learned how Z-score and IQR can be used to find these unusual values and how they can be handled properly. What surprised me was that an outlier should not always be removed because it may still represent important information.

### **Chapter 7**
In Chapter 7, I learned that feature selection removes useless variables so a model can focus only on what actually helps make predictions. What surprised me was that we can do this in different ways, like using statistical scores to filter them out beforehand, testing groups of variables using wrapper methods, or letting model algorithms like Lasso drop weak features on their own during training. In the end, I realized that feeding a model more data isn't always better, and trimming unnecessary features actually makes predictions sharper.

### **Chapter 8**
In this chapter, I learned how a preprocessing pipeline combines different steps, such as filling missing values and scaling data, into one process. I understood that this makes data preparation more organized and consistent. What surprised me was how pipelines prevent human mistakes and data leakage by applying the exact same transformations to both training and test data. In short, they keep machine learning projects organized, consistent, and easy to run. In addition to this, I also learned that if the dataset does not match what the code needs, the code may not work properly because some required columns or data are missing.

### **Chapter 9**
In this chapter, I learned how different preprocessing techniques can be combined to prepare a real dataset for analysis. I understood how to handle missing values, scale numerical data, encode categorical data, and use visualizations to better understand the processed data. What surprised me was how the plots made it easier to see patterns and differences in the data.

---

## ⚠️ Errors I Found

**ERROR:** Chapter 6

**Mistake:** I noticed that the Z-score method did not detect 100 as an outlier, while the IQR method identified it as an outlier. This may cause confusion because both methods are used to detect outliers. The Z-score method did not detect it because its Z-score was only 2.615, which is within the stated cutoff of -3 to 3.

**Correction:** The results do not necessarily need to be the same because the two methods use different criteria. That is why 100 was not detected as an outlier using the Z-score method but was identified as an outlier using the IQR method. The existing Z-score code is correct based on the cutoff used, so no code correction is necessary.

However, if the goal is to make the Z-score method also identify 100 as an outlier, the cutoff can be changed from 3 to 2.5.

**Original Code:**

outliers = data[np.abs(z_scores) > 3]

**Corrected Code (if using a cutoff of 2.5):**

outliers = data[np.abs(z_scores) > 2.5]

Changing the cutoff to 2.5 will allow the Z-score method to detect 100 as an outlier because its Z-score of 2.615 is greater than 2.5. 

---

## 📝 Note on AI tools

I used ChatGPT to help me understand the error I found in Chapter 6. I asked if it was possible for the Z-score and IQR methods to produce different results in detecting outliers. It helped me understand why the Z-score method did not identify 100 as an outlier while the IQR method did, and what changes could be made to the cutoff if I wanted both methods to identify it.

---

## 📚 References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.

VanderPlas, J. Python Data Science Handbook.

GregorySmith. (n.d.). Video Game Sales. Kaggle. [https://www.kaggle.com/datasets/gregorut/videogamesales]()

Anakha, A. S. (n.d.). Titanic Dataset. Kaggle. [https://www.kaggle.com/datasets/anakha27/titanic-dataset]()
