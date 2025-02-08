# 📈 Zambia Stock Market Data Pipeline

🚀 **An end-to-end data engineering pipeline for Zambia's stock market using Apache Airflow, PostgreSQL, AWS S3, and Looker Studio.**  

---

## **📉 Background**

The **Lusaka Securities Exchange (LuSE)**, established in 1993 with assistance from the **International Finance Corporation (IFC)** and the **World Bank**, commenced operations on **February 21, 1994**. ([luse.co.zm](https://www.luse.co.zm/about-us/?utm_source=chatgpt.com)) As Zambia’s principal stock exchange, LuSE facilitates the trading of equities, bonds, and other securities, playing a crucial role in the country’s capital markets.

However, **market data accessibility remains a challenge**. Unlike more established exchanges, LuSE does not provide **APIs or centralized data feeds**, making it difficult for analysts and investors to obtain real-time or historical market information. This lack of transparency and data availability contributes to **low market participation** and limits research-driven investment strategies.

### **🚀 About This Project**
This repository demonstrates **an end-to-end data engineering pipeline** designed to **automate the collection, processing, and visualization** of **LuSE stock market data and Bank of Zambia exchange rates**. The goal is to showcase how **data engineering techniques** can improve market transparency and accessibility in an emerging financial market.

### **⚠️ Disclaimer**
🚨 **This is an example project and NOT a production-ready financial application.**  
- The data pipeline relies on **web scraping**, which is subject to website changes.  
- No guarantees are made regarding **data accuracy, completeness, or reliability**.  
- This project is for **educational and research purposes only**.  

If you're an investor, always use **official sources** or consult a financial expert before making investment decisions.

---

## **🔮 Architecture**
```
[ Web Scraper ] ➞ [ S3 Bucket ] ➞ [ Airflow DAG ] ➞ [ RDS PostgreSQL ] ➞ [ Looker Dashboard ]
```
- **Scrapes data daily** from LuSE & Bank of Zambia (BoZ)
- **Uploads CSV to AWS S3**
- **Processes & stores data** in PostgreSQL (AWS RDS)
- **Visualizes market trends** via Looker Studio

---

## **📊 Features**
- **Automated Web Scraping** (“BeautifulSoup”, “Selenium”) for LuSE stock prices & BoZ exchange rates.
- **ETL Orchestration** using **Apache Airflow**.
- **Data Storage** in **AWS S3** and **PostgreSQL (AWS RDS)**.
- **Looker Studio Dashboard** for real-time market insights.

---

## **💻 Tech Stack**
| Component          | Tool/Service            |
|------------------|---------------------|
| **Web Scraping** | BeautifulSoup, Selenium, Pandas |
| **Storage**      | AWS S3 (CSV files)   |
| **Database**     | PostgreSQL (AWS RDS) |
| **Orchestration**| Apache Airflow      |
| **Visualization**| Looker Studio       |

---

## **🗒️ Setup & Installation**

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/yourusername/zambia-stock-market-data-pipeline.git
cd zambia-stock-market-data-pipeline
```

### **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3️⃣ Configure AWS Credentials**
```bash
aws configure
```

### **4️⃣ Run Web Scraper**
```bash
python scraper.py
```

### **5️⃣ Deploy Airflow DAG**
```bash
airflow scheduler &
airflow webserver --port 8080 &
```

---

## **🔍 Data Model**

A **diagram of the data model** will be uploaded soon. *(To be updated)*

---

## **📺 Architecture Diagram**

A **detailed architecture diagram** will be uploaded soon. *(To be updated)*

---

## **📈 Dashboard in Looker Studio**
### 💎 **Real-time Visualizations**
- 📈 **Stock Performance Trends**
- 💰 **Market Capitalization in USD**
- 📆 **Exchange Rate Trends (ZMW/USD)**

### **📍 View Live Dashboard**
👉 [Looker Studio Dashboard](https://lookerstudio.google.com) *(Coming Soon)*

---

## **🏃️ Next Steps**
✅ Add **historical data backfilling**  
✅ Implement **alerts for Airflow failures**  
✅ Automate **EC2 startup scripts**  

---

## **💪 Contributing**
🔹 Fork the repository  
🔹 Open a pull request  
🔹 Report issues via GitHub  

---

## **📄 License**
🖊️ MIT License - Free to use and modify.

---

## **👥 Contact**
📧 **Your Name** – [your.email@example.com](mailto:your.email@example.com)  
📞 **LinkedIn** – [linkedin.com/in/yourname](https://linkedin.com/in/yourname)  

