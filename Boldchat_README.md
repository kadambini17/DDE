## BOLDCHAT DATA SOURCE:
BoldChat is one of the data source from which data is retrieved from an API in json format based on date and Region as input from user.
## Ingestion
This script ingests data from BoldChat i.e Hit the boldchat API and store the result which is Json file in AWS S3 bucket.
Below are the request type for which Ingestion is handled: < br />
 <ul> <li> Emails</li> <li> Chats </li>  <br /> <li> Operators </li> <li> Contacts </li>  <br /> <li> Departments </li> </ul> <br />
Folder structure in main resposirtory is as follow:<br />
**made_master/ingestion/boldchat/main** <br />
Unit test case are developed which cover to test the functionality of each method written in main code. Folder structure in main resposirtory is as follow:<br />
**made_master/ingestion/boldchat/tests/unit** <br />
Integration test case are developed which cover to test the connection to AWS S3 bucket and data storage in same.Folder structure in main resposirtory is as follow:<br />
**made_master/ingestion/boldchat/tests/integration**

## Modeling
