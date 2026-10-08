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
| Ch1_2_3 | [link](https://colab.research.google.com/drive/1UGICAYhnft6JnNV05ayw_6qMChwekXDd?usp=sharing) | 
| Ch4 | [link](https://colab.research.google.com/drive/1iYa9tG_nkVzHZ5HSYQOFIlvqqwsANosu?usp=sharing) | 
| Ch5 | [link](https://colab.research.google.com/drive/1W4TFxFUmmYx4KId1ja45wLgRxZuiaQ5J?usp=sharing) | 
| Ch6 | [link](https://colab.research.google.com/drive/13qk_PptArr0kkWq0CM7OScsGTJFUZADy?usp=sharing) | 
| Ch7 | [link](https://colab.research.google.com/drive/1qh6WhXX4XqtOss2srGZWlPJUr2OTzlpN?usp=sharing) | 
| Ch8 | [link](https://colab.research.google.com/drive/1pmeJ0tR5Q0fK8GbyCAy3hwwB8ShBl_if?usp=sharing) | 
| Ch9 | [link](https://colab.research.google.com/drive/1vMq9GEGmao1JurCf3fZoZ8UpjlX6MaSA?usp=sharing) | 

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

List any mistake you found in the original notebooks, and the correct version.
There are real ones in there. Finding them earns points.

---

## 📝 Note on AI tools

Say whether you used an AI tool, and what for. This is not a penalty.
Hiding it is.

---

## 📚 References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.
VanderPlas, J. Python Data Science Handbook.
Any other page or article you used.
