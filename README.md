****S3****
1. Create s3-bucket-a
2. Create s3-bucket-b

****IAM****
Create IAM Policy - IAM.JSON
Create execution for policy on Lambda

****Lambda****
Create function called "handler"
Upload handler.zip
Create Layer - arn:aws:lambda:us-east-1:770693421928:layer:Klayers-p38-Pillow:3
    This layer includes the PIL (python image library)

****s3****
Create s3 event trigger for "create objects" and destination to the lambda arn created above


TASK2
Create 2 IAM policies using the json policy files 
On userB - Attach the BucketB read only policy
On userA - Attach the BucketA RW policy



