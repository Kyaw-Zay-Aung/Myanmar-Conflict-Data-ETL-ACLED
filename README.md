# 🛡️ Myanmar-Conflict-Data-ETL-ACLED

> **⚠️ CRITICAL SECURITY WARNING**
> **DO NOT UPLOAD YOUR `.env` FILE TO GITHUB.** > This file contains your private API password. Always ensure `.env` is listed in your `.gitignore` before pushing code. 🛑

---

## **📌 Project Overview**
This project extracts and cleans conflict event data in Myanmar from **February 1, 2021**, to the same date of the previous year (e.g., if today is April 1, 2026, data will be provided up to April 1, 2025).

As **ACLED** maintains a strict verification process, there is a **one-year data lag** for the specific filtered records used in this project. By using the ACLED API, this pipeline ensures that the dataset is always updated with the latest available verified records.

---

## **✨ Key Features (What this project does)**

* **🚀 Easy Data Access:** Connects directly to the ACLED database to get the latest Myanmar conflict records without manual downloading.
* **💻 Smart Login System:** Works everywhere—whether you are using **Google Colab** or your own computer (**VS Code/PyCharm**).
* **🧹 High-Quality Cleaning:** Automatically fixes messy dates and fills in missing information to make the data ready for analysis.
* **🔍 Data Verification:** Includes built-in "Checks" to ensure there are no errors, duplicates, or wrong data types before you use it.
* **🎯 Specialized Filters:** Easily identifies specific events, such as those involving high-profile actors or specific social groups.

---
## **🛠️ How it Works (Simple Process)**
For those who are new to this project, here is the simple 4-step process the code follows:

1. **Connect:** The script logs into the **ACLED API** using your private credentials (stored safely in `.env` or Colab Secrets).
2. **Fetch:** It automatically gathers all relevant conflict records starting from **February 2021**.
3. **Clean & Verify:** It fixes errors in the raw data and runs a validation test to ensure the dataset is **100% accurate** and "clean."
4. **Export:** It saves the final, verified data into a neat **CSV file** ready for your research or visualization.

---

## **🚀 Getting Started**

### **1. Install Required Tools**
Make sure you have **Python** installed, then run this command in your terminal to install the necessary libraries:

pip install -r requirements.txt

---

### **2. Set Up Your Credentials**
To use the **ACLED API**, you need to provide your login details safely:

1.  **Locate Template:** Find the file named `.env.example` in the project folder.
2.  **Rename File:** Rename it to exactly `.env`.
3.  **Enter Details:** Open the `.env` file with a text editor and type in your ACLED email and password.

> [!IMPORTANT]
> **Security Note:** Your real password stays on your computer. It will **NOT** be uploaded to GitHub because the `.env` file is already listed in the `.gitignore` "shield."

---

### **3. Run the Project**
Once your credentials are set up, you are ready to go:

1.  **Open Notebook:** Open the `ACLED_Clean_Data.ipynb` file (using VS Code, Jupyter, or Google Colab).
2.  **Execute:** Click the **"Run All"** button at the top of the editor.
3.  **Finish:** The script will handle the rest and notify you as soon as your final **CSV file** is ready for use.

--- 

## **📂 Repository Structure**

* **`ACLED_Clean_Data.ipynb`**: The **"main brain"** of the project where data is fetched, cleaned, and verified.
* **`.gitignore`**: The **"shield"** that prevents your private passwords and `.env` files from being leaked to GitHub.
* **`requirements.txt`**: A simple list of the Python libraries (Pandas, Requests, etc.) required to run this project.
* **`.env.example`**: A safe template showing you exactly how to set up your private login file.
* **`README.md`**: The project documentation and guide (the file you are reading now).
