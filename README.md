****S3****
1. Create s3-bucket-a
2. Create s3-bucket-b

****IAM****
1. Create IAM Policy - IAM.JSON
2. Create an execution role tor the Lambda service and attach the above created policy

****Lambda****
1. Create a function called "handler"
2. Upload the repo file handler.zip
3. Create a Layer using  - arn:aws:lambda:us-east-1:770693421928:layer:Klayers-p38-Pillow:3
     "This layer includes the PIL (python image library)"

****s3****
1. Create an s3 event trigger for "create objects" and target the destination to the lambda arn created above.  The lambda arn can be found on the function handler (EG:arn:aws:lambda:us-east-1:711392004085:function:handler)


TASK2
1. Create 2 IAM policies using the json policy files 
2. On userB - Attach the BucketB read only policy
3. On userA - Attach the BucketA RW policy



