# lambda-source-bucket
Lambdaのソースを管理するためのS3バケットを作るやつ

## Initialize
```
$ aws cloudformation create-stack \
  --stack-name <Your Stack Name> \
  --template-body file://cloudformation/s3.yml \
  --parameters \
    ParameterKey=BucketName,ParameterValue=<Your S3 Bucket Name>
```

## Delete
```
$ aws cloudformation delete-stack \
  --stack-name <Your Stack Name>
```
