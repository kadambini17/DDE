## BOLDCHAT DATA SOURCE:
<li> BoldChat offers live communication software including chat, email management, and click to call tools to help businesses control customer <b> interactions</b> and boost website sales. </li><br />
* BoldChat is one of the data source through which data is retrieved from an API in json format. User need to input the date for which data need to be retrieved.There are 6 different market/region GB, IE, US, CA, JP and AU.which further classify data reterival.

## Ingestion
* This script ingests data from BoldChat i.e Hit the boldchat API and store the result which is Json file in AWS S3 bucket.
* Below are the request type for which Ingestion is handled:
  >> Emails <br />   >> Chats <br /> >> Operators<br /> >> Contacts <br />  >> Departments  <br />
* Folder structure in main resposirtory for ingestion is **made_master/ingestion/boldchat/main**    <br />
* Unit test case are developed which cover to test the functionality of each method written in main code. Folder structure in main resposirtory for unit test case is **made_master/ingestion/boldchat/tests/unit** <br />
* Integration test case are developed which cover to test the connection to AWS S3 bucket and data storage in same.Folder structure in main resposirtory where integration test case are written is **made_master/ingestion/boldchat/tests/integration** 

## Modeling
* The main puprose of modeling to compress the json data for which .parquet file extension is used. 
* pull the Json data from AWS S3 bucket and convert the file into parquet file format and push new parquet file back into AWS s3 bucket.
* Folder structure in main resposirtory for modeling is **made_master/modeling/boldchat/main** <br />
* Unit test case are developed which cover to test the functionality of each method written in main code. Folder structure in main resposirtory is **made_master/modeling/boldchat/tests/unit** <br />
* Integration test case are developed which cover to test the connection to AWS S3 bucket and data storage in same.Folder structure in main resposirtory is **made_master/modeling/boldchat/tests/integration**

