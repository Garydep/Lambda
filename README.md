****S3****
Create s3-bucket-a
Create s3-bucket-b

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




