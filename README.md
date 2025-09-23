# Marketing Campaign Data Analysis (PySpark)

## 📌 Project Overview
This project analyzes **marketing campaign data** using **PySpark** on a Dataproc/HDFS environment.  
It processes raw JSON datasets from ad campaigns, user profiles, and store details to generate insights such as campaign performance, user engagement, and store-based analysis.  
The results are written back into HDFS in **nested JSON format**, ready for Hive queries and reporting.

---

## 📂 Project Structure

├── Untitled-1.py # Main PySpark script (solutions for Q1, Q2, Q3)
├── README.md # Project documentation
├── input_data/ # Raw JSON files
│ ├── ad_campaigns_data.json
│ ├── user_profile_data.json
│ └── store_data.json
└── output_data/
└── marketing_DA/ # Results written in JSON format
├── ques_1/
├── ques_2/
└── ques_3/


---

## 🛠️ Technologies Used
- **PySpark** (DataFrame API)
- **HDFS** for storage
- **Hive** for external table creation
- **Dataproc** (or local Spark environment)

---

## 📑 Input Data
Three JSON files are required in the `input_data/` directory:

1. **ad_campaigns_data.json**  
   Contains campaign events such as impressions, clicks, and video ads.  

   Example:
   ```json
   {
     "campaign_id": "ABCDFAE",
     "campaign_name": "Summer Sale",
     "campaign_country": "US",
     "os_type": "android",
     "device_type": "mobile",
     "place_id": "CASSBB-11",
     "user_id": "U123",
     "event_type": "impression",
     "event_time": "2018-10-12T13:00:00"
   }

user_profile_data.json
Contains user demographic and interest details.

Example:

{
  "user_id": "U123",
  "country": "US",
  "gender": "M",
  "age_group": "25-34",
  "category": ["fashion", "electronics"]
}

store_data.json
Contains mapping of store names to place IDs.

Example:

{
  "store_name": "McDonald",
  "place_ids": ["CASSBB-11", "CADGBD-13", "FDBEGD-14"]
}

