## BAZAARVOICE DATA SOURCE:
* Bazaarvoice is a digital marketing company based in Austin, Texas. It provides software that allows retailers to add customer reviews to their websites.
*Bazaarvocie is one of the data source through which data is retrieved from an API in json format. User need to input the date for which data need to be retrieved.Date can be backdated to reterive hsitorical data.Bazaarvocie API return review shared by customer for various Dyson products.

## Ingestion
<li> This script ingests data from Bazaarvoice i.e hit the bazaarvoice API and store the result which is Json file in AWS S3 bucket.</li> <br />
 First script hit product API fom which all the productId are stored temopory and for all productId respective review API is hit and json data return from this review API is store in S3 bucket. 
- Folder structure in main resposirtory for ingestion is made_master/ingestion/bazaarvoice/main
<li> Unit test case are developed which cover to test the functionality of each method written in main code. Folder structure in main resposirtory for unit test case is **made_master/ingestion/bazaarvoice/tests/unit** </li> <br />
<li> Integration test case are developed which cover to test the connection to AWS S3 bucket and data storage in same.Folder structure in main resposirtory where integration test case are written is **made_master/ingestion/bazaarvoice/tests/integration**</li>

## Modeling
<li> The main puprose of modeling to compress the json data for which .parquet file extension is used.User need to input the date for which modeling is to be done.</li> <br />
<li> pull the Json data from AWS S3 bucket and convert the file into parquet file format and push new parquet file back into AWS s3 bucket.</li> <br />
<li> Folder structure in main resposirtory for modeling is **made_master/modeling/bazaarvoice/main** </ li> <br />
<li> Unit test case are developed which cover to test the functionality of each method written in main code. Folder structure in main resposirtory is **made_master/modeling/bazaarvoice/tests/unit** </li> <br />
<li> Integration test case are developed which cover to test the connection to AWS S3 bucket and data storage in same.Folder structure in main resposirtory is **made_master/modeling/bazaarvoice/tests/integration**</li>

