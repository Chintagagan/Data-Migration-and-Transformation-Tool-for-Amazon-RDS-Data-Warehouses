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
2. Configure your AWS credentials using the AWS CLI or environment variables:
    aws configure
  
  Alternatively, export your credentials:
    - export AWS_ACCESS_KEY_ID=your_access_key_id
    - export AWS_SECRET_ACCESS_KEY=your_secret_access_key
    - export AWS_DEFAULT_REGION=your_region

### **How to Run the Script**
1. Clone the Repository:
  '''bash
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
2. Update Configuration in the Script:
   - Open the script and update the following variables:
 '''python
    - URL = "https://example.com/path/to/your/zipfile.zip"
    - S3_BUCKET = "your-s3-bucket-name"
    - RDS_ENDPOINT = "your-rds-endpoint"
    - RDS_DATABASE = "your-database-name"
    - RDS_USERNAME = "your-rds-username"
    - RDS_PASSWORD = "your-rds-password"
###** Script Workflow **
1.Download the Zip File: The requests library is used to download the zip file from the given URL.
2.Extract JSON Files: The zipfile module extracts JSON files from the archive.
3.Process JSON Data: Each JSON file is read, parsed, and converted into a list of dictionaries or a DataFrame using pandas.
4.Upload to Amazon S3:
  - The processed JSON files are uploaded to the specified S3 bucket using the boto3 library.
5.Load Data into RDS:
  - Data is loaded into Amazon RDS using the pandas DataFrame and sqlalchemy.



### **Instructions**
- Replace placeholders like `your-username`, `your-repo-name`, `your.email@example.com`, and AWS-related configuration details with your actual project information.
- Copy and paste this directly into your `README.md` file.

### **Contact**
For any questions or issues, please contact:
  - Name: Chinta Gagan Susveer
  - Email: chintagagan@gmail.com





