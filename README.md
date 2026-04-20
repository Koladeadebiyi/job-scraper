# 🧑‍💻 Python Job Scraper (Fake Jobs Website)

## 📌 Project Overview

This project is a beginner-friendly **Python web scraper** that collects job listings from the Fake Jobs website.

It automatically extracts key job information and saves it into a CSV file for easy analysis.

---

## 🎯 What This Project Does

The scraper will:

* Visit the job listing website
* Extract:

  * Job Title
  * Company Name
  * Location
  * Job Application Link
* Save the data into a structured CSV file

---

## 🌐 Data Source

We are scraping from:

👉 https://realpython.github.io/fake-jobs/

This is a practice website designed for learning web scraping.

---

## 🧰 Tools & Libraries Used

| Tool          | Purpose                      |
| ------------- | ---------------------------- |
| Python        | Programming language         |
| requests      | Fetch webpage content        |
| BeautifulSoup | Parse and extract HTML data  |
| pandas        | Store and export data to CSV |
| VS Code       | Code editor                  |

---

## 📁 Project Structure

```
job-scraper/
│── scraper.py      # Main script
│── jobs.csv        # Output file (generated after running)
│── README.md       # Project documentation
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```
git clone https://github.com/your-username/job-scraper.git
cd job-scraper
```

### 2. Install Dependencies

```
pip install requests beautifulsoup4 pandas
```

---

## ▶️ How to Run the Project

Run the script using:

```
python scraper.py
```

After running successfully, a file will be created:

```
jobs.csv
```

---

## 🧠 How It Works (Step-by-Step Flow)

1. **Send Request**
   The script connects to the website using `requests`.

2. **Parse HTML**
   The page content is converted into a readable format using `BeautifulSoup`.

3. **Find Job Listings**
   All job cards are located using their HTML class.

4. **Extract Data**
   For each job, the script collects:

   * Title
   * Company
   * Location
   * Application link

5. **Handle Missing Data**
   If any field is missing, it safely assigns `None`.

6. **Store Data**
   All job records are saved into a list.

7. **Export to CSV**
   The data is converted into a table using `pandas` and saved as `jobs.csv`.

---

## 📊 Sample Output

| Job Title | Company | Location | Apply Link |
| --------- | ------- | -------- | ---------- |

---

## ⚠️ Edge Cases Handled

* Network errors (e.g., no internet connection)
* Missing job fields
* Empty results

---

## 🚀 Future Improvements

* Add keyword filtering (e.g., only "Python" jobs)
* Automate scraper to run daily
* Store data in a database (PostgreSQL / SQLite)
* Build a dashboard (Streamlit / Power BI)
* Scrape real job platforms

---

## 📚 Learning Outcomes

By completing this project, you will understand:

* Basics of web scraping
* How HTML structure works
* Data extraction techniques
* Handling errors in real-world scripts
* Saving structured data for analysis

---

## 🙌 Author

**koladeAdebiyi**

