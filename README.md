# README
Code to Support the CivTechSA Datathon\
Send questions to datathon@allosense.com

# REQUIREMENTS
- Amazon Web Services access (https://console.aws.com)
- National Instruments LabVIEW 2020 (https://www.ni.com/en-us/support/downloads/software-products/download.labview.html)
- Tableau (https://www.tableau.com/products/desktop)

# PROGRAMS
### 1. Allosense - File to AWS Athena Converter.vi
  Prepares .csv files to be used with AWS Athena that runs standard SQL queries (https://aws.amazon.com/athena/).<br />
#### Input
  - .CSV formatted files<br />
#### Output
  - Updated .CSV (Timestamp Formatted)
  - Header Datatype Table .TXT (for AWS Athena)
  - Saved Header Configurations .BIN<br /><br />

### 2. Allosense - File to AWS NoSQL Converter.vi
  Sample program that sends .csv file to AWS DynamoDb NoSQL database. The code requires AWS CLI to run.<br />
#### Input
  - .CSV formatted files<br />
#### Output
  - Sends data to DynamoDb<br /><br />

# SQL QUERIES
If you want to make a SQL call:\
  Open Tableau -> To a Server -> More... -> Installed Connectors -> Amazon Athena\
Enter the following credentials:
- Server:               athena.us-east-1.amazonaws.com
- Port:                 443
- S3 Staging Directory: s3://allosense-2021-datathon/athena-query/
- Access Key ID:        AKIA5HOYAEX3PUYVVNOU
- Access Key:           C7ZoePAwnL7blD8pOE5hyKAjZgOpwJ1S3kbeSTRJ
