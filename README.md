# 🧹 Data Cleaning Using Pure Python

A beginner-level **Data Analysis / Data Cleaning project built using pure Python**.

This was my **first Data Analysis project**, created to practice working with JSON data, identifying data-quality problems, cleaning datasets, and exporting the cleaned data.

## 📌 Project Overview

The project works with a JSON dataset containing:

* Users
* Friends/connections
* Liked pages
* Pages

The original dataset contains several common data-quality problems, such as:

* Missing user names
* Duplicate friends
* Inactive users
* Duplicate page IDs

The goal of this project is to clean the dataset using **Python only**, without using Pandas or other data-analysis libraries.

## 🛠️ Technologies Used

* **Python**
* **JSON**
* Python built-in `json` module
* Lists
* Dictionaries
* Sets
* Loops
* Functions
* List Comprehension

## 🔍 Data Cleaning Process

The project contains a `clean_data()` function that performs several cleaning operations.

### 1. Remove Users With Missing Names

Users whose names are empty are removed from the dataset.

For example, the original dataset contains a user with an empty name.

### 2. Remove Duplicate Friends

Duplicate friend IDs are removed using a Python `set`.

For example:

```text
Before:
friends = [2, 2]

After:
friends = [2]
```

### 3. Remove Inactive Users

Users who have neither friends nor liked pages are removed.

This helps eliminate users who don't contain useful activity information.

### 4. Remove Duplicate Pages

Duplicate page IDs are removed using a dictionary.

The original dataset contains page ID `104` twice, with different page names. The cleaning process keeps the final occurrence.

### 5. Save the Cleaned Dataset

After cleaning, the processed data is exported into:

```text
cleaned_data2.json
```

The resulting dataset contains cleaned users and unique pages.

## 📂 Project Structure

```text
Data-Cleaning-Pure-Python/
│
├── lec_02_S_Actual_coding.ipynb
├── data2.json
├── cleaned_data2.json
└── README.md
```

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Saadkhan-777/Data-Analysis-1st-Project.git
```

### 2. Open the Jupyter Notebook

Open:

```text
code.ipynb
```

You can run it using:

* Jupyter Notebook
* JupyterLab
* Google Colab
* VS Code

### 3. Run the notebook

The notebook loads:

```text
data2.json
```

cleans the data, and generates:

```text
cleaned_data2.json
```

## 📊 Before vs After

### Before Cleaning

The dataset contains:

* A user with a missing name
* Duplicate friend IDs
* An inactive user
* Duplicate page IDs

### After Cleaning

The dataset contains:

* Valid user records
* Unique friend IDs
* Active users
* Unique page IDs
* Cleaned JSON structure

## 🎯 What I Learned

Through this project, I practiced:

* Reading JSON files using Python
* Working with nested dictionaries and lists
* Creating reusable Python functions
* Using list comprehensions
* Using sets to remove duplicates
* Using dictionaries for unique records
* Detecting and handling missing data
* Cleaning real-world-style messy data
* Writing cleaned data back to JSON

## 🚀 Future Improvements

I plan to extend this project by:

* Adding more data-validation rules
* Generating data-quality reports
* Adding basic data analysis
* Creating visualizations
* Rebuilding the project using **Pandas**
* Comparing pure Python data cleaning with Pandas

## 👨‍💻 Author

**Saad Khan**

BS Computer Science Student | Aspiring AI/ML Engineer

---

⭐ If you find this project useful, feel free to explore the repository and follow my learning journey in **Python, Data Analysis, AI, and Machine Learning**.
