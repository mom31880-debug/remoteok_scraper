# 🌐 RemoteOK Job Scraper

Scraping and analyzing real job listings from RemoteOK to find the most in-demand skills and roles in the tech market.

---

## 📁 Data Source
- **Website:** [RemoteOK.com](https://remoteok.com)
- **API:** `https://remoteok.com/api`
- **Size:** 98 real job listings

---

## 🛠️ Tools Used
- `Python`
- `Requests` — fetching data from the API
- `Pandas` — data cleaning and analysis
- `Matplotlib` — visualization

---

## 📋 Steps

### 1️⃣ Check robots.txt
Verified that RemoteOK allows scraping before starting.
```
User-agent: *
Allow: /
Crawl-delay: 1
```

### 2️⃣ Fetch Data
Used RemoteOK API to get real job listings in JSON format.

### 3️⃣ Data Cleaning
- Extracted relevant fields: `position`, `company`, `location`, `tags`, `date`
- Cleaned date format
- Filled empty locations with "Remote"

### 4️⃣ Analysis
- Most in-demand skills
- Most in-demand roles
- Top skills by city

---

## 📊 Key Findings
- Most in-demand **role**: Engineer (28 jobs)
- Most in-demand **skills**: Senior, Technical, Engineer
- Most jobs are **Remote**

---

## 🚀 How to Run
```bash
pip install requests pandas matplotlib
jupyter notebook remoteok_scraper.ipynb
```
