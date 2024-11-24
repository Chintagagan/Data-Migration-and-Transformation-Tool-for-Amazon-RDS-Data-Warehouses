# Data-Migration-and-Transformation-Tool-for-Amazon-RDS-Data-Warehouses

# JSON Data Extraction and Loading into Amazon S3 and RDS

This project demonstrates how to extract data from a zip file containing multiple JSON files, store the data in Amazon S3, and load it into Amazon RDS using Python. The script downloads the zip file from a given URL, extracts the JSON files, processes the data, uploads it to S3, and then stores it in an RDS instance.

---

## **Features**

- Downloads a zip file from a URL.
- Extracts multiple JSON files from the zip archive.
- Processes the JSON data into structured formats.
- Stores processed data as JSON files in Amazon S3.
- Loads data into an Amazon RDS (NoSQL or SQL) instance.

---

## **Technologies Used**

- **Python Libraries**: 
  - `requests`: For downloading the zip file.
  - `zipfile`: For extracting data from the zip file.
  - `boto3`: For interacting with Amazon S3.
  - `pandas`: For processing JSON data.
  - `sqlalchemy`: For interacting with Amazon RDS.
- **Amazon Web Services**:
  - S3
  - RDS (NoSQL or SQL)

---

## **Setup and Prerequisites**

### **AWS Requirements**
1. Create an S3 bucket to store the JSON files.
2. Set up an Amazon RDS instance (SQL or NoSQL) for data storage.
3. Ensure your AWS IAM user or role has the following permissions:
   - `s3:PutObject`
   - `s3:GetObject`
   - `rds:Connect`

### **Python Environment**
1. Install the required libraries:
   ```bash
   pip install requests boto3 pandas sqlalchemy pymysql
